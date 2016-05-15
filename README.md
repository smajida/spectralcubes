# Face Spoofing Detection Through Visual Codebooks of Spectral Temporal Cubes

### Abstract

Despite important recent advances, the vulnerability of biometric systems to spoofing attacks is still an open problem. Spoof attacks occur when impostor users present synthetic biometric samples of a valid user to the biometric system seeking to deceive it. Considering the case of face biometrics, a spoofing attack consists in presenting a fake sample (e.g., photograph, digital video or even a 3D mask) to the acquisition sensor with the facial information of a valid user. In this paper, we introduce a low-cost and software-based method for detecting spoofing attempts in face recognition systems. Our hypothesis is that during acquisition there will be inevitable artifacts left behind in the recaptured biometric samples allowing us to create a discriminative signature of the video generated by the biometric sensor. To characterize these artifacts, we extract time-spectral feature descriptors from the video, which can be understood as a low-level feature descriptor that gathers temporal and spectral information across the biometric sample and use the visual codebook concept to find mid-level feature descriptors computed from the low-level ones. Such descriptors are more robust for detecting several kinds of attacks than low-level ones. Experimental results show the effectiveness of the proposed method for detecting different types of attacks in a variety of scenarios and datasets including photos, videos and 3D masks.


### Requirements to Run this Software

The OpenCV Package 2.4.11 or later is required for use this software.

The other requirements are python packages and are listed in **requirements.txt**.
We provide a script *(install_requirements.sh)*, to install theses python requirements via **pip command**.    

This software runs on Linux Operating systems, and we tested it by using Ubuntu 14.04 LTS.

### How to Use this Software?

This software run only by command line interfaces (CLIs) such as the shell program (e.g., sh, bash, ksh). To see the usage of this sofware, use the follow command:

>     spectralcubesantispoofing.py --help

### Examples

1. Run this software to reproduce the results from Replay-Attack dataset:
>     
>     spectralcubesantispoofing.py --dataset 0 --dataset_path datasets/replayattack --output_path ./working --protocol intra_dataset
>     

1. Run this software to reproduce the results from CASIA FASD dataset:
>     
>     spectralcubesantispoofing.py --dataset 1 --dataset_path datasets/casia --output_path ./working --protocol intra_dataset
>     

1. Run this software to reproduce the results from 3DMAD dataset:
>     
>     spectralcubesantispoofing.py --dataset 2 --dataset_path datasets/3dmad --output_path ./working --protocol intra_dataset
>     

1. Run this software to reproduce the results from UVAD dataset:
>     
>     spectralcubesantispoofing.py --dataset 3 --dataset_path datasets/uvad --facelocations_path datasets/uvad/face-locations --output ./working --protocol intra_dataset
>     

### Please, Cite our Work!

If you use this software, please cite our paper published in *IEEE Transactions on Image Processing*:

> **Reference**
>
>     Pinto, A.; Pedrini, H.; Robson Schwartz, W.; Rocha, A., "Face Spoofing Detection Through Visual Codebooks of Spectral Temporal Cubes," in Image Processing, IEEE Transactions on , vol.24, no.12, pp.4726-4740, Dec. 2015
>     doi: 10.1109/TIP.2015.2466088
>     keywords: {face recognition;feature extraction;image coding;image sensors;spatiotemporal phenomena;acquisition sensor;biometric system vulnerability;discriminative video signature;face biometrics;face recognition systems;face spoofing detection;low-level feature descriptor;recaptured biometric samples;software-based method;spectral information;spectral temporal cubes;spoofing attack;synthetic biometric samples;temporal information;time-spectral feature descriptor extraction;visual codebook concept;visual codebooks;Face;Face recognition;Feature extraction;Noise;Three-dimensional displays;Visualization;Face spoofing attack detection;face biometric system;mobile device;mobile device, face biometric system;spectral analysis;time-spectral visual features;timespectral visual features;visual codebook},
>     URL: http://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7185398&isnumber=7271151


> **Bibtex**
>
>     @ARTICLE{7185398,
>     author={Pinto, A. and Pedrini, H. and Robson Schwartz, W. and Rocha, A.},
>     journal={Image Processing, IEEE Transactions on},
>     title={Face Spoofing Detection Through Visual Codebooks of Spectral Temporal Cubes},
>     year={2015},
>     volume={24},
>     number={12},
>     pages={4726-4740},
>     keywords={face recognition;feature extraction;image coding;image sensors;spatiotemporal phenomena;acquisition sensor;biometric system vulnerability;discriminative video signature;face biometrics;face recognition systems;face spoofing detection;low-level feature descriptor;recaptured biometric samples;software-based method;spectral information;spectral temporal cubes;spoofing attack;synthetic biometric samples;temporal information;time-spectral feature descriptor extraction;visual codebook concept;visual codebooks;Face;Face recognition;Feature extraction;Noise;Three-dimensional displays;Visualization;Face spoofing attack detection;face biometric system;mobile device;mobile device, face biometric system;spectral analysis;time-spectral visual features;timespectral visual features;visual codebook},
>     doi={10.1109/TIP.2015.2466088},
>     ISSN={1057-7149},
>     month={Dec},}


### License

This software is available under condition of the New BSD Licence, whose terms are:

    Copyright (c) 2015, Allan Pinto, Helio Pedrini, William Robson Schwartz, and Anderson Rocha
    All rights reserved.

    Redistribution and use in source and binary forms, with or without
    modification, are permitted provided that the following conditions are met:

    * Redistributions of source code must retain the above copyright notice, this
      list of conditions and the following disclaimer.

    * Redistributions in binary form must reproduce the above copyright notice,
      this list of conditions and the following disclaimer in the documentation
      and/or other materials provided with the distribution.

    * Neither the name of University of Campinas (Unicamp) nor the names of its
      contributors may be used to endorse or promote products derived from
      this software without specific prior written permission.

    THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
    AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
    IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
    DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
    FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
    DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
    SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
    CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
    OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
    OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
