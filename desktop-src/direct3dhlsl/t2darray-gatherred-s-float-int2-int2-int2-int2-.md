---
title: GatherRed(S,float,int2,int2,int2,int2) function
description: Samples a texture and returns the red component.
ms.assetid: EB367373-D798-4CBA-AEB6-8BF89371D765
keywords:
- GatherRed function HLSL
topic_type:
- apiref
api_name:
- GatherRed
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
api_location: 
---

# GatherRed(S,float,int2,int2,int2,int2) function

Samples a texture and returns the red component.

## Syntax


```C++
TemplateType GatherRed(
  _In_ SamplerState S,
  _In_ float        Location,
  _In_ int2         Offset1,
  _In_ int2         Offset2,
  _In_ int2         Offset3,
  _In_ int2         Offset4
);
```



## Parameters

<dl> <dt>

*S* \[in\]
</dt> <dd>

Type: **SamplerState**

The zero-based sampler index.

</dd> <dt>

*Location* \[in\]
</dt> <dd>

Type: **float**

The sample coordinates (u,v).

</dd> <dt>

*Offset1* \[in\]
</dt> <dd>

Type: **int2**

The first offset component applied to the texture coordinates before sampling.

</dd> <dt>

*Offset2* \[in\]
</dt> <dd>

Type: **int2**

The second offset component applied to the texture coordinates before sampling.

</dd> <dt>

*Offset3* \[in\]
</dt> <dd>

Type: **int2**

The third offset component applied to the texture coordinates before sampling.

</dd> <dt>

*Offset4* \[in\]
</dt> <dd>

Type: **int2**

The fourth offset component applied to the texture coordinates before sampling.

</dd> </dl>

## Return value

Type: **TemplateType**

A four-component value whose type is the same as the template type.

## Remarks

The texture samples can be used for bilinear interpolation.

This function is supported for the following types of shaders:



| Vertex | Hull | Domain | Geometry | Pixel | Compute |
|--------|------|--------|----------|-------|---------|
| x      | x    | x      | x        | x     | x       |



 

## See also

<dl> <dt>

[GatherRed methods](texture2darray-gatherred.md)
</dt> </dl>

 

 




