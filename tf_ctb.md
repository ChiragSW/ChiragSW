<div align="center">
 
<img src="banner (2).svg" width="1000px" style="border-radius: 50%;" alt="avatar"/>
 
# Tensorflow


<a href="https://github.com/tensorflow/tensorflow">
  <img width="100" height="100" alt="image" src="https://github.com/user-attachments/assets/41b7fb69-ea2b-4fd8-836e-d349bf69b9cd" />
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

[Issue: #118727](https://github.com/tensorflow/tensorflow/issues/118727)

tf.bitcast after tf.cast to uint64 differs between eager and XLA
 
</td>
<td width="50%">
 
[PR - #118744](https://github.com/tensorflow/tensorflow/pull/118744)

Updated TensorFlow-to-XLA cast lowering to preserve TensorFlow behavior by routing negative float values through a signed integer conversion before converting to unsigned.
</td>
</tr>
