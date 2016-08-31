## Deep Learning

* Recommanded Papers

	| Network | Code |
	|--------|--------|
	|[LeNet5](http://yann.lecun.com/exdb/publis/pdf/lecun-98.pdf)        |        |
	|AlexNet|--------|
	|GoogLeNet|--------|
	|ResNet|--------|
    |DenseNet|https://github.com/liuzhuang13/DenseNet|

* MS Caffe : http://github.com/Microsoft/caffe
 
* Datasets
	* MNIST : http://yann.lecun.com/exdb/mnist
	* CIFAR : (Krizhevsky & Hinton, 2009)
	* SVHN : (Netzer et al. 2011)

* LeNet-5

<style type="text/css">
    talbe, td{
        font-size:19px;
    }
</style>
<table>
<thead style="background-color: #4CAF50;color=white;">
	<tr>
    	<td colspan="2">Layer</td>
        <td>Net</td>
        <td># of Parameters</td>
	<td>Output Volume</td>
	</tr>
	    </thead>
	<tr>
	<td colspan="2">Input</td>
	<td>Data 1 x 32 x 32</td>
	<td></td>
	<td></td>
    </tr>


    <tr>
    <td rowspan="2">Layer 1</td>
    <td>C1</td>
    <td>Convolution : 6 x 5 x 5, Stride = 1</td>
    <td>(1x5x5+1)x6=55</td>
    <td>(32-5)/1+1=28 &#8594; 28x28x6</td>
    </tr>
    <tr>
    <td>S2</td>
    <td>Pooling-Max, Kernel size=2, Stride=2</td>
    <td>0</td>
    <td>(28-2)/2+1=14 &#8594; 14x14x6</td>
    </tr>

    <tr>
    <td rowspan="2">Layer 2</td>
    <td>C3</td>
    <td>Convolution : 16 x 5 x 5, Stride=1</td>
    <td>(6x5x5+1)x16=2416</td>
    <td>(14-5)/1+1=10 &#8594; 10x10x16</td>
    </tr>
    <tr>
    <td>S2</td>
    <td>Pooling-Max, Kernel size=2, Stride=2</td>
    <td>0</td>
    <td>(10-2)/2+1=5 &#8594; 5x5x16</td>
    </tr>

    <tr>
    <td>Layer 3</td>
    <td>C5</td>
    <td>Inner Product : output=120</td>
    <td>(16x5x5+1)x120=48,120</td>
    <td>120</td>
    </tr>
    
    <tr>
    <td>Layer 4</td>
    <td>F6</td>
    <td>Inner Product : output=84</td>
    <td>(120+1)x84=10,164</td>
    <td>84</td>
    </tr>
    
    <tr>
    <td>Layer 5</td>
    <td>Output</td>
    <td>Inner Product : output=10</td>
    <td>(84+1)x10=850</td>
    <td>10</td>
    </tr>

</table>


