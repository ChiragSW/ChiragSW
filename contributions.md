<div align="center">
 
<img src="banner (2).svg" width="1000px" style="border-radius: 50%;" alt="avatar"/>
 
# Open Source Contributions
 
</div>
 
### [<img src="kerass.png" width="200"/>](https://github.com/keras-team/keras)

<table>
<tr>
  <tr>
    <th width="50%"> Issue</th>
    <th width="50%"> Merged PR</th>
  </tr>
<td width="50%">

[#22428 - Conv1DTranspose: Invalid Symbolic Shape + Runtime Crash When output_padding ≥ strides
](https://github.com/keras-team/keras/issues/22428)
 
</td>
<td width="50%">
 
[PR - #22439](https://github.com/keras-team/keras/pull/22439)

Validates output_padding < strides, adds tests, improves error clarity
 
</td>
</tr>

<tr>
<td width="50%">

[#22429 - Conv2DTranspose: Invalid Symbolic Shape + Runtime Crash (output_padding ≥ strides per dimension)(related to #22428)](https://github.com/keras-team/keras/issues/22429)

</td>
<td width="50%">

[PR - #22439](https://github.com/keras-team/keras/pull/22439)

Validates output_padding < strides, adds tests, improves error clarity

</td>
</tr>

<tr>
<td width="50%">

[#22430 - Conv3DTranspose: Invalid Symbolic Shape + Runtime Crash (output_padding ≥ strides for 3D dimensions)(related to #22428 & #22429)](https://github.com/keras-team/keras/issues/22430)

</td>
<td width="50%">

[PR - #22439](https://github.com/keras-team/keras/pull/22439)

Validates output_padding < strides, adds tests, improves error clarity

</td>
</tr>

<tr>
<td width="50%">

[#22474 - ConvLSTM1D allows invalid strides/dilation config when built with Keras Input](https://github.com/keras-team/keras/issues/22474)

</td>
<td width="50%">

[PR - #22477](https://github.com/keras-team/keras/pull/22477)

Added validation in ConvLSTMCell.__init__to raise ValueError when both are > 1.
Added regression tests to ensure symbolic builds now correctly fail across ConvLSTM1D

</td>
</tr>

<tr>
<td width="50%">

[#22475 - ConvLSTM2D allows invalid strides+dilation_rate config when built with Keras.Input](https://github.com/keras-team/keras/issues/22475)

</td>
<td width="50%">

[PR - #22477](https://github.com/keras-team/keras/pull/22477)

Added validation in ConvLSTMCell.__init__to raise ValueError when both are > 1.
Added regression tests to ensure symbolic builds now correctly fail across ConvLSTM2D

</td>
</tr>

<tr>
<td width="50%">

[#22476 - ConvLSTM3D fails to validate incompatible strides and dilation_rate in symbolic mode](https://github.com/keras-team/keras/issues/22476)

</td>
<td width="50%">

[PR - #22477](https://github.com/keras-team/keras/pull/22477)

Added validation in ConvLSTMCell.__init__to raise ValueError when both are > 1.
Added regression tests to ensure symbolic builds now correctly fail across ConvLSTM3D

</td>
</tr>

<tr>
<td width="50%">

[#22472 - rgb_to_hsv does not validate channel count for Keras Input with channels_first](https://github.com/keras-team/keras/issues/22472)

</td>
<td width="50%">

[PR - #22478](https://github.com/keras-team/keras/pull/22478)

Added explicit channel-count validation in compute_output_spec().
Added regression tests to ensure invalid-channel inputs raise errors rgb_to_hsv

</td>
</tr>

<tr>
<td width="50%">

[#22473 - keras.ops.image.hsv_to_rgb accepts invalid channels_first shape in symbolic mode](https://github.com/keras-team/keras/issues/22473)

</td>
<td width="50%">

[PR - #22478](https://github.com/keras-team/keras/pull/22478)

Added explicit channel-count validation in compute_output_spec().
Added regression tests to ensure invalid-channel inputs raise errors hsv_to_rgb

</td>
</tr>

<tr>
<td width="50%">

[#22479 - AttributeError in ZIP extraction: 'ZipInfo' object has no attribute 'name'](https://github.com/keras-team/keras/issues/22479)

</td>
<td width="50%">

[PR - #22480](https://github.com/keras-team/keras/pull/22480)

 Updated warning message in keras/src/utils/file_utils.py to use finfo.filename instead of finfo.name

</td>
</tr>

</table>

<div align="center">
</div>
