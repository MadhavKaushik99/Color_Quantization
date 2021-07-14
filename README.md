# Color_Quantization
Reduced the number of colours required while preserving overall image appearance quality.

Vector Quantization (VQ) is an efficient technique for data compression. It has recently emerged as a powerful and efficient technique for digital speech and image coding.

The key to VQ is the good codebook. Good codebook design leads to less distortion in reconstructed image. The goal of this process is data compression to minimize communication channel capacity or digital storage memory requirements while maintaining an acceptable fidelity level of the data.

Vector Quantization works by dividing a large set of points (vectors) into groups having approximately the same number of points closest to them. Each group is represented by its centroid point, as in k-means and some other clustering algorithms.

Color quantization is a process that reduces the number of distinct colors used in an image with the aim that the new image should be as visually similar as possible to the original image. In this we map from high resolution to lower resolution. In the image processing literature, the codebook obtained from K-means (the cluster centers) is called the color palette.

After generation of codebook, two processes are done:-

Encoding : • Instead of the original data value, closest value in the alphabet of reference vectors called codebook vectors or code words is used. • Encoder tires to generate and assign the address of codebook vector in the codebook for the input vector. • For encoding, the criterion of least minimum distortion is used to generate the codebook • The output of the encoder is the address of searched vector.

Decoding : • Image is reconstructed as each pixel is represented with the most similar entry in the codebook. • That is, instead of the original data value, the closest value for each of the pixel in the codebook is used. • The decoder is only a simple (hence fast) look-up table indexed by codeword containing the replacement vectors.
