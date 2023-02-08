##### Forked from https://github.com/tensorflow/examples

# To run on linux:

### Check your Python version. You should have Python 3.7 or later.
python3 --version

### Install virtualenv and upgrade pip.
python3 -m pip install --user --upgrade pip
python3 -m pip install --user virtualenv

### Create a Python virtual environment for the TFLite samples (optional but strongly recommended)
python3 -m venv ~/tflite

### Run this command whenever you open a new Terminal window/tab to activate the environment.
source ~/tflite/bin/activate

### Clone the TensorFlow example repository with the TFLite Raspberry Pi samples.
git clone https://github.com/tensorflow/examples.git
cd examples/lite/examples/object_detection/raspberry_pi

### Install dependencies required by the sample
sh setup.sh

### Run the object detection sample
*IMPORTANT: If you SSH to the Pi, make sure that:*
*1. There is a display connected to the Pi.*
*2. Run `export DISPLAY=:0` before proceed to make the object_detection window appear on the display*
python detect.py


*If you see an error running the sample: *
*ImportError: libcblas.so.3: cannot open shared object file: No such file or directory *
*you can fix it by installing an OpenCV dependency that is missing on your Raspberry Pi. *
sudo apt-get install libatlas-base-dev





# TensorFlow Examples

<div align="center">
  <img src="https://www.tensorflow.org/images/tf_logo_social.png" /><br /><br />
</div>

<h2>Most important links!</h2>

* [Community examples](./community)
* [Course materials](./courses/udacity_deep_learning) for the [Deep Learning](https://www.udacity.com/course/deep-learning--ud730) class on Udacity

If you are looking to learn TensorFlow, don't miss the
[core TensorFlow documentation](http://github.com/tensorflow/docs)
which is largely runnable code.
Those notebooks can be opened in Colab from
[tensorflow.org](https://tensorflow.org).

<h2>What is this repo?</h2>

This is the TensorFlow example repo.  It has several classes of material:

* Showcase examples and documentation for our fantastic [TensorFlow Community](https://tensorflow.org/community)
* Provide examples mentioned on TensorFlow.org
* Publish material supporting official TensorFlow courses
* Publish supporting material for the [TensorFlow Blog](https://blog.tensorflow.org) and [TensorFlow YouTube Channel](https://youtube.com/tensorflow)

We welcome community contributions, see [CONTRIBUTING.md](CONTRIBUTING.md) and, for style help,
[Writing TensorFlow documentation](https://www.tensorflow.org/community/contribute/docs_style)
guide.

To file an issue, use the tracker in the
[tensorflow/tensorflow](https://github.com/tensorflow/tensorflow/issues/new?template=20-documentation-issue.md) repo.

## License

[Apache License 2.0](LICENSE)
