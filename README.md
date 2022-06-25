# EEGBetaThetaExtraction
This is implementation of Beta(4-7Hz), Theta(13-25Hz) extraction for EDF formatted EEG data by spectogram. and LDA classification of cognitive process for "[Albasri, Ahmed (2019), EEG dataset of Fusion relaxation and concentration moods”, Mendeley Data, V1, doi: 10.17632/8c26dn6c7w.1](https://data.mendeley.com/datasets/8c26dn6c7w/1)

# Requirements
mne, scipy, matplotlib, numpy, sklearn, pandas required.<br>
`!pip install mne scipy matplotlib numpy sklearn pandas`

# Methods
`fileToLabeld` returns labeled theta/beta data for channel wise by given path(edf). signal p8 skipped due to dataset errors so shape of return is (256(hz)*180(sec), 13(channels)) for EEG concentration dataset.

`folderToLabeled` returns concatenated dataset from specified folder. <br>

`getData` returns (train, test) data according to given params.<br>

`classify` returns (input_data, labeled) <br>

# Install
[Edf dataset](https://data.mendeley.com/datasets/8c26dn6c7w/1) should located at ./edfs.

# Contributors
Hyungi Cho (Catholic Univ., [@jasonhk24](https://github.com/jasonhk24))
