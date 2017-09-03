package dogeMeme;

import com.sun.speech.freetts.*;

import java.awt.Container;
import java.awt.Graphics;
import java.awt.Graphics2D;
import java.awt.RenderingHints;

import javax.swing.JComponent;
import javax.swing.JFrame;

/* Made thanks to open source FreeTTS library.
 * Created by Andrew Obrzut
 * aobrzut2@illinois.edu
 */

public class lab0 {
	private static final String VOICENAME = "kevin16";
	public static void main(String[] args) {
		Voice voice;
		VoiceManager vm = VoiceManager.getInstance();
		voice = vm.getVoice(VOICENAME);
		
		voice.allocate();
		
		JFrame jf = new JFrame("Doge Memes");
	    Container cp = jf.getContentPane();
	    doges tl = new doges();
	    cp.add(tl);
	    jf.setSize(350, 200);
	    
	    jf.setVisible(true);
		try {
			voice.speak("Hello World!!");
			voice.speak("Dank memes make for sweet dreams.");
		} catch(Exception e) {}
	}
	
	
	

}


class doges extends JComponent {

	 
	  public void paintComponent(Graphics g) {
	      if(g instanceof Graphics2D)
	      {
	        Graphics2D g2 = (Graphics2D)g;
	        g2.setRenderingHint(RenderingHints.KEY_ANTIALIASING,
	        RenderingHints.VALUE_ANTIALIAS_ON);

	        g2.drawString("Hello World!" + "\n Dank memes make for sweet dreams.",20,20); 
	       }
	   }
}
