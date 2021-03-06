* Project summary 
** Day-to-day analysis log
This project is focusing upon applying current models for AGN to
BHXRBs. The progress being made is noted below, with the most recent
comments at the top.
 - 22.02.17: HB and RW worked on completing coherence analysis with
   various segment numbers and working on understanding coherence. We
   also worked on setting up Github. This should now be on Github.
 - 21.02.17: Some of the files made are large so we've improved the
   run script to delete them once they don't need to be used anymore.
   The website now has images too! VZ improved the Excel file used to
   make the .fits files, although this could be turned into a Python
   script if necessary. Need to ask AY: Where to target the 60 cp
   project, now we have done the Epitropakis and coherence so quickly.
   What should the focus be of our writeups? Coherence fitting to an
   equation? Paper or OpenCL? Should we run the table model? Lag energy?
 - 20.02.17: HB and RW worked on improving the segment analysis.
 - 18.02.17: HB completed the preliminary analysis for 060, 065 and
   020...201 observations. This included lag and coherence plots for
   all with relevant `max frequency' and `max coherence' lines on
   them. The coherence for all of those combinations has also been
   found and shown in latest analysis results. This needs to be done
   for both the 020...301 observations (long and short) then we should
   discuss the physical meaning. Model fitting has been improved and
   will fit to data, provided the black hole mass is 10^{2.5}, which
   is about an order of magnitude too high
 - 17.02.17: HB discussed with AY how valid it was to combine all the
   observations of GX339-4 when using the segmentation analysis. This
   should be fine and could possibly be used later to determine
   exactly what the source was doing in the different flux states
   (this depends on the coherence of the source i.e. how consistent
   the difference in phase angle was, so far it looks promising!) The
   model unfortunately did not fit well. We should discuss this and
   how to use the coherence analysis in further meetings. HB produced
   coherence and lag freq according to AE16 for all bar the 020...301
   observation. The others all require minor refining after we have
   discussed with AY. The combined observation has been included in
   latest analysis.
 - 16.02.17: HB, RW and VZ met to discuss how we could improve the
   coherence and time lags. The Epitropakis time lag method now shows
   good comparisons to the 'normal' method (although it has a few
   negative lags above 1 Hz). The coherence is currently on 1
   constantly but we are running analysis for for the 065... and
   020..201. Combinations of this may give a better coherence plot.
 - 15.02.17: HB and RW met up to look at coherence. We developed the
   python script and updated Steff's postproc script. This is quite a
   complex/ lengthy process with many input and output files. See the
   060 coherence analysis example for a description and the scripts
   for further comments. We ran the 060 fine but we were unable to
   plot coherence effectively, possibly need more segment numbers?
 - 14.02.17: AY, HB, RW, VZ Skype meeting with Poemwai. We discussed
   generally the project and just need to fit the model really. We
   will work on how to do coherence now. We found that coherence was
   going to take much longer than expected. We can also use slightly
   different parameters than initially expected (smaller than 20ks
   bins) so we will have many more segments. HB has begun writing a
   small python script that would do this.
 - 7.02.17: HB ran the analysis of the 060... obs with a 0.01 bin size
   instead of 0.06 to ensure all obs were consistent. We also need to
   check why the combined obs has two timing_evts files (U002 and U003)
 - 4.02.17: RW worked on going through the website and picking up
   inconsistencies which will need to be ironed out.
 - 3.02.17: AY, PC, OD, HB meeting. AY will look at the code, but in
   principle the binary should work. PC thinks it should work, if the
   shifting in frequency and scaling is correct. Might need a
   truncated radius. Possibly the freq grid needs changing. We may
   also have problems interpreting, as the thermal lag might be
   different (also don't have a truncated radius, assumes maximally
   spinning). Possibly look at coding up a truncation radius, PC. We
   should double check by comparing to an AGN. SO and HB worked on
   improving the fitting script, line drawing and speeding up making
   the .fits files. AY will get the 2 blobs model working so we can do
   fitting GX339-4 lag fitting. HB, RW, and VZ need to look at
   coherence in the meantime. HB is trying to get the website online
   so it is less laggy and can be used to display results more easily.
   VZ has begun her writeup as the main result will likely be the
   lag-freq plots. If they fit well this may be published.
   Lag-energies are less likely to fit well but could still be done as
   it would be interesting to see why. AY suggested a RAS conference
   we could go to on 10.02.16 on general X-Ray astronomy.
 - 2.02.17: AY agrees it could be a problem with the model that can't
   fit properly. We will meet 3.02.17 to discuss with Poemwai at 9am
   and 1pm with AY further. Spherical corona looks like it might take
   a while to do so we should focus on the two blobs model, and try to
   interpret the results.
 - 1.02.17: VZ has also come across the same chi-squared fitting
   problem as HB. SO is going to look at it. HB has emailed AY to see
   if this is expected. Currently waiting to hear about new model.
 - 31.01.17:  HB has apparently fixed the problem by running a
   later version of python (thanks to R. Morris). There is now a problem in the
   setup_table.sl script (missing scale_tlag.sl) which HB has emailed
   Steff about. With Steff's assistance, HB has run the table model
   however the plots are far away from what is expected. Possibly the
   model just won't work with the binary data.
 - 30.01.17: VZ ran the merger analysis and produced similar
   lag-freqency plots to HB. VZ has also been held up however by the
   astropy problem.
 - 27.01.17: HB, RW, VZ meeting. VZ repeated analysis to try and
   create the lag-eng plots. RW spotted a bug in his lag-eng code,
   some errors on the website and has also set his isis lag-eng code
   to run again. HB has laid foundations for the table model analysis,
   and (with RW) generated the relevant analysis scripts for the 2004
   data observations, however HB is having problems installing
   'astropy' - a python package.
 - 26.01.17: Continued analysis into how to merge the observations.
   Steff has suggested we try a script he wrote to combine the
   datasets. This appears to have worked well and is recorded in the
   notes. An overlay of all lag-freq plots has been produced (very
   roughly) and appears to match with the theory well!. The normal lag-freq analysis for ...201 ran successfully but I've not
   looked at the data output in detail, but it may be interesting to
   compare the benefits of combining consecutive orbits.
 - 25.01.17: Continued analysis into how to merge the observations. A new
   merge attempt was tried but resulted in an error message. (Happy
   Birthday, Ralph!)
 - 24.01.17: Harry looked into how to merge files, see [[http://www.mpe.mpg.de/xray/wave/xmm/cookbook/preparation/merged_events.php][here]] for
   instructions. isis was found to hang.
 - 23.01.16: Meeting with Andy, Ralph and Harry. Discussed 60cp
   extension. Agreed in general we need to be working on lag-frequency
   of GX339-4. Then we'll fit Poemwai's spherical model. Once we've
   done this we can begin writing up and focus on 'extensions'.
 - 15.12.16: Christmas plan. We need to consider where to go
   (Epitropakis, Spherical, 2 blobs, RXTE). Andy will talk to Poemwai
   about which is best.
 - 8.12.16: Updated the website to now include all analysis in one
   place. Lag-energy image uploaded. Emailed for website access as the
   current means to view the html is laggy.
 - 06.12.16: Weekly group meeting. During an especially delicious
   meeting we discussed issues with timebinsize and altered the
   lag-energy scripts to reflect the difference with binaries. We aim
   to complete the low luminosity observation analysis from DM15b by
   the end of this term. Our long term goal will be to fit the spherical
   corona model to this (Ref needed).
   In the afternoon we managed to recreate the lag-frequency plot for
   the high luminosity observation in DM15a. The lag-energy scripts
   are currently running (taking approx. 6 hrs)
 - 02.12.16: Met up to look at the code again. Using a
  timebinsize=0.001 as described in DM15b caused an error (**
  epiclccorr: error (BinSizeTooSmall), Light curve bin size smaller
  than frame time). We will now be using a timebinsize=0.01 as the
   later paper refers to this instead.
 - 29.11.16: Code brought into Emacs and .html made. Issues with
   producing the lag-frequency plots for GX339-4 obsid:0605610201 have
   slowed progress. We are currently unsure how to produce the plots
   above 1 Hz. The analysis follows currently that from 2 papers, both
   published De Marco in 2015 (DM15a and DM15b).

References
DM15a - B. De Marco, G. Ponti, T. Muñoz-Darias, and K. Nandra, “The evolution of the disc variability along the hard state of the black hole transient GX 339-4,” Mon. Not. R. Astron. Soc., vol. 454, no. 3, pp. 2360–2371, 2015.

DM15b - B. De Marco, G. Ponti, T. Muñoz-Darias, and K. Nandra,
“Tracing the Reverberation Lag in the Hard State of Black Hole X-Ray
Binaries,” Astrophys. J., vol. 814, no. 1, p. 50, 2015.

** Progress
*** Current tasks to complete
 - (complete) Repeat all isis lag-freq scripts with identical plotting parameters
   and see if an 'overlay' is possible
 - (in progress) Test spherical corona fit to an AGN to check we're doing the fitting
   mechanics properly (awaiting model from Poemwai)
 - (complete) Check if RA has been accepted.
 - (in progress) Attempt to fit the model the draft 2 blobs model
 - Produce Lag-energy for the last 2 2009 observations.
 - Backup all data.

*** 60cp Extension
 - Coherence and Epitropakis methods.
 - Coherence overlay plots.
 - Coherence for the 020...301 observation.
 - List below describes what we need to be working on.
   Looking at OpenCL additon to Poemwai's code.
   decompising into a basis also to define polarisation.
 - Update 2 blobs model to add Xlliver model and truncation radius.
 - Move website to Gitpages



AE16 - A. Epitropakis and I. E. Papadakis, “Statistical properties of Fourier-based time-lag estimates,” Astron. Astrophys., vol. 591, p. A113, 2016.

** Latest Analysis Results

We have currently been working on the Epitropakis methods. See the
'Epitropakis Methods' sections in the individual observation sections
for the lag and coherence plots. The observation segments have been
combined in various ways, and these are shown below. The scripts to do
this can be found in =/data/cluster/XRayReverb2016/HarryData/GX339-4=,
however, look very similar to the ones shown in the separate
observation files.

#+CAPTION: Latest Analysis: All observations combined Lag-Frequency plot using E16 analysis.
file:./CombinedAllLagFrequency.gif

#+CAPTION: Latest Analysis: All observations combined  Coherence-Frequency plot.
[[file:./CombinedAllCoherenceFrequency.gif]]

#+CAPTION: Latest Analysis: Combined 060, 065 and 020...201 Lag-Frequency plot.
file:./Combined060065022LagFrequency.gif

#+CAPTION: Latest Analysis: Combined 060, 065 and 020...201 Coherence-Frequency plot.
[[file:./Combined060065022CoherenceFrequency.gif]]

#+CAPTION: Latest Analysis: Combined 060, 020...201  Lag-Frequency plot.
[[file:./Combined060022LagFrequency.gif]]

#+CAPTION: Latest Analysis: Combined 060 and 020...201 Coherence-Frequency plot.
[[file:./Combined060022CoherenceFrequency.gif]]

#+CAPTION: Latest Analysis: Combined 065, 020...201  Lag-Frequency plot.
[[file:./Combined065022LagFrequency.gif]]

#+CAPTION: Latest Analysis: Combined 065 and 020...201 Coherence-Frequency plot.
[[file:./Combined065022CoherenceFrequency.gif]]

#+CAPTION: Latest Analysis: Combined 060, 065  Lag-Frequency plot.
[[file:./Combined06LagFrequency.gif]]

#+CAPTION: Latest Analysis: Combined 060 and 065 Coherence-Frequency plot.
[[file:./Combined06CoherenceFrequency.gif]]


Archive:

#+CAPTION: Latest Analysis: An overlay plot with our lag-frequency analysis of GX339-4 and that from DM15b.
[[file:./LagFreq_Overlay.png]]


#+CAPTION: Latest Analysis: The lag-frequency plot using timebinsize=0.01 s for the highest luminosity observation in DM15a. We believe this is a clear copy of the De Marco Analysis.
[[file:./0654130401/PROC/lagfreq.gif]]

#+CAPTION: Latest Analysis: The lag-frequency plot using timebinsize=0.01 s for the intermediate luminosity observation in DM15a. We believe this is a clear copy of the De Marco Analysis.
[[file:./0204730201-0204730301-Merger/PROC/lagfreq_comb.gif]]

#+CAPTION: Latest Analysis: The lag-frequency plot using timebinsize=0.01 s for the lowest luminosity observation in DM15a. We believe this is a clear copy of the De Marco Analysis.
[[file:./0605610201/PROC/lagfreq.gif]]

#+CAPTION: Latest Analysis: 0605610201 lag-energy plot.
[[file:./0605610201/PROC/lagen_0.8-2Hz.gif]]

#+CAPTION: Latest Analysis: 0654130401 lag-energy plot.
[[file:./0654130401/PROC/lagen_0.8-2Hz.gif]]

** About

This website records the analysis if GX339-4 as part of a 2016/17
masters project. Should you find any errors, please contact the website administrator
at =hb13486@bris.ac.uk=. Sections marked with a * are extension
projects worked on as part of a 60cp project.

The Collaboration:

 - 2016 MSci Students: Harry Birch, Ralph Wellington and Viktoria Zekoll
 - Supervisor: Dr. Andy Young
 - Collaborators: Steff O'Donnell and Dr. Poemwai Chainakun

Find us on GitHub at: [[https://github.com/hpbirch]] and [[https://github.com/RCWellington]]

* GX339-4
** 0605610201
#+INCLUDE: "/data/cluster/XRayReverb2016/HarryData/GX339-4/0605610201/PROC/TrialGXAnalysis2.org"
** 0654130401
#+INCLUDE: "/data/cluster/XRayReverb2016/HarryData/GX339-4/0654130401/PROC/TrialGXAnalysis3.org"
** 0204730201
#+INCLUDE: "/data/cluster/XRayReverb2016/HarryData/GX339-4/0204730201/PROC/0204730201Analysis.org"

** 0204730301 (U002)
The 0204730301 observation was split into 2 parts. This is the longer
U002 analysis.
#+INCLUDE:"/data/cluster/XRayReverb2016/HarryData/GX339-4/02047303012/PROC/02047303012Analysis.org"

** 0204730301 (U003)
The 0204730301 observation was split into 2 parts. This is the shorter
U003 analysis.
#+INCLUDE:"/data/cluster/XRayReverb2016/HarryData/GX339-4/02047303013/PROC/02047303013Analysis.org"

** 0204730201-024730301 Merger Analysis
#+INCLUDE: "/data/cluster/XRayReverb2016/HarryData/GX339-4/0204730201-0204730301-Merger/PROC/0204730201-0204730201-PostMergerAnalysis.org"







** COMMENT Archive Analysis and code snippets

85 - all
146 -02021
1430 - 020065022
9 -  mode fitting
10 - all 2004 observations normal analysis


#+BEGIN_SRC elisp
   (url-copy-file "https://fb-s-d-a.akamaihd.net/h-ak-xpf1/v/t35.0-12/16326237_10209184188334282_886787265_o.png?oh=91c4ddc7ffce4bd228164ca0d3fce7fc&oe=588C3664&__gda__=1485584870_2bbe04751e63d48491c7f8907351a1e1" (expand-file-name "./LagFreq_Overlay.png") 1)
#+END_SRC


*** Initial Processing

#+BEGIN_SRC sh
echo '\n\n\n Initial SAS setup, general for all files. Run in a suitable folder after replacing the OBSID'

mkdir OBSID
cd OBSID
mkdir ODF PROC
cd ODF
echo '\n\nDOWNLOAD TAR FILE...'
curl -o 0654130401.tar "http://nxsa.esac.esa.int/nxsa-sl/servlet/data-action-aio?obsno=0654130401&level=ODF"
tar -zxvf *.tar
tar -xvf *.TAR

echo '\n\n\n file unpacked. Setup SAS'

heainit
setsas
setenv SAS_CCFPATH /usr/local/XMM/ccf/
setenv SAS_ODF $PWD
cifbuild
setenv SAS_CCF ccf.cif
odfingest
setenv SAS_ODF $PWD/*SUM.SAS
cp ccf.cif ../PROC
cp *SUM.SAS ../PROC
cd ../PROC

echo '\n\n\n MOVED TO PROC FOLDER. INITIALISING WORK'

epproc randomizetime=no randomizeposition=no randomizeenergy=no

echo '\n\n\nScript to process ODF data\n\n\n'
cp *TimingEvts.ds PN.fits

echo 'Create a light curve.'
evselect table=PN.fits withrateset=yes rateset=PN_flares_lc.fits maketimecolumn=yes timebinsize=0.001 makeratecolumn=yes expression='#XMMEA_EP && (PI>10000&&PI<12000) && (PATTERN==0)'
dsplot table=PN_flares_lc.fits x=TIME y=RATE &


#+END_SRC

At this point flares must be removed if they exist.
In this instance there were no flares so they were not removed.
*** Flare removal

#+BEGIN_SRC sh
echo '\n no flares removed'
cp PN.fits EPICclean.fits

echo '\n\n\n MAKE IMAGE...'
evselect table=EPICclean.fits withimageset=yes imageset=EPICclean_image.fits xcolumn=RAWX ycolumn=RAWY imagebinning=binSize ximagebinsize=1 yimagebinsize=1
ds9 EPICclean_image.fits &
echo '\nImage created. Please note down a source and background range of pixels.'

#+END_SRC

#+CAPTION: 2D Image of the source in timing mode. The central region was extracted using the 'projection' tool in ds9 (hence the green line).
#+LABEL: image
[[file:2DImage.png]]
At this point the source and background 'RAWX' values were found using
Fig. [[image]]
replaced in the following text.

*** Extract Source and Background Region

#+BEGIN_SRC sh
echo '\n\nSoft Filter\n'
evselect table=EPICclean.fits withfilteredset=yes filteredset=PN_time_soft.fits filtertype=expression expression='(FLAG==0)&&(PATTERN<=4)&&(PI in [500:1500])&&#XMMEA_EP' keepfilteroutput=yes updateexposure=yes filterexposure=yes

echo '\n\nHard Filter\n'
evselect table=EPICclean.fits withfilteredset=yes filteredset=PN_time_hard.fits filtertype=expression expression='(FLAG==0)&&(PATTERN<=4)&&(PI in [2000:9000])&&#XMMEA_EP' keepfilteroutput=yes updateexposure=yes filterexposure=yes

echo '\n\n Extract src and bg\n\n'

echo 'Extract Source from Soft Photons'
evselect table=PN_time_soft.fits withfilteredset=yes filteredset=PN_time_soft_src.fits filtertype=expression expression='RAWX in [31:45]' keepfilteroutput=yes updateexposure=yes filterexposure=yes

echo 'Extract Source from Hard Photons'
evselect table=PN_time_hard.fits withfilteredset=yes filteredset=PN_time_hard_src.fits filtertype=expression expression='RAWX in [31:45]' keepfilteroutput=yes updateexposure=yes filterexposure=yes

echo 'Extract Background from Soft Photons'
evselect table=PN_time_soft.fits withfilteredset=yes filteredset=PN_time_soft_bkg.fits filtertype=expression expression='RAWX in [3:5]' keepfilteroutput=yes updateexposure=yes filterexposure=yes

echo 'Extract Background from Hard Photons'
evselect table=PN_time_hard.fits withfilteredset=yes filteredset=PN_time_hard_bkg.fits filtertype=expression expression='RAWX in [3:5]' keepfilteroutput=yes updateexposure=yes filterexposure=yes

#+END_SRC

*** Make Light Curves

Note the time bin size here.

#+BEGIN_SRC sh
echo '\n\nCreate Lightcurve from source\n'

echo '\n\nCreate lc from soft photons\n'
evselect table=PN_time_soft_src.fits withrateset=yes rateset=PN_time_soft_src_lc.fits maketimecolumn=yes timecolumn=TIME timebinsize=0.001 makeratecolumn=yes

echo '\n\nCreate lc from hard photons\n'
evselect table=PN_time_hard_src.fits withrateset=yes rateset=PN_time_hard_src_lc.fits maketimecolumn=yes timecolumn=TIME timebinsize=0.001 makeratecolumn=yes

echo '\n\nCreate lc from Background\n'

echo '\n\nCreate lc from soft photons\n'
evselect table=PN_time_soft_bkg.fits withrateset=yes rateset=PN_time_soft_bkg_lc.fits maketimecolumn=yes timecolumn=TIME timebinsize=0.001 makeratecolumn=yes

echo '\n\nCreate lc from hard photons\n'
evselect table=PN_time_hard_bkg.fits withrateset=yes rateset=PN_time_hard_bkg_lc.fits maketimecolumn=yes timecolumn=TIME timebinsize=0.001 makeratecolumn=yes

echo '\n\nCreate Background Subtracted Light Curve\n'

echo '\n\nFrom soft photons (10 mins)\n'
epiclccorr srctslist=PN_time_soft_src_lc.fits eventlist=EPICclean.fits outset=PN_time_soft_lccorr.fits bkgtslist=PN_time_soft_bkg_lc.fits withbkgset=yes applyabsolutecorrections=yes

echo '\n\nFrom hard photons (10 mins)\n'
epiclccorr srctslist=PN_time_hard_src_lc.fits eventlist=EPICclean.fits outset=PN_time_hard_lccorr.fits bkgtslist=PN_time_hard_bkg_lc.fits withbkgset=yes applyabsolutecorrections=yes

echo 'Display the lightcurve'

dsplot table=PN_time_soft_lccorr.fits x=TIME y=RATE &
dsplot table=PN_time_hard_lccorr.fits x=TIME y=RATE &

echo 'Note that the above lightcurves can be chopped with the evselect timemin and timemax command'

#+END_SRC

*** Produce Lag-Frequency Plots

Begin by downloading a template
#+BEGIN_SRC sh
echo("\n\n\nProduce lagfreq script\n\n\n")
cp /data/cluster/XRayReverb2016/SharedData/UpdatedAnalysisScripts/isis_lagfreq_script.sl .
emacs -nw isis_lagfreq_script.sl
#+END_SRC

Edit this file accordingly (update OBSID and frequency ranges if
necessary). Then run the file analysis in isis. The one used in this
case is shown in the following in a separate section [[Lag-Frequency Script][here]].

#+BEGIN_SRC sh
isis
() = evalfile("isis_lagfreq_script.sl");
#+END_SRC

The output from this is shown in Figure [[LagFreq]].
 #+BEGIN_SRC elisp
    (url-copy-file "https://scontent.xx.fbcdn.net/v/t34.0-12/15226442_10208645591709703_2038569113_n.png?oh=d6a5ba34a3ace2cea0337429e26ec02c&oe=584039E3" (expand-file-name "./LagFreq.png") 1)
 #+END_SRC

 #+RESULTS:
 #+begin_example
 t
#+end_example

#+CAPTION: The problem graph
#+LABEL: LagFreq
[[file:LagFreq.png]]

*** Produce Lag-Energy Plots

Once the lag-freq plots have been generated, the lag-energy plots can
also be made. This is done by initially copying an template and
editing suitably.
#+BEGIN_SRC sh
echo '\n\n\nRun LagEng Processing Scripts\n\n\n'
cp /data/cluster/XRayReverb2016/SharedData/UpdatedAnalysisScripts/sas_lagen_script1.py .
cp /data/cluster/XRayReverb2016/SharedData/UpdatedAnalysisScripts/isis_lagen_lf_script.sl .
cp /data/cluster/XRayReverb2016/SharedData/UpdatedAnalysisScripts/isis_lagen_hf_script.sl .
#+END_SRC

Once done, the python script will run. This can take many hours so to
avoid it being interrupted the 'screen' tool has been used. Once a new
'screen' has been entered, the python script can be run (Note: the
environments variables may need to be reset.  Once the script is
running, pressing =Ctrl + A   d= will
detach the screen. To bring it back up, enter =screen
-r= to the command line. The output will be in the usual place.

#+BEGIN_SRC sh
echo '\n\n Run the Lag_energy scripts.\nThis step will take a long time.\nYou can close the ssh.\n\n\n'
screen
python sas_lagen_script1.py
#+END_SRC
Once complete the below can be run to generate the lag-energy plots
for high and low frequencies.
#+BEGIN_SRC sh
isis
() = evalfile("isis_lagen_lf_script.sl");
() = evalfile("isis_lagen_hf_script.sl");

echo 'Script is complete'
#+END_SRC

*** Produce a spectrum - UNDER CONSTRUCTION
**** Initial Processing
Begin by refiltering the curve.

#+BEGIN_SRC sh
echo '\n\n\n FILTER CURVE...\n\n'
evselect table=EPICclean.fits withfilteredset=yes expression='(FLAG==0) && (PATTERN <= 4)&&(PI in [200:15000])&&#XMMEA_EP' filteredset=pn_filt.fits filtertype=expression keepfilteroutput=yes updateexposure=yes filterexposure=yes
#+END_SRC

At this point the image and light curves can be looked at using. If
the previous sections have not been analysed already, this will need
to be done to determine the source and background regions.

#+BEGIN_SRC sh
evselect table=pn_filt.fits withimageset=yes imageset=image.fits xcolumn=RAWX ycolumn=RAWY imagebinning=binSize ximagebinsize=1 yimagebinsize=0.001
ds9 image.fits &

echo '\n\n\n CREATE AND DISPLAY LIGHT CURVE...\n\n'
evselect table=pn.fits withrateset=yes rateset=pn_ltcrv.fits maketimecolumn=yes timecolumn=TIME timebinsize=0.001 makeratecolumn=yes
fv pn_ltcrv.fits &
#+END_SRC

#+BEGIN_SRC sh
echo '\n\n\nEXTRACT SOURCE AND BACKGROUND'
evselect table=pn_filt.fits withimageset=yes imageset=image.fits xcolumn=RAWX ycolumn=RAWY imagebinning=binSize ximagebinsize=1 yimagebinsize=1 expression='(FLAG==0) && (PI in [500:15000])'

evselect table=pn_filt.fits spectrumset=source_pi_WithBore.fits energycolumn=PI spectralbinsize=5 specchannelmin=0 specchannelmax=20479 filteredset=pn_filt_source_WithBore.fits expression='(FLAG==0) && (PI in [500:15000]) && (RAWX in [27:47])'

evselect table=pn_filt.fits withspectrumset=yes spectrumset=bkg_pi.fits energycolumn=PI spectralbinsize=5 withspecranges=yes specchannelmin=0 expression='(FLAG==0) && (PI in [500:15000]) && (RAWX in [3:5])' specchannelmax=20479 withfilteredset=y filteredset=pn_filt_bkg.fits

epatplot set=pn_filt_source_WithBore.fits plotfile=pn_epat.ps useplotfile=yes withbackgroundset=yes backgroundset=pn_filt_bkg.fits
gv pn_epat.ps &
#+END_SRC

At this point, pile up must be checked. The last command in the
previous section is used to do this. In the case the doubles are >1
and singles <1 then the detector has pileup. This can be corrected for
using the following method where a region of the source is removed.


**** Case 1 - spectrum is piled up
The code below extracts a region of the source. It then checks for
pileup this process must be repeated until pileup is removed.

#+BEGIN_SRC sh
evselect table=pn_filt.fits withspectrumset=yes spectrumset=source_pi_NoBore.fits energycolumn=PI spectralbinsize=5 withspecranges=yes specchannelmin=0 specchannelmax=20479 expression='(FLAG ==0)&&(PI in [500:15000])&&(RAWX in [27:47])&&!(RAWX in [30:44])' withfilteredset=yes filteredset=pn_filt_source_NoBore.fits
epatplot set=pn_filt_source_NoBore.fits plotfile=pn_epat.ps useplotfile=yes withbackgroundset=yes backgroundset=pn_filt_bkg.fits
gv pn_epat.ps &
echo('\nCheck for pileup\n\n')
#+END_SRC

Once this correction has been made, then the arf and rmf files may be
made, as shown below.

#+BEGIN_SRC sh
evselect table=pn_filt.fits withspectrumset=yes spectrumset=source_pi_Excised.fits energycolumn=PI spectralbinsize=5 withspecranges=yes specchannelmin=0 specchannelmax=20479 expression='(FLAG ==0)&&(PI in [500:15000])&&(RAWX in [27:47])&&!(RAWX in [29:45])' withfilteredset=yes filteredset=pn_filt_source_Excised.fits

echo '\n\n\nDETERMINE SPECTRAL EXTRACTION AREA'
backscale spectrumset=source_pi_NoBore.fits badpixlocation=pn_filt.fits
backscale spectrumset=bkg_pi.fits badpixlocation=pn_filt.fits

echo '\n\n\nMAKE RMF AND ARF FILES. (Takes a long time!)'
rmfgen rmfset=source_rmf_NoBore.fits spectrumset=source_pi_NoBore.fits

arfgen arfset=source_arf_WithBore.fits spectrumset=source_pi_WithBore.fits detmaptype=psf
arfgen arfset=source_arf_Excised.fits spectrumset=source_pi_Excised.fits detmaptype=psf

addarf "source_arf_WithBore.fits source_arf_Excised.fits" "1.0 -1.0" source_arf_NoBore.fits
echo("\n\ndone\n\n")
#+END_SRC



**** Case 2 - spectrum is not piled up

In this instance, simply run the following to generate the rmf and arf files

#+BEGIN_SRC sh
echo '\n\n\nDETERMINE SPECTRAL EXTRACTION AREA'
backscale spectrumset=source_pi_NoBore.fits badpixlocation=pn_filt.fits
backscale spectrumset=bkg_pi.fits badpixlocation=pn_filt.fits
echo("\n\nproduce RMF and ARF files\n\n")
rmfgen rmfset=source_pi_WithBore_rmf.fits spectrumset=source_pi_WithBore.fits
arfgen arfset=source_pi_WithBore_arf.fits spectrumset=source_pi_WithBore.fits withrmfset=yes rmfset=source_pi_WithBore_rmf.fits withbadpixcorr=yes badpixlocation=pn_filt.fits

#+END_SRC

**** Make Group Spectral Files

If there was pileup the following is run. Note this should be entered
line by line not in one go to avoid clashes.

#+BEGIN_SRC sh
grppha
source_pi_NoBore.fits      ! input spectrum file name
spectrum_pi_grp.fits  ! output grouped spectrum
bkg_pi.fits           ! include the background spectrum
source_rmf_NoBore.fits         ! include the RMF
source_arf_NoBore6.fits          ! include the ARF
group min 25                         ! group the data by 25 counts/bin
exit
#+END_SRC

If there was no pileup the following is used.
#+BEGIN_SRC sh
grppha
source_pi_WithBore.fits      ! input spectrum file name
spectrum_pi_grp.fits  ! output grouped spectrum
bkg_pi.fits           ! include the background spectrum
source_rmf_WithBore.fits         ! include the RMF
source_arf_WithBore.fits          ! include the ARF
group min 25                         ! group the data by 25 counts/bin
exit
#+END_SRC

**** Plot the spectrum
Plot as below. The spectrum is compared to a simple powerlaw model.

With pileup:
#+BEGIN_SRC sh
isis
d=load_data("spectrum_pi_grp.fits");
r=load_rmf("source_rmf_NoBore.fits");
a=load_arf("source_arf_NoBore.fits");
assign_rsp(a,r,d);
define_back(d, "bkg_pi.fits");
fit_fun("powerlaw");
rebin_data(1, 10);
xnotice_en(d, 1, 10.0);
set_par(2, 2.0);
fancy_plot_unit(“keV”);
()=fit_counts;
popt.xrange = [1, 10.0];
popt.yrange = [1.0e-6, 1.0, -10.0, 10.0];
popt.dsym = 1;
popt.res = 1;
xlog;
ylog;
title ("GX339-4 OBSID Spectrum");
plot_data(d, popt; dsym=1);
#+END_SRC

or in the case of no pileup
#+BEGIN_SRC sh
echo '\n\n\n PLOT SPECTRUM \n\n\n'
isis
d=load_data("spectrum_pi_grp.fits");
r=load_rmf("source_rmf_WithBore.fits");
a=load_arf("source_arf_WithBore.fits");
assign_rsp(a,r,d);
define_back(d, "bkg_pi.fits");
fit_fun("powerlaw");
rebin_data(1, 10);
xnotice_en(d, 1, 10.0);
set_par(2, 2.0);
fancy_plot_unit(“keV”);
()=fit_counts;
popt.xrange = [1, 10.0];
popt.yrange = [1.0e-6, 1.0, -10.0, 10.0];
popt.dsym = 1;
popt.res = 1;
xlog;
ylog;
title ("GX339-4 OBSID Spectrum");
plot_data(d, popt; dsym=1);
#+END_SRC

*** Lag-Frequency Script

#+BEGIN_SRC

%declare observation ID's
variable obs_id = ["0605610201"];


variable i;
variable j;
variable k;

%declare frequency bins
variable n_bins =21;
variable df_f = 0.5/1.1; %Possibly change bin size to be bigger to exactly emulate DeMarco2015 results.
variable lo = Double_Type[n_bins];
variable hi = Double_Type[n_bins];
lo[0]=0.005;
hi[0]=(lo[0] + lo[0]*df_f);

for(i=1;i<n_bins;i++){
    lo[i]=hi[i-1];
    hi[i]=lo[i]+lo[i]*df_f;
 }

%logarithmic frequency bin centre
variable rb_freq = 10^(0.5*(log10(lo)+log10(hi)));

%declare arrays
variable rb_n = Integer_Type[n_bins];
variable lag = Double_Type[n_bins];
variable g_a_real = Double_Type[n_bins];
variable g_a_imag = Double_Type[n_bins];
variable g_a = Double_Type[n_bins];
variable g_b = Double_Type[n_bins];
variable g_c = Double_Type[n_bins];
variable g = Double_Type[n_bins];
variable delta_phi = Double_Type[n_bins];
variable delta_lag = Double_Type[n_bins];

%loop through observarions
for(k=0; k<length(obs_id); k++){


%Read data:
variable lc_soft = fits_read_table("PN_time_soft_lccorr.fits");
variable lc_hard = fits_read_table("PN_time_hard_lccorr.fits");

%exclude non-numbers:
variable ix_soft = where(not isnan(lc_soft.rate));
variable ix_hard = where(not isnan(lc_hard.rate));

%Pass to new variables:
variable time_soft = lc_soft.time[ix_soft];
variable time_hard = lc_hard.time[ix_hard];
variable rate_soft = lc_soft.rate[ix_soft];
variable rate_hard = lc_hard.rate[ix_hard];
variable error_soft = lc_soft.error[ix_soft];
variable error_hard = lc_hard.error[ix_hard];

% Compute soft dft:
variable dft_soft = fft(rate_soft,-1);
variable freq = [[0:length(dft_soft)-1]]/(double(length(dft_soft))*(time_soft[1]-time_soft[0]));
variable dft_real_soft = Real(dft_soft[[0:length(freq)-1]]);
variable dft_imag_soft = Imag(dft_soft[[0:length(freq)-1]]);

% Compute hard dft:
variable dft_hard = fft(rate_hard,-1);
variable dft_real_hard = Real(dft_hard[[0:length(freq)-1]]);
variable dft_imag_hard = Imag(dft_hard[[0:length(freq)-1]]);

%Calculate and sum CPS for each frequency bin in each observation.
for(i=0; i< n_bins; i++)
{
        for (j=0; j<length(freq); j++)
        {
                if(freq[j] > lo[i] && freq[j] <= hi[i])
                {
                        g_a_real[i] += abs(dft_real_soft[j]*dft_real_hard[j] + dft_imag_soft[j]*dft_imag_hard[j]);
                        g_a_imag[i] += dft_imag_soft[j]*dft_real_hard[j] - dft_real_soft[j]*dft_imag_hard[j];
                        g_b[i] += dft_real_soft[j]*dft_real_soft[j] + dft_imag_soft[j]*dft_imag_soft[j];
                        g_c[i] += dft_real_hard[j]*dft_real_hard[j] + dft_imag_hard[j]*dft_imag_hard[j];
                        rb_n[i] ++;
                }
        }
}
}

%Plot variables including frequency error bars
variable x = (hi+lo)/2;
variable dxp = hi-x;
variable dxm = x-lo;

%Average CPS in each frequency bin for all observations. Calculate coherence, g[i], for each frequency bin.
for(i=0;i<n_bins;i++)
{
        %Lag error
        g_a[i] = (g_a_real[i]*g_a_real[i] + g_a_imag[i]*g_a_imag[i])/(double(rb_n[i])*double(rb_n[i]));
        g_b[i] /= double(rb_n[i]);
        g_c[i] /= double(rb_n[i]);
        g[i] = g_a[i]/(g_b[i]*g_c[i]);
        delta_phi[i] = sqrt((1.0-g[i])/(2.0*g[i]))/sqrt(double(rb_n[i]));
        delta_lag[i] = delta_phi[i]/(2.0*PI*rb_freq[i]);

        %Lag
        g_a_real[i] /= rb_n[i];
        g_a_imag[i] /= rb_n[i];
        lag[i] = atan2(g_a_imag[i] , g_a_real[i])/(2.0*PI*rb_freq[i]);
}

% Plot results:

%open_plot("lagfreq.gif/gif");

xlog;
ylog;
xlabel("Frequency (Hz)");
ylabel("Time Lag (s)");
title("GX339-4 0605610201 lag-frequency >3e-3 Hz");
connect_points(0);

plotxy(x,dxm,dxp,lag,delta_lag,delta_lag; dcol=1, decol=4,dsym=6, xrange=[3e-3,10], yrange=[0.0001,1]);
_pgmove(-10000,0);
_pgsls(2);
_pgslw(1);
_pgdraw(1,0);

for (i=0; i<length(x); i++) {
  () = printf("%e,%e,%e\n", x[i], lag[i], delta_lag[i]);
}
#+END_SRC
*** Lag-Energy Scripts
**** Setup Script

#+BEGIN_SRC python
#!/usr/bin/env python
import os
i=0
#Enter energy bands here
#band = [300,350,400,500,600,700,800,1000,1300,1600,2000,2400,3000,4000,5000,6000,7000,10000]
#band = [300,400,500,600,800,1000,1300,2000,3000,4000,5000,7000,10000]

band = [400,550,700,900,1100,1400,1700,2000,2400,3200,3600,4000,4400,4700,5200,5600,6000,6700,7300,8100,9000,9600]
number_bands = (len(band)-1)

min1 = '31' #Set source coordinates.
max1 = '45'
minmax1 = '['+min1+':'+max1+']'

min2 = '3' #Set background coordinates.
max2 = '5'
minmax2 = '['+min2+':'+max2+']'

while(i < number_bands):
    os.system("echo 'Running band " + repr(band[i]) + "-" + repr(band[i+1]) + "eV.'")
    #Energy filters
    os.system("evselect table=EPICclean.fits withfilteredset=yes filteredset=PN_time_reference.fits filtertype=expression expression='(FLAG==0)&&(PATTERN<=4)&&(PI in [" + repr(band[0])  + ":" + repr(band[i]) + "],[" + repr(band[i+1]) + ":" + repr(band[number_bands]) + "])&&#XMMEA_EP' keepfilteroutput=yes updateexposure=yes filterexposure=yes &> /dev/null")
    os.system("evselect table=EPICclean.fits withfilteredset=yes filteredset=PN_time_narrow.fits filtertype=expression expression='(FLAG==0)&&(PATTERN<=4)&&(PI in [" +  repr(band[i]) + ":" + repr(band[i+1]) +"])&&#XMMEA_EP' keepfilteroutput=yes updateexposure=yes filterexposure=yes &> /dev/null")
    #Source extraction - NOTE BLANK CIRCLES
    os.system("evselect table=PN_time_reference.fits  withfilteredset=yes filteredset=PN_time_reference_src.fits filtertype=expression expression='RAWX in "+minmax1+"' keepfilteroutput=yes updateexposure=yes filterexposure=yes &> /dev/null")
    os.system("evselect table=PN_time_narrow.fits  withfilteredset=yes filteredset=PN_time_narrow_src.fits filtertype=expression expression='RAWX in "+minmax1+"' keepfilteroutput=yes updateexposure=yes filterexposure=yes &> /dev/null")
    #Background extraction - NOTE BLANK CIRCLES
    os.system("evselect table=PN_time_reference.fits withfilteredset=yes filteredset=PN_time_reference_bkg.fits filtertype=expression expression='RAWX in "+minmax2+"' keepfilteroutput=yes updateexposure=yes filterexposure=yes &> /dev/null")
    os.system("evselect table=PN_time_narrow.fits  withfilteredset=yes filteredset=PN_time_narrow_bkg.fits filtertype=expression expression='RAWX in "+minmax2+"' keepfilteroutput=yes updateexposure=yes filterexposure=yes &> /dev/null")
    #Create light curves
    os.system("evselect table=PN_time_reference_src.fits withrateset=yes rateset=PN_time_reference_src_lc.fits maketimecolumn=yes timecolumn=TIME timebinsize=0.006 makeratecolumn=yes &> /dev/null")
    os.system("evselect table=PN_time_narrow_src.fits withrateset=yes rateset=PN_time_narrow_src_lc.fits maketimecolumn=yes timecolumn=TIME timebinsize=0.006 makeratecolumn=yes &> /dev/null")
    os.system("evselect table=PN_time_reference_bkg.fits withrateset=yes rateset=PN_time_reference_bkg_lc.fits maketimecolumn=yes timecolumn=TIME timebinsize=0.006 makeratecolumn=yes &> /dev/null")
    os.system("evselect table=PN_time_narrow_bkg.fits withrateset=yes rateset=PN_time_narrow_bkg_lc.fits maketimecolumn=yes timecolumn=TIME timebinsize=0.006 makeratecolumn=yes &> /dev/null")
    #Epic light curve correction
    os.system("epiclccorr srctslist=PN_time_reference_src_lc.fits eventlist=EPICclean.fits outset=reference_" + repr(band[i]) + "_" + repr(band[i+1]) +"_lccorr.fits bkgtslist=PN_time_reference_bkg_lc.fits withbkgset=yes applyabsolutecorrections=yes &> /dev/null")
    os.system("epiclccorr srctslist=PN_time_narrow_src_lc.fits eventlist=EPICclean.fits outset=narrow_" + repr(band[i]) + "_" + repr(band[i+1]) + "_lccorr.fits bkgtslist=PN_time_narrow_bkg_lc.fits withbkgset=yes applyabsolutecorrections=yes &> /dev/null")
    i=i+1

#+END_SRC
**** Plotting Script for selecting specific frequencies

#+BEGIN_SRC
%declare observation ID's
variable obs_id = ["0605610201"];

%declare energy band edges
%variable band = [300,350,400,500,600,700,800,1000,1300,1600,2000,2400,3000,4000,5000,6000,7000,10000];

%variable band = [300,400,500,600,800,1000,1300,2000,3000,4000,5000,7000,10000];

variable band = [400,550,700,900,1100,1400,1700,2000,2400,3200,3600,4000,4400,4700,5200,5600,6000,6700,7300,8100,9000,9600];

variable number_bands = length(band)-1;
variable i;
variable k;
variable j;

%Declare arrays
variable g_a_real = Double_Type[number_bands];
variable g_a_imag = Double_Type[number_bands];
variable g_a = Double_Type[number_bands];
variable g_b = Double_Type[number_bands];
variable g_c = Double_Type[number_bands];
variable g = Double_Type[number_bands];
variable delta_phi = Double_Type[number_bands];
variable delta_lag = Double_Type[number_bands];
variable lag = Double_Type[number_bands];

%Set frequency range interested in
variable lo = 0.8;
variable hi = 2;


%Logarithmic centre of frequency bin
variable rb_freq = 10^(0.5*(log10(lo)+log10(hi)));

%counts CPS for each binlag_en_script.sl
variable rb_n = Integer_Type[number_bands];

%Define energy bins
variable elo = Double_Type[number_bands];
variable ehi = Double_Type[number_bands];

for(i=0; i<number_bands;i++){
        elo[i] =  band[i];
        ehi[i] = band[i+1];
}


%loop through observations
for(k=0; k<length(obs_id); k++){

%change to appropriate directory for observation

variable fn_r;
variable fn_n;

%loop through energy bands
for(i=0; i<number_bands; i++){

%read in fits file - MAKE SURE FILE NAMES MATCH
fn_r = sprintf("reference_%i_%i_lccorr.fits",band[i],band[i+1]);
fn_n = sprintf("narrow_%i_%i_lccorr.fits",band[i],band[i+1]);

variable lc_reference = fits_read_table(fn_r);
variable lc_narrow = fits_read_table(fn_n);

%exclude non-numbers:
variable ix_reference = where(not isnan(lc_reference.rate));
variable ix_narrow = where(not isnan(lc_narrow.rate));

% Pass to new variables:
variable time_reference = lc_reference.time[ix_reference];
variable time_narrow = lc_narrow.time[ix_narrow];
variable rate_reference = lc_reference.rate[ix_reference];
variable rate_narrow = lc_narrow.rate[ix_narrow];
variable error_reference = lc_reference.error[ix_reference];
variable error_narrow = lc_narrow.error[ix_narrow];

% Compute reference dft:
variable dft_reference = fft(rate_reference,-1);
variable freq = [[0:length(dft_reference)-1]]/(double(length(dft_reference))*(time_reference[1]-time_reference[0]));
variable dft_real_reference = Real(dft_reference[[0:length(freq)-1]]);
variable dft_imag_reference = Imag(dft_reference[[0:length(freq)-1]]);

% Compute narrow dft:
variable dft_narrow = fft(rate_narrow,-1);
variable dft_real_narrow = Real(dft_narrow[[0:length(freq)-1]]);
variable dft_imag_narrow = Imag(dft_narrow[[0:length(freq)-1]]);

% Calculate CPS in the frequency range [lo,hi] for each energy bin [i], summing across observations.
for (j=0; j<length(freq); j++){
if(freq[j] > lo && freq[j] <= hi)
                {
                        g_a_real[i] += dft_real_reference[j]*dft_real_narrow[j] + dft_imag_reference[j]*dft_imag_narrow[j];
                        g_a_imag[i] += dft_real_narrow[j]*dft_imag_reference[j]-dft_real_reference[j]*dft_imag_narrow[j];
                        g_b[i] += dft_real_reference[j]*dft_real_reference[j] + dft_imag_reference[j]*dft_imag_reference[j];
                        g_c[i] += dft_real_narrow[j]*dft_real_narrow[j] + dft_imag_narrow[j]*dft_imag_narrow[j];
                        rb_n[i] ++;
                }

}
}
}

variable x = (ehi+elo)/2;
variable dxp = ehi-x;
variable dxm = x-elo;

%Average the CPS for each energy bin for all observations. Calculate coherence, g[i], for each energy bin.
for(i=0; i<number_bands; i++){
        %Lag error
        g_a[i] = (g_a_real[i]*g_a_real[i] + g_a_imag[i]*g_a_imag[i])/(double(rb_n[i])*double(rb_n[i]));
        g_b[i] /= double(rb_n[i]);
        g_c[i] /= double(rb_n[i]);
        g[i] = g_a[i]/(g_b[i]*g_c[i]);
        delta_phi[i] = sqrt((1.0-g[i])/(2.0*g[i]))/sqrt(double(rb_n[i]));
        delta_lag[i] = delta_phi[i]/(2.0*PI*rb_freq);

        %Lag
        g_a_real[i] /= rb_n[i];
        g_a_imag[i] /= rb_n[i];
        lag[i] = atan2(g_a_imag[i] , g_a_real[i])/(2.0*PI*rb_freq);

}

%open_plot("lagen_0.8-2Hz.gif/gif");
xlog;
ylin;
xlabel("Energy (eV)");
ylabel("Time Lag (s)");
title("GX339-4 0605610201 lag-energy 0.8-2 Hz");
connect_points(0);
_pgsfs(3);
plotxy(x,dxm,dxp,lag,delta_lag,delta_lag; dcol=1, decol=2, dsym=6, xrange=[300,11000], yrange=[-0.02,0.02]);
_pgsls(2);
_pgslw(1);
_pgdraw(1,0);

for (i=0; i<length(x); i++) {
  () = printf("%e,%e,%e\n", x[i], lag[i], delta_lag[i]);
}
%close_plot;

#+END_SRC
