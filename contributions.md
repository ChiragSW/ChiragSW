<div align="center">
 
<img src="banner (2).svg" width="1000px" style="border-radius: 50%;" alt="avatar"/>
 
# Open Source Contributions
 

<a href="https://github.com/keras-team/keras">
<img src="kerass.png" width="300"/>
</a>

</div>

<table>
<tr>
  <tr>
    <th width="5%">S.No</th>
    <th width="45%"> Issue</th>
    <th width="50%"> Pull Request</th>
  </tr>
<td width="5%">1</td>
<td width="45%">

[#22428 - Conv1DTranspose: Invalid Symbolic Shape + Runtime Crash When output_padding ≥ strides
](https://github.com/keras-team/keras/issues/22428)
 
</td>
<td width="50%">
 
[PR - #22439](https://github.com/keras-team/keras/pull/22439)

Validates output_padding < strides, adds tests, improves error clarity
 
</td>
</tr>

<tr>
<td>2</td>
<td>

[#22429 - Conv2DTranspose: Invalid Symbolic Shape + Runtime Crash (output_padding ≥ strides per dimension)(related to #22428)](https://github.com/keras-team/keras/issues/22429)

</td>
<td>

[PR - #22439](https://github.com/keras-team/keras/pull/22439)

Validates output_padding < strides, adds tests, improves error clarity

</td>
</tr>

<tr>
<td>3</td>
<td>

[#22430 - Conv3DTranspose: Invalid Symbolic Shape + Runtime Crash (output_padding ≥ strides for 3D dimensions)(related to #22428 & #22429)](https://github.com/keras-team/keras/issues/22430)

</td>
<td>

[PR - #22439](https://github.com/keras-team/keras/pull/22439)

Validates output_padding < strides, adds tests, improves error clarity

</td>
</tr>

<tr>
<td>4</td>
<td>

[#22474 - ConvLSTM1D allows invalid strides/dilation config when built with Keras Input](https://github.com/keras-team/keras/issues/22474)

</td>
<td>

[PR - #22477](https://github.com/keras-team/keras/pull/22477)

Added validation in ConvLSTMCell.__init__to raise ValueError when both are > 1.
Added regression tests to ensure symbolic builds now correctly fail across ConvLSTM1D

</td>
</tr>

<tr>
<td>5</td>
<td>

[#22475 - ConvLSTM2D allows invalid strides+dilation_rate config when built with Keras.Input](https://github.com/keras-team/keras/issues/22475)

</td>
<td>

[PR - #22477](https://github.com/keras-team/keras/pull/22477)

Added validation in ConvLSTMCell.__init__to raise ValueError when both are > 1.
Added regression tests to ensure symbolic builds now correctly fail across ConvLSTM2D

</td>
</tr>

<tr>
<td>6</td>
<td>

[#22476 - ConvLSTM3D fails to validate incompatible strides and dilation_rate in symbolic mode](https://github.com/keras-team/keras/issues/22476)

</td>
<td>

[PR - #22477](https://github.com/keras-team/keras/pull/22477)

Added validation in ConvLSTMCell.__init__to raise ValueError when both are > 1.
Added regression tests to ensure symbolic builds now correctly fail across ConvLSTM3D

</td>
</tr>

<tr>
<td>7</td>
<td>

[#22472 - rgb_to_hsv does not validate channel count for Keras Input with channels_first](https://github.com/keras-team/keras/issues/22472)

</td>
<td>

[PR - #22478](https://github.com/keras-team/keras/pull/22478)

Added explicit channel-count validation in compute_output_spec().
Added regression tests to ensure invalid-channel inputs raise errors rgb_to_hsv

</td>
</tr>

<tr>
<td>8</td>
<td>

[#22473 - keras.ops.image.hsv_to_rgb accepts invalid channels_first shape in symbolic mode](https://github.com/keras-team/keras/issues/22473)

</td>
<td>

[PR - #22478](https://github.com/keras-team/keras/pull/22478)

Added explicit channel-count validation in compute_output_spec().
Added regression tests to ensure invalid-channel inputs raise errors hsv_to_rgb

</td>
</tr>

<tr>
<td>9</td>
<td>

[#22479 - AttributeError in ZIP extraction: 'ZipInfo' object has no attribute 'name'](https://github.com/keras-team/keras/issues/22479)

</td>
<td>

[PR - #22480](https://github.com/keras-team/keras/pull/22480)

Updated warning message in keras/src/utils/file_utils.py to use finfo.filename instead of finfo.name

</td>
</tr>

<tr>
<td>10</td>
<td>

[#22543 - keras.ops.sort(axis=None) fails on eager tensors instead of flattening and sorting](https://github.com/keras-team/keras/issues/22543)

</td>
<td>

[PR - #22544](https://github.com/keras-team/keras/pull/22544)

Updated the sort operation across TensorFlow and PyTorch backends to support axis=None, ensuring the output correctly flattens and matches NumPy's behavior.

</td>
</tr>

<tr>
<td>11</td>
<td>

[#22406 - TextVectorization fails on G4 on Colab (all fine on H100, or A100 and earlier)](https://github.com/keras-team/keras/issues/22406)

</td>
<td>

[PR - #22465](https://github.com/keras-team/keras/pull/22465)

Wrapped TF string/hash/lookup operations in with tf.device("CPU:0") to avoid GPU dispatch issues. Added GPU regression tests that are automatically skipped on CPU-only machines.

</td>
</tr>

<tr>
<td>12</td>
<td>

[#22058 - Resolve infinite recursion in keras.ops.associative_scan under Tensorflow static graph mode](https://github.com/keras-team/keras/issues/22058)

</td>
<td>

[PR - #22072](https://github.com/keras-team/keras/pull/22072)

Resolved an infinite recursion issue encountered in ```keras.ops.associative_scan``` when operating within TensorFlow's static graph mode (tf.function) with symbolic input shapes. The core of the fix involved leveraging static shape information to guide conditional execution, thereby preventing the tracing of recursive paths when the element length is known at graph construction time. This ensures that the associative_scan operation behaves correctly and efficiently under both static and dynamic tensor length scenarios.

</td>
</tr>

<tr>
<td>13</td>
<td>

[#22538 - keras.ops.blackman returns NaN for window length 1](https://github.com/keras-team/keras/issues/22538)

</td>
<td>

[PR - #22545](https://github.com/keras-team/keras/pull/22545)

Addressed a critical bug in the ```keras.ops.blackman``` function that caused it to produce NaN outputs for a window length of 1. Implemented a robust solution to prevent division by zero in this specific scenario, ensuring the function consistently returns accurate Blackman window values. 

</td>
</tr>

<tr>
<td>14</td>
<td>

[#22539 - keras.ops.flip fails for eager tensors when axis is a list of axes](https://github.com/keras-team/keras/issues/22539)

</td>
<td>

[PR - #22548](https://github.com/keras-team/keras/pull/22548)

Updated the TensorFlow backend implementation of the flip operation to support multiple axes and negative axis indexing, ensuring consistency with Numpy behavior.

</td>
</tr>

<tr>
<td>15</td>
<td>

[#22535 - MelSpectrogram skips fft_length >= sequence_length validation for symbolic Keras inputs](https://github.com/keras-team/keras/issues/22535)

</td>
<td>

[PR - #22549](https://github.com/keras-team/keras/pull/22549)

Added a validation check in the MelSpectrogram layer to ensure that fft_length is at least as large as sequence_length, along with a corresponding unit test to verify this behavior.

</td>
</tr>

<tr>
<td>16</td>
<td>

[#22586 - Mixed Precision (float16) numerical instability in GroupNormalization with small epsilon](https://github.com/keras-team/keras/issues/22586)

</td>
<td>

[PR - #22589](https://github.com/keras-team/keras/pull/22589)

Updated the GroupNormalization layer to improve numerical stability during mixed precision training. It disables automatic casting for the layer and its weights (gamma and beta) and adds an explicit cast to compute_dtype at the end of the call method.

</td>
</tr>

<tr>
<td>17</td>
<td>

[APIs in the keras.ops module lack validity checks when accepting Keras.Input as an input](https://github.com/keras-team/keras/issues/22472#issuecomment-4133026201)

</td>
<td>

[PR - #22707](https://github.com/keras-team/keras/pull/22707)

Added input validation for image padding and cropping, including helper functions to enforce non-negative and properly specified parameters, along with comprehensive unit tests.

</td>
</tr>

<tr>
<td>18</td>
<td>

[Refactor axis validation and canonicalization for targeted review](https://github.com/keras-team/keras/issues/22472#issuecomment-4133026201)

</td>
<td>

[PR - #22708](https://github.com/keras-team/keras/pull/22708)

Introduced axis normalization utilities and updated various operations, including log_softmax, sparsemax, and roll, to utilize these helpers for more consistent behavior.

</td>
</tr>

<tr>
<td>19</td>
<td>

[[Bug] PR test-workflow title shows raw template expression instead of evaluated value](https://github.com/keras-team/keras/issues/22776)

</td>
<td>

[PR - #22824](https://github.com/keras-team/keras/pull/22824)

Replace the dynamic expression with explicit matrix.include fields (name_suffix, runner) so the job name evaluates reliably to:
- Run tests on TPU for single-device
- Run tests on multi-TPU for multi-device

</td>
</tr>

<tr>
<td>20</td>
<td>

[[Bug] Torch divide_no_nan() produces NaN gradients](https://github.com/keras-team/keras/issues/23063)

</td>
<td>

[PR - #23064](https://github.com/keras-team/keras/pull/23064)

Updated the PyTorch backend implementation of divide_no_nan to prevent gradient issues when division by zero occurs by introducing a safe divisor tensor.

</td>
</tr>

<tr>
<td>21</td>
<td>

[[Bug] Audio padded batching assumes scalar labels](https://github.com/keras-team/keras/issues/23061)

</td>
<td>

[PR - #23062](https://github.com/keras-team/keras/pull/23062)

Simplified the dataset padding logic in `audio_dataset_utils.py` by removing explicit padded_shapes from padded_batch when the output sequence length is dynamic
and the dataset is not ragged.

</td>
</tr>

<tr>
<td>22</td>
<td>

[[Bug] Sparse TensorFlow wrapper drops trailing all-zero rows](https://github.com/keras-team/keras/issues/23059)

</td>
<td>

[PR - #23060](https://github.com/keras-team/keras/pull/23060)

Fixed an issue where trailing empty rows in a `tf.SparseTensor` were truncated during data adaptation. In `array_slicing.py` nrows is now explicitly passed to `tf.experimental.RowPartition.from_value_rowids` using the sparse tensor's dense shape.

</td>
</tr>

<tr>
<td>23</td>
<td>

[[Bug]  Empty py generator passed to model.fit raises raw IndexError](https://github.com/keras-team/keras/issues/23072)

</td>
<td>

[PR - #23074](https://github.com/keras-team/keras/pull/23074)

Added a check to `GeneratorDataAdapter` to raise a clear ValueError when an empty generator is passed.

</td>
</tr>

<tr>
<td>24</td>
<td>

[ValueError when loading SAMImageSegmenter from preset sam_huge_sa1b in Keras Hub](https://github.com/keras-team/keras/issues/23018)

</td>
<td>

[PR - #23036](https://github.com/keras-team/keras/pull/23036)

Updated the weight saving and loading mechanisms in Keras to recursively resolve and skip nested saveable objects when `objects_to_skip` is provided. Specifically, replaced the shallow ID collection in `save_weights_only` and `load_weights_only` with a recursive helper `_get_saveable_ids` that traverses KerasSaveable objects and standard Python containers (lists, tuples, sets, dicts)

</td>
</tr>

<tr>
<td>25</td>
<td>

[[Bug] TorchDataLoaderAdapter corrupts dict and single-tensor batches on non-Torch backends](https://github.com/keras-team/keras/issues/23080)

</td>
<td>

[PR - #23096](https://github.com/keras-team/keras/pull/23096)

Removed the force change of the dict and single tensor batches to tuple(...). Now tree utilities preserve the batch structure. Added a tf specific normalization so now nested lists to tuples without converting dicts or tensors accidentally. Added regression tests for the same.

</td>
</tr>

<tr>
<td>26</td>
<td>

[[Bug] sklearn wrapper warm_start=True does not reuse model instance weights](https://github.com/keras-team/keras/issues/23097)

</td>
<td>

[PR - #23098](https://github.com/keras-team/keras/pull/23098)

Added an extra check in the _get_model function so now it uses previous model instead of cloning new one. Also added regression test for the same.

</td>
</tr>

<tr>
<td>27</td>
<td>

[keras.ops.nancumsum returns finite values instead of inf/nan for inputs containing NaN and infinities](https://github.com/keras-team/keras/issues/23130)

</td>
<td>

[PR - #23135](https://github.com/keras-team/keras/pull/23135)

Updated the nancumsum implementation across the OpenVINO, TensorFlow, and PyTorch backends to ensure that positive and negative infinity values are preserved by passing posinf=float("inf") and neginf=float("-inf") to nan_to_num

</td>
</tr>

<tr>
<td>28</td>
<td>

[keras.ops.nancumprod returns float32 max instead of inf for NaN followed by Inf](https://github.com/keras-team/keras/issues/23127)

</td>
<td>

[PR - #23134](https://github.com/keras-team/keras/pull/23134)

nan_to_num(x, nan=1.0) used a buggy path, it converted inf values to floats as default. Fixed it such that nancumprod replaces only NaNs with 1.0 preserving inf and -inf.

</td>
</tr>

<tr>
<td>29</td>
<td>

[[Bug] Torch random.shuffle(axis=-1) mishandles negative axes](https://github.com/keras-team/keras/issues/23118)

</td>
<td>

[PR - #23119](https://github.com/keras-team/keras/pull/23119)

Updated the PyTorch backend's random.shuffle implementation to support negative axes by using canonicalize_axis.

</td>
</tr>

<tr>
<td>30</td>
<td>

[[Bug] Segmentation mask visualization docs use one-based class labels but implementation uses zero-based indices](https://github.com/keras-team/keras/issues/23088)

</td>
<td>

[PR - #23114](https://github.com/keras-team/keras/pull/23114)

Updated the segmentation mask visualization utilities to support 0-indexed class indices (from 0 to num_classes - 1) instead of 1-indexed ones, and adjusts the automatic inference of num_classes accordingly.

</td>
</tr>

<tr>
<td>31</td>
<td>

[keras.ops.hypot returns NaN instead of Inf for Inf and -Inf inputs](https://github.com/keras-team/keras/issues/23131)

</td>
<td>

[PR - #23157](https://github.com/keras-team/keras/pull/23157)

Tf and OpenVINO backends used max * sqrt(1 + (min/max)^2) but inf / inf gives nan
Now both return positive inf when either input is inf

</td>
</tr>

<tr>
<td>32</td>
<td>

[keras.ops.isclose incorrectly returns False for matching positive and negative infinities](https://github.com/keras-team/keras/issues/23128)

</td>
<td>

[PR - #23136](https://github.com/keras-team/keras/pull/23136)

TensorFlow and openvino backends computed abs(x1 - x2) <= tolerance; inf - inf becomes NaN, so it returned False. Now fixed it so it only checks finite values.

</td>
</tr>

</table>

<div align="center">
</div>
