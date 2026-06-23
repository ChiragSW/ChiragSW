<div align="center">
 
<img src="banner (2).svg" width="1000px" style="border-radius: 50%;" alt="avatar"/>
 
# Open Source Contributions


<a href="https://github.com/llvm/llvm-project">
<img width="240" height="150" alt="image" src="https://github.com/user-attachments/assets/56e123a7-5cca-4663-bd1e-7ac246746b7e" />
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

[Issue: #204911](https://github.com/llvm/llvm-project/issues/204911)

mlir(convert-tensor-to-spirv) mlir-opt crashes at BuiltinAttributes.cpp:366 with assertion `(getType().isIndex() || getType().isSignlessInteger()) && "must be signless integer"' failed.
 
</td>
<td width="50%">
 
[PR - #204937](https://github.com/llvm/llvm-project/pull/204937)

Updated arith.constant verification to reject integer constants with signed and unsigned element types including shaped constants like tensors and vectors, as the arith dialect does not support signed/unsigned types.
 
</td>
</tr>
