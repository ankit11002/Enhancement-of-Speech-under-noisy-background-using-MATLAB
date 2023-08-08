# Enhancement-of-Speech-under-noisy-background-using-MATLAB
An improved multi-band spectral subtraction algorithm  with the goal of improving the quality of speech signal in various noise environments.
In the proposed enhancement algorithm, the whole speech spectrum is divided into different uniformly spaced continuous frequency bands and spectral over-subtraction is performed in each band, independently. 
The proposed algorithm uses a novel approach to estimate the noise from each band continuously, without using speech pause detection. The noise is estimated and updated by adaptively smoothing the noisy signal power in each uniformly spaced frequency band. The smoothing parameter is controlled by a linear function of a-posteriori signal-to-noise ratio (SNR). 
The input is taken from a noisy speech. To test the performance of the proposed speech enhancement algorithm, objective quality measurement tests (SNR, segmental SNR (Seg. SNR), and perceptual evaluation of speech quality (PESQ)) and spectrogram with informal listening tests are conducted for various noise types 
at different SNRs.
Proposed Method 
1.Subband Decomposition: The input speech signal is divided into multiple 
subbands using a filter bank. Each subband contains a portion of the speech 
spectrum, allowing for independent processing of noise reduction. 
2. Noise Power Spectrum Estimation: For each subband, the noise power 
spectrum is adaptively estimated based on the characteristics of the noisy 
speech. This adaptive estimation accounts for varying noise levels across 
different subbands, providing a more accurate representation of the noise in 
each frequency range. 
3. Spectral Subtraction: With the estimated noise power spectrum for each 
subband, spectral subtraction is applied independently in each subband. The 
noisy speech spectrum in each subband is attenuated by the estimated noise 
power spectrum, resulting in a clean speech spectrum in each subband. 
4. Inverse Subband Decomposition: After applying spectral subtraction in 
the subband domain, the modified subbands are combined to reconstruct 
the enhanced speech signal. The reconstructed signal exhibits reduced noise 
while preserving the original speech components. 
5. SNR-Based Adaptive Control: The method utilizes the Signal-to-Noise 
Ratio (SNR) of each subband to adaptively control the spectral subtraction 
process. Based on the SNR, the algorithm adjusts the subtraction factor, 
emphasizing speech components while suppressing noise. 
6. VAD (Voice Activity Detection): The method includes a Voice Activity 
Detection algorithm to determine whether a subband contains speech or 
noise. This helps to update the noise estimate adaptively and further 
improves noise reduction performance.
