# DJster
Repository for the DJster software

<strong>Installation</strong>
<ol>
	<li>Use the installer version for your platform</li>
	<li>Make sure you set Max application in the Live preferences to Max 6.1</li>
	<li>Locate DJster.als in the Ableton User Library and open the file.</li>
	<li>Set Mode to "key"</li>
	<li>Turn player on by clicking on the Stream button</li>
	<li>Set Eventfulness to a value greater than 0</li>
	<li>You should now be able to hear the sounds</li>
</ol>
<div></div>
<div><strong>Scale</strong></div>
<div>When opening DJster for the first time it automatically tries to load a file called basic.cents.txt containing the definitions of some well-known scales.</div>
<div></div>
<div>
<blockquote>
pentatonic 0 200 400 700 900 1200<div>
whole-tone 0 200 400 600 800 1000 1200<div>
major 0 200 400 500 700 900 1100 1200<div>
dorian 0 200 300 500 700 900 1000 1200<div>
mixolydian 0 200 400 500 700 900 1000 1200<div>
minor-harmonic 0 200 300 500 700 800 1100 1200<div>
gipsy 0 200 300 600 700 900 1000 1200<div>
phrygian 0 100 300 500 700 800 1000 1200<div>
octatonic 0 200 300 500 600 800 900 1100 1200<div>
whole-half-half 0 200 300 400 600 700 800 1000 1100 1200<div>
chromatic 0 100 200 300 400 500 600 700 800 900 1000 1100 1200</blockquote>
</div>
<div></div>
<div>Each line contains the name of a scale and the cent values for the steps in between the frame at which the scale will be replicated, usually the octave.</div>
<div>A microtonal scale may use values other than multiples of 100 and a non-octave frame such as this one</div>
<div></div>
<blockquote>Lambda 0 293 439 585 878 1024 1317 1463 1756 1902</blockquote>
<div></div>
<div>You can also create your own definitions and/or add .scl files from the Scala archive. Scala files can also be added by dragging and dropping them from the Finder or Explorer onto the scale menu.</div>
<div></div>
<div>The TProfile menu refers to a tonality profile according to which the raw cent values are translated into an intervallic ratio in respect to given fundamental (tonic pitch). This is the basis for the establishment of a tonal hierarchy which is intimately linked with the harmoniclarity parameter, i.e. (with a non-zero harmoniclarity value) the higher the tonality index of a pitch (octave&gt;fifth&gt;major third etc.) the more likely it will occur on a strong beat. With a zero harmoniclarity value all pitches have the same probability.
<div></div>
<div><strong>Meter</strong></div>
<div>The basic.meters.txt contains the stratifications of a meter which is either multiplicative or additive. Strata only consist of prime number divisors, usually 2 and 3. A 4 meter will be represented as 2 2.</div>
<div>
<blockquote>
2 2 2<div>
2 2 3<div>
3 2 3<div>
3 3 2<div>
3 3 3<div>
2 2 2 2<div>
2 2 2 3<div>
</blockquote>
Besides using 5, 7 or higher prime numbers, additive meters can also be represented by twos and threes combined by a plus sign, such as 2+3 or 3+2+2.

You can create and load your own meter sets which will be displayed in the DJster meter menu.

Scales and meters are located in Programs&gt;Cycling '74 (Windows) or Applications (OS X)&gt;Max6&gt;patches&gt;DJster+&gt;DJster&gt;Lib&gt;Scales and Meters

Note that starting with DJster v. 2.0 transport, tempo and time signature are automatically linked to Ableton Live's Play/Stop Button, Tempo and Time Signature settings for better integration and synchronization. Meter from now on refers to the subdivision of a beat defined by Time Signature Denominator.
<div><strong>Mode</strong></div>
<div>DJster runs in two modes:</div>
<div>
<ol>
	<li>a <em>key</em> mode with pitches snapping to the black and white key grid</li>
	<li>a <em>cent</em> mode in which parameters are set in cent precision.</li>
</ol>
<div><strong>Output</strong></div>
<div>DJster has two output modes:</div>
<div>
<ol>
	<li>a <em>MIDI</em> mode with pitches being sent to generic Live instruments for (non-microtonal/chromatic) playback</li>
	<li>a <em>OSC</em> mode which allows pitches to be played back in cent precision.
This requires a device or program listening locally on ports 11100 plus track number, e.g. 11104 for track no. 4. LiveScore playback devices such as LiveScore Fluidsynth2 or LiveScore Sampler automatically receive the note streams when dropped inside the same track</li>
</ol>
<strong>Other parameters</strong>
For all other parameters please refer to Clarence Barlow's own documentation available at  <a href="http://www.musikwissenschaft.uni-mainz.de/Autobusk/">http://www.musikwissenschaft.uni-mainz.de/Autobusk/</a>.

<strong>Playback</strong>
Two playback devices are included from the <a href="http://www.computermusicnotation.com" target="_blank">LiveScore</a> installation:
<ul>
	<li>LiveScore Fluidsynth2</li>
	<li>LiveScore Sampler</li>
</ul>
LiveScore Fluidsynth2 opens most SoundFont 2 (.sf2) files (check for compatibility with your platform first), while LiveScore Sampler allowing you to create and use your own banks.  All banks must be in the Max search path to be accessible within Ableton Live. More information can be found <a href="http://www.computermusicnotation.com/?page_id=291" target="_blank">here</a>.

</div>
</div>
</div>
</div>
