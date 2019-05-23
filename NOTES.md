pip install --upgrade tensorflow==1.13.1 \
  numpy pandas matplotlib Pillow scipy sklearn

###########

(env) Brunos-MBP:tensorflow-svhn bambrozi$ pip install --upgrade tensorflow==1.13.1 \
>   numpy pandas matplotlib PillowDEPRECATION: Python 2.7 will reach the end of its life on January 1st, 2020. Please upgrade your Python as Python 2.7 won't be maintained after that date. A future version of pip will drop support for Python 2.7.
Collecting tensorflow==1.13.1
  Using cached https://files.pythonhosted.org/packages/89/33/8617196404b6bbdd7d8a4c4fad0a2b28c81cfdb63786ce70800778d8e72d/tensorflow-1.13.1-cp27-cp27m-macosx_10_11_x86_64.whl
Collecting numpy
  Using cached https://files.pythonhosted.org/packages/6e/36/e8369aa628b29f50211ba82daec31cc110f6627feca160bc11b0e4ee1191/numpy-1.16.3-cp27-cp27m-macosx_10_6_intel.macosx_10_9_intel.macosx_10_9_x86_64.macosx_10_10_intel.macosx_10
(env) Brunos-MBP:tensorflow-svhn bambrozi$ python train_classifier.py
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/lib/python2.7/site-packages/tensorflow/python/framework/op_def_library.py:263: colocate_with (from tensorflow.python.framework.ops) is dep
recated and will be removed in a future version.
Instructions for updating:
Colocations handled automatically by placer.
Starting without Saved Weights.
Training (65931, 32, 32, 3)
Valid (7326, 32, 32, 3)
Test (26032, 32, 32, 3)
Using drop out
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/svhn_model.py:123: calling dropout (from tensorflow.python.ops.nn_ops) with keep_prob is deprecated and will be removed in a future version.
Instructions for updating:
Please use `rate` instead of `keep_prob`. Rate should be set to `rate = 1 - keep_prob`.
WARNING:tensorflow:From train_classifier.py:73: softmax_cross_entropy_with_logits (from tensorflow.python.ops.nn_ops) is deprecated and will be removed in a future version.
Instructions for updating:
Future major versions of TensorFlow will allow gradients to flow
into the labels input on backprop by default.

See `tf.nn.softmax_cross_entropy_with_logits_v2`.

Not using dropout
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/lib/python2.7/site-packages/tensorflow/python/util/tf_should_use.py:193: initialize_all_variables (from tensorflow.python.ops.variables) i
s deprecated and will be removed after 2017-03-02.
Instructions for updating:
Use `tf.global_variables_initializer` instead.
2019-05-23 00:58:48.399170: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2 FMA
Validation Accuracy: 0.11%
Training Accuracy: 0.13%
Adding run metadata for 0
2019-05-23 00:58:50.035467: step 0, loss = 2.29  learning rate = 0.075000  (322.9 examples/sec; 0.79 sec/batch)
Mini-Batch Accuracy: 0.08%
2019-05-23 00:59:24.141655: step 100, loss = 1.94  learning rate = 0.075000  (7.5 examples/sec; 34.11 sec/batch)
Mini-Batch Accuracy: 0.35%
2019-05-23 00:59:58.749781: step 200, loss = 1.09  learning rate = 0.075000  (7.4 examples/sec; 34.61 sec/batch)
Mini-Batch Accuracy: 0.66%
2019-05-23 01:00:32.921624: step 300, loss = 0.77  learning rate = 0.071250  (7.5 examples/sec; 34.17 sec/batch)
Mini-Batch Accuracy: 0.77%
2019-05-23 01:01:10.433431: step 400, loss = 0.49  learning rate = 0.071250  (6.8 examples/sec; 37.51 sec/batch)
Mini-Batch Accuracy: 0.87%
2019-05-23 01:01:46.349760: step 500, loss = 0.41  learning rate = 0.071250  (7.1 examples/sec; 35.92 sec/batch)
Mini-Batch Accuracy: 0.87%
2019-05-23 01:02:20.674102: step 600, loss = 0.47  learning rate = 0.067688  (7.5 examples/sec; 34.32 sec/batch)
Mini-Batch Accuracy: 0.82%
2019-05-23 01:02:53.353489: step 700, loss = 0.33  learning rate = 0.067688  (7.8 examples/sec; 32.68 sec/batch)
Mini-Batch Accuracy: 0.91%
2019-05-23 01:03:28.132612: step 800, loss = 0.47  learning rate = 0.064303  (7.4 examples/sec; 34.78 sec/batch)
Mini-Batch Accuracy: 0.88%
2019-05-23 01:04:02.461278: step 900, loss = 0.37  learning rate = 0.064303  (7.5 examples/sec; 34.33 sec/batch)
Mini-Batch Accuracy: 0.88%
Validation Accuracy: 0.87%
Training Accuracy: 0.92%
Adding run metadata for 1000
2019-05-23 01:04:40.560039: step 1000, loss = 0.32  learning rate = 0.064303  (6.9 examples/sec; 37.27 sec/batch)
Mini-Batch Accuracy: 0.88%
2019-05-23 01:05:18.786477: step 1100, loss = 0.30  learning rate = 0.061088  (6.7 examples/sec; 38.23 sec/batch)
Mini-Batch Accuracy: 0.91%
2019-05-23 01:05:55.370910: step 1200, loss = 0.26  learning rate = 0.061088  (7.0 examples/sec; 36.58 sec/batch)
Mini-Batch Accuracy: 0.94%
2019-05-23 01:06:30.106125: step 1300, loss = 0.34  learning rate = 0.058034  (7.4 examples/sec; 34.74 sec/batch)
Mini-Batch Accuracy: 0.91%
2019-05-23 01:07:04.586483: step 1400, loss = 0.38  learning rate = 0.058034  (7.4 examples/sec; 34.48 sec/batch)
Mini-Batch Accuracy: 0.87%
2019-05-23 01:07:37.857881: step 1500, loss = 0.34  learning rate = 0.058034  (7.7 examples/sec; 33.27 sec/batch)
Mini-Batch Accuracy: 0.91%
2019-05-23 01:08:10.056080: step 1600, loss = 0.27  learning rate = 0.055132  (8.0 examples/sec; 32.20 sec/batch)
Mini-Batch Accuracy: 0.91%
2019-05-23 01:08:42.341268: step 1700, loss = 0.27  learning rate = 0.055132  (7.9 examples/sec; 32.29 sec/batch)
Mini-Batch Accuracy: 0.92%
2019-05-23 01:09:16.428302: step 1800, loss = 0.28  learning rate = 0.052375  (7.5 examples/sec; 34.09 sec/batch)
Mini-Batch Accuracy: 0.91%
2019-05-23 01:09:51.090230: step 1900, loss = 0.31  learning rate = 0.052375  (7.4 examples/sec; 34.66 sec/batch)
Mini-Batch Accuracy: 0.92%
Validation Accuracy: 0.91%
Training Accuracy: 0.96%
Adding run metadata for 2000
2019-05-23 01:10:26.382155: step 2000, loss = 0.17  learning rate = 0.052375  (7.4 examples/sec; 34.63 sec/batch)
Mini-Batch Accuracy: 0.93%
2019-05-23 01:10:56.760287: step 2100, loss = 0.22  learning rate = 0.049757  (8.4 examples/sec; 30.38 sec/batch)
Mini-Batch Accuracy: 0.96%
2019-05-23 01:11:33.169061: step 2200, loss = 0.24  learning rate = 0.049757  (7.0 examples/sec; 36.41 sec/batch)
Mini-Batch Accuracy: 0.93%
2019-05-23 01:12:11.064996: step 2300, loss = 0.30  learning rate = 0.049757  (6.8 examples/sec; 37.90 sec/batch)
Mini-Batch Accuracy: 0.92%
2019-05-23 01:12:43.340417: step 2400, loss = 0.34  learning rate = 0.047269  (7.9 examples/sec; 32.28 sec/batch)
Mini-Batch Accuracy: 0.91%
2019-05-23 01:13:15.177265: step 2500, loss = 0.28  learning rate = 0.047269  (8.0 examples/sec; 31.84 sec/batch)
Mini-Batch Accuracy: 0.93%






















2019-05-23 01:13:47.145554: step 2600, loss = 0.36  learning rate = 0.044905  (8.0 examples/sec; 31.97 sec/batch)
Mini-Batch Accuracy: 0.91%
2019-05-23 01:14:16.997304: step 2700, loss = 0.22  learning rate = 0.044905  (8.6 examples/sec; 29.85 sec/batch)
Mini-Batch Accuracy: 0.94%
2019-05-23 01:14:46.695159: step 2800, loss = 0.23  learning rate = 0.044905  (8.6 examples/sec; 29.70 sec/batch)
Mini-Batch Accuracy: 0.96%
2019-05-23 01:15:17.083202: step 2900, loss = 0.29  learning rate = 0.042660  (8.4 examples/sec; 30.39 sec/batch)
Mini-Batch Accuracy: 0.94%
Validation Accuracy: 0.89%
Training Accuracy: 0.98%
Adding run metadata for 3000
2019-05-23 01:15:47.233616: step 3000, loss = 0.13  learning rate = 0.042660  (8.7 examples/sec; 29.54 sec/batch)
Mini-Batch Accuracy: 0.95%
2019-05-23 01:16:17.095223: step 3100, loss = 0.28  learning rate = 0.040527  (8.6 examples/sec; 29.86 sec/batch)
Mini-Batch Accuracy: 0.92%
2019-05-23 01:16:48.517251: step 3200, loss = 0.15  learning rate = 0.040527  (8.1 examples/sec; 31.42 sec/batch)
Mini-Batch Accuracy: 0.97%
2019-05-23 01:17:19.860757: step 3300, loss = 0.16  learning rate = 0.040527  (8.2 examples/sec; 31.34 sec/batch)
Mini-Batch Accuracy: 0.97%
2019-05-23 01:17:49.166855: step 3400, loss = 0.18  learning rate = 0.038501  (8.7 examples/sec; 29.31 sec/batch)
Mini-Batch Accuracy: 0.95%
2019-05-23 01:18:18.438666: step 3500, loss = 0.23  learning rate = 0.038501  (8.7 examples/sec; 29.27 sec/batch)
Mini-Batch Accuracy: 0.94%
2019-05-23 01:18:47.696493: step 3600, loss = 0.22  learning rate = 0.036576  (8.7 examples/sec; 29.26 sec/batch)
Mini-Batch Accuracy: 0.95%
2019-05-23 01:19:17.105782: step 3700, loss = 0.17  learning rate = 0.036576  (8.7 examples/sec; 29.41 sec/batch)
Mini-Batch Accuracy: 0.96%
2019-05-23 01:19:46.465107: step 3800, loss = 0.12  learning rate = 0.036576  (8.7 examples/sec; 29.36 sec/batch)
Mini-Batch Accuracy: 0.97%
2019-05-23 01:20:16.641995: step 3900, loss = 0.19  learning rate = 0.034747  (8.5 examples/sec; 30.18 sec/batch)
Mini-Batch Accuracy: 0.95%
Validation Accuracy: 0.93%
Training Accuracy: 0.98%
Adding run metadata for 4000
2019-05-23 01:20:46.433759: step 4000, loss = 0.12  learning rate = 0.034747  (8.8 examples/sec; 29.17 sec/batch)
Mini-Batch Accuracy: 0.96%
2019-05-23 01:21:16.098055: step 4100, loss = 0.19  learning rate = 0.034747  (8.6 examples/sec; 29.66 sec/batch)
Mini-Batch Accuracy: 0.96%
2019-05-23 01:21:45.516338: step 4200, loss = 0.25  learning rate = 0.033009  (8.7 examples/sec; 29.42 sec/batch)
Mini-Batch Accuracy: 0.95%
2019-05-23 01:22:15.274831: step 4300, loss = 0.18  learning rate = 0.033009  (8.6 examples/sec; 29.76 sec/batch)
Mini-Batch Accuracy: 0.95%
2019-05-23 01:22:44.726336: step 4400, loss = 0.17  learning rate = 0.031359  (8.7 examples/sec; 29.45 sec/batch)
Mini-Batch Accuracy: 0.97%
2019-05-23 01:23:14.031946: step 4500, loss = 0.19  learning rate = 0.031359  (8.7 examples/sec; 29.31 sec/batch)
Mini-Batch Accuracy: 0.96%
2019-05-23 01:23:43.403140: step 4600, loss = 0.11  learning rate = 0.031359  (8.7 examples/sec; 29.37 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:24:12.852355: step 4700, loss = 0.15  learning rate = 0.029791  (8.7 examples/sec; 29.45 sec/batch)
Mini-Batch Accuracy: 0.96%
2019-05-23 01:24:42.106840: step 4800, loss = 0.19  learning rate = 0.029791  (8.8 examples/sec; 29.25 sec/batch)
Mini-Batch Accuracy: 0.94%
2019-05-23 01:25:12.109156: step 4900, loss = 0.12  learning rate = 0.028302  (8.5 examples/sec; 30.00 sec/batch)
Mini-Batch Accuracy: 0.97%
Validation Accuracy: 0.90%
Training Accuracy: 0.98%
Adding run metadata for 5000
2019-05-23 01:25:42.250653: step 5000, loss = 0.13  learning rate = 0.028302  (8.7 examples/sec; 29.53 sec/batch)
Mini-Batch Accuracy: 0.96%
2019-05-23 01:26:11.661260: step 5100, loss = 0.14  learning rate = 0.028302  (8.7 examples/sec; 29.41 sec/batch)
Mini-Batch Accuracy: 0.97%
2019-05-23 01:26:40.905419: step 5200, loss = 0.17  learning rate = 0.026886  (8.8 examples/sec; 29.24 sec/batch)
Mini-Batch Accuracy: 0.97%
2019-05-23 01:27:10.544936: step 5300, loss = 0.09  learning rate = 0.026886  (8.6 examples/sec; 29.64 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:27:40.020453: step 5400, loss = 0.14  learning rate = 0.025542  (8.7 examples/sec; 29.48 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:28:09.468081: step 5500, loss = 0.11  learning rate = 0.025542  (8.7 examples/sec; 29.45 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:28:38.721818: step 5600, loss = 0.13  learning rate = 0.025542  (8.8 examples/sec; 29.25 sec/batch)
Mini-Batch Accuracy: 0.97%
2019-05-23 01:29:08.167333: step 5700, loss = 0.10  learning rate = 0.024265  (8.7 examples/sec; 29.45 sec/batch)
Mini-Batch Accuracy: 0.97%
2019-05-23 01:29:37.641309: step 5800, loss = 0.20  learning rate = 0.024265  (8.7 examples/sec; 29.47 sec/batch)
Mini-Batch Accuracy: 0.96%
2019-05-23 01:30:07.086397: step 5900, loss = 0.14  learning rate = 0.024265  (8.7 examples/sec; 29.45 sec/batch)
Mini-Batch Accuracy: 0.98%
Validation Accuracy: 0.91%
Training Accuracy: 0.98%
Adding run metadata for 6000
2019-05-23 01:30:37.890883: step 6000, loss = 0.10  learning rate = 0.023052  (8.5 examples/sec; 30.19 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:31:07.446948: step 6100, loss = 0.14  learning rate = 0.023052  (8.7 examples/sec; 29.56 sec/batch)
Mini-Batch Accuracy: 0.97%
2019-05-23 01:31:37.243379: step 6200, loss = 0.14  learning rate = 0.021899  (8.6 examples/sec; 29.80 sec/batch)
Mini-Batch Accuracy: 0.97%
2019-05-23 01:32:07.003581: step 6300, loss = 0.08  learning rate = 0.021899  (8.6 examples/sec; 29.76 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:32:36.306612: step 6400, loss = 0.09  learning rate = 0.021899  (8.7 examples/sec; 29.30 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:33:05.445748: step 6500, loss = 0.10  learning rate = 0.020804  (8.8 examples/sec; 29.14 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:33:34.399029: step 6600, loss = 0.15  learning rate = 0.020804  (8.8 examples/sec; 28.95 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:34:03.634238: step 6700, loss = 0.15  learning rate = 0.019764  (8.8 examples/sec; 29.24 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:34:32.980310: step 6800, loss = 0.16  learning rate = 0.019764  (8.7 examples/sec; 29.35 sec/batch)
Mini-Batch Accuracy: 0.97%
2019-05-23 01:35:02.095408: step 6900, loss = 0.11  learning rate = 0.019764  (8.8 examples/sec; 29.12 sec/batch)
Mini-Batch Accuracy: 0.99%
Validation Accuracy: 0.92%
Training Accuracy: 0.98%
Adding run metadata for 7000
2019-05-23 01:35:32.472773: step 7000, loss = 0.08  learning rate = 0.018776  (8.6 examples/sec; 29.78 sec/batch)
Mini-Batch Accuracy: 0.97%
2019-05-23 01:36:01.633476: step 7100, loss = 0.11  learning rate = 0.018776  (8.8 examples/sec; 29.16 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:36:30.925272: step 7200, loss = 0.07  learning rate = 0.017837  (8.7 examples/sec; 29.29 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:37:00.214997: step 7300, loss = 0.11  learning rate = 0.017837  (8.7 examples/sec; 29.29 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:37:29.287567: step 7400, loss = 0.13  learning rate = 0.017837  (8.8 examples/sec; 29.07 sec/batch)
Mini-Batch Accuracy: 0.97%
2019-05-23 01:37:58.456443: step 7500, loss = 0.12  learning rate = 0.016945  (8.8 examples/sec; 29.17 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:38:27.519920: step 7600, loss = 0.07  learning rate = 0.016945  (8.8 examples/sec; 29.06 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:38:56.709101: step 7700, loss = 0.12  learning rate = 0.016945  (8.8 examples/sec; 29.19 sec/batch)
Mini-Batch Accuracy: 0.97%
2019-05-23 01:39:25.979193: step 7800, loss = 0.09  learning rate = 0.016098  (8.7 examples/sec; 29.27 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:39:55.228010: step 7900, loss = 0.05  learning rate = 0.016098  (8.8 examples/sec; 29.25 sec/batch)
Mini-Batch Accuracy: 1.00%
Validation Accuracy: 0.91%
Training Accuracy: 1.00%
Adding run metadata for 8000
2019-05-23 01:40:25.939409: step 8000, loss = 0.06  learning rate = 0.015293  (8.5 examples/sec; 30.07 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 01:40:55.242390: step 8100, loss = 0.05  learning rate = 0.015293  (8.7 examples/sec; 29.30 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 01:41:24.788752: step 8200, loss = 0.09  learning rate = 0.015293  (8.7 examples/sec; 29.55 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:41:54.221749: step 8300, loss = 0.06  learning rate = 0.014528  (8.7 examples/sec; 29.43 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:42:23.694162: step 8400, loss = 0.12  learning rate = 0.014528  (8.7 examples/sec; 29.47 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:42:52.922264: step 8500, loss = 0.10  learning rate = 0.013802  (8.8 examples/sec; 29.23 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:43:22.093350: step 8600, loss = 0.08  learning rate = 0.013802  (8.8 examples/sec; 29.17 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:43:51.996254: step 8700, loss = 0.18  learning rate = 0.013802  (8.6 examples/sec; 29.90 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:44:21.517219: step 8800, loss = 0.08  learning rate = 0.013112  (8.7 examples/sec; 29.52 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 01:44:50.870254: step 8900, loss = 0.08  learning rate = 0.013112  (8.7 examples/sec; 29.35 sec/batch)
Mini-Batch Accuracy: 0.99%
Validation Accuracy: 0.90%
Training Accuracy: 0.98%
Adding run metadata for 9000
2019-05-23 01:45:21.563447: step 9000, loss = 0.08  learning rate = 0.012456  (8.5 examples/sec; 30.09 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:45:51.036308: step 9100, loss = 0.03  learning rate = 0.012456  (8.7 examples/sec; 29.47 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 01:46:20.638846: step 9200, loss = 0.08  learning rate = 0.012456  (8.6 examples/sec; 29.60 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:46:50.103432: step 9300, loss = 0.10  learning rate = 0.011833  (8.7 examples/sec; 29.46 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:47:19.431665: step 9400, loss = 0.14  learning rate = 0.011833  (8.7 examples/sec; 29.33 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:47:48.928605: step 9500, loss = 0.07  learning rate = 0.011833  (8.7 examples/sec; 29.50 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 01:48:18.161185: step 9600, loss = 0.06  learning rate = 0.011242  (8.8 examples/sec; 29.23 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:48:47.405938: step 9700, loss = 0.06  learning rate = 0.011242  (8.8 examples/sec; 29.24 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 01:49:16.812382: step 9800, loss = 0.04  learning rate = 0.010680  (8.7 examples/sec; 29.41 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 01:49:46.067552: step 9900, loss = 0.08  learning rate = 0.010680  (8.8 examples/sec; 29.26 sec/batch)
Mini-Batch Accuracy: 0.99%
Validation Accuracy: 0.88%
Training Accuracy: 1.00%
Adding run metadata for 10000
2019-05-23 01:50:16.730178: step 10000, loss = 0.06  learning rate = 0.010680  (8.5 examples/sec; 30.02 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 01:50:46.115018: step 10100, loss = 0.12  learning rate = 0.010146  (8.7 examples/sec; 29.38 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:51:16.708447: step 10200, loss = 0.10  learning rate = 0.010146  (8.4 examples/sec; 30.59 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:51:46.428015: step 10300, loss = 0.07  learning rate = 0.009638  (8.6 examples/sec; 29.72 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:52:16.349093: step 10400, loss = 0.07  learning rate = 0.009638  (8.6 examples/sec; 29.92 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:52:45.968465: step 10500, loss = 0.08  learning rate = 0.009638  (8.6 examples/sec; 29.62 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:53:15.691622: step 10600, loss = 0.07  learning rate = 0.009156  (8.6 examples/sec; 29.72 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 01:53:45.515879: step 10700, loss = 0.06  learning rate = 0.009156  (8.6 examples/sec; 29.82 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:54:15.297556: step 10800, loss = 0.07  learning rate = 0.008699  (8.6 examples/sec; 29.78 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:54:44.974395: step 10900, loss = 0.06  learning rate = 0.008699  (8.6 examples/sec; 29.68 sec/batch)
Mini-Batch Accuracy: 0.99%
Validation Accuracy: 0.91%
Training Accuracy: 0.99%
Adding run metadata for 11000
2019-05-23 01:55:15.883733: step 11000, loss = 0.06  learning rate = 0.008699  (8.5 examples/sec; 30.29 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:55:45.631563: step 11100, loss = 0.07  learning rate = 0.008264  (8.6 examples/sec; 29.75 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:56:15.387920: step 11200, loss = 0.05  learning rate = 0.008264  (8.6 examples/sec; 29.76 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 01:56:45.210619: step 11300, loss = 0.05  learning rate = 0.008264  (8.6 examples/sec; 29.82 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 01:57:14.965912: step 11400, loss = 0.06  learning rate = 0.007851  (8.6 examples/sec; 29.76 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 01:57:44.495941: step 11500, loss = 0.08  learning rate = 0.007851  (8.7 examples/sec; 29.53 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:58:14.026155: step 11600, loss = 0.08  learning rate = 0.007458  (8.7 examples/sec; 29.53 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 01:58:43.663638: step 11700, loss = 0.14  learning rate = 0.007458  (8.6 examples/sec; 29.64 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 01:59:13.342391: step 11800, loss = 0.07  learning rate = 0.007458  (8.6 examples/sec; 29.68 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 01:59:42.868446: step 11900, loss = 0.07  learning rate = 0.007085  (8.7 examples/sec; 29.53 sec/batch)
Mini-Batch Accuracy: 1.00%
Validation Accuracy: 0.89%
Training Accuracy: 1.00%
Adding run metadata for 12000
2019-05-23 02:00:13.497531: step 12000, loss = 0.06  learning rate = 0.007085  (8.5 examples/sec; 29.99 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:00:43.294361: step 12100, loss = 0.08  learning rate = 0.006731  (8.6 examples/sec; 29.80 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:01:12.960263: step 12200, loss = 0.07  learning rate = 0.006731  (8.6 examples/sec; 29.67 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:01:42.652412: step 12300, loss = 0.12  learning rate = 0.006731  (8.6 examples/sec; 29.69 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:02:12.480315: step 12400, loss = 0.07  learning rate = 0.006394  (8.6 examples/sec; 29.83 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:02:42.138960: step 12500, loss = 0.07  learning rate = 0.006394  (8.6 examples/sec; 29.66 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:03:11.839187: step 12600, loss = 0.05  learning rate = 0.006075  (8.6 examples/sec; 29.70 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:03:41.270168: step 12700, loss = 0.15  learning rate = 0.006075  (8.7 examples/sec; 29.43 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:04:11.082783: step 12800, loss = 0.07  learning rate = 0.006075  (8.6 examples/sec; 29.81 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:04:40.922369: step 12900, loss = 0.09  learning rate = 0.005771  (8.6 examples/sec; 29.84 sec/batch)
Mini-Batch Accuracy: 0.99%
Validation Accuracy: 0.95%
Training Accuracy: 0.98%
Adding run metadata for 13000
2019-05-23 02:05:11.585647: step 13000, loss = 0.10  learning rate = 0.005771  (8.5 examples/sec; 30.03 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 02:05:41.502029: step 13100, loss = 0.05  learning rate = 0.005771  (8.6 examples/sec; 29.92 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:06:11.206519: step 13200, loss = 0.09  learning rate = 0.005482  (8.6 examples/sec; 29.70 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:06:41.027438: step 13300, loss = 0.06  learning rate = 0.005482  (8.6 examples/sec; 29.82 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:07:10.986659: step 13400, loss = 0.10  learning rate = 0.005208  (8.5 examples/sec; 29.96 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:07:40.735278: step 13500, loss = 0.06  learning rate = 0.005208  (8.6 examples/sec; 29.75 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:08:10.455583: step 13600, loss = 0.08  learning rate = 0.005208  (8.6 examples/sec; 29.72 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:08:40.256426: step 13700, loss = 0.06  learning rate = 0.004948  (8.6 examples/sec; 29.80 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:09:09.965179: step 13800, loss = 0.04  learning rate = 0.004948  (8.6 examples/sec; 29.71 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:09:39.801866: step 13900, loss = 0.04  learning rate = 0.004700  (8.6 examples/sec; 29.84 sec/batch)
Mini-Batch Accuracy: 1.00%
Validation Accuracy: 0.91%
Training Accuracy: 1.00%
Adding run metadata for 14000
2019-05-23 02:10:10.381863: step 14000, loss = 0.07  learning rate = 0.004700  (8.6 examples/sec; 29.94 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:10:40.289339: step 14100, loss = 0.05  learning rate = 0.004700  (8.6 examples/sec; 29.91 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:11:10.053627: step 14200, loss = 0.04  learning rate = 0.004465  (8.6 examples/sec; 29.76 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:11:39.976063: step 14300, loss = 0.05  learning rate = 0.004465  (8.6 examples/sec; 29.92 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:12:10.098444: step 14400, loss = 0.05  learning rate = 0.004242  (8.5 examples/sec; 30.12 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:12:39.835471: step 14500, loss = 0.06  learning rate = 0.004242  (8.6 examples/sec; 29.74 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:13:09.580312: step 14600, loss = 0.10  learning rate = 0.004242  (8.6 examples/sec; 29.74 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 02:13:39.229524: step 14700, loss = 0.05  learning rate = 0.004030  (8.6 examples/sec; 29.65 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:14:08.965333: step 14800, loss = 0.06  learning rate = 0.004030  (8.6 examples/sec; 29.74 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:14:38.897688: step 14900, loss = 0.05  learning rate = 0.004030  (8.6 examples/sec; 29.93 sec/batch)
Mini-Batch Accuracy: 1.00%
Validation Accuracy: 0.90%
Training Accuracy: 1.00%
Adding run metadata for 15000
2019-05-23 02:15:09.745704: step 15000, loss = 0.04  learning rate = 0.003829  (8.5 examples/sec; 30.16 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:15:39.850754: step 15100, loss = 0.08  learning rate = 0.003829  (8.5 examples/sec; 30.11 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:16:09.620019: step 15200, loss = 0.07  learning rate = 0.003637  (8.6 examples/sec; 29.77 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:16:39.580512: step 15300, loss = 0.08  learning rate = 0.003637  (8.5 examples/sec; 29.96 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:17:09.601661: step 15400, loss = 0.04  learning rate = 0.003637  (8.5 examples/sec; 30.02 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:17:39.303306: step 15500, loss = 0.04  learning rate = 0.003455  (8.6 examples/sec; 29.70 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:18:09.021201: step 15600, loss = 0.06  learning rate = 0.003455  (8.6 examples/sec; 29.72 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:18:38.749379: step 15700, loss = 0.04  learning rate = 0.003282  (8.6 examples/sec; 29.73 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:19:08.489273: step 15800, loss = 0.08  learning rate = 0.003282  (8.6 examples/sec; 29.74 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:19:38.247054: step 15900, loss = 0.03  learning rate = 0.003282  (8.6 examples/sec; 29.76 sec/batch)
Mini-Batch Accuracy: 1.00%
Validation Accuracy: 0.92%
Training Accuracy: 1.00%
Adding run metadata for 16000
2019-05-23 02:20:08.802287: step 16000, loss = 0.04  learning rate = 0.003118  (8.6 examples/sec; 29.87 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:20:38.989094: step 16100, loss = 0.07  learning rate = 0.003118  (8.5 examples/sec; 30.19 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:21:08.848399: step 16200, loss = 0.10  learning rate = 0.002962  (8.6 examples/sec; 29.86 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:21:38.753333: step 16300, loss = 0.09  learning rate = 0.002962  (8.6 examples/sec; 29.90 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:22:08.708614: step 16400, loss = 0.08  learning rate = 0.002962  (8.5 examples/sec; 29.96 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:22:38.460507: step 16500, loss = 0.05  learning rate = 0.002814  (8.6 examples/sec; 29.75 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:23:08.304454: step 16600, loss = 0.06  learning rate = 0.002814  (8.6 examples/sec; 29.84 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:23:38.039252: step 16700, loss = 0.08  learning rate = 0.002814  (8.6 examples/sec; 29.73 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:24:07.778310: step 16800, loss = 0.05  learning rate = 0.002674  (8.6 examples/sec; 29.74 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:24:37.660804: step 16900, loss = 0.06  learning rate = 0.002674  (8.6 examples/sec; 29.88 sec/batch)
Mini-Batch Accuracy: 1.00%
Validation Accuracy: 0.93%
Training Accuracy: 1.00%
Adding run metadata for 17000
2019-05-23 02:25:08.281562: step 17000, loss = 0.05  learning rate = 0.002540  (8.5 examples/sec; 29.97 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:25:38.512634: step 17100, loss = 0.07  learning rate = 0.002540  (8.5 examples/sec; 30.23 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:26:08.388620: step 17200, loss = 0.10  learning rate = 0.002540  (8.6 examples/sec; 29.88 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:26:38.477907: step 17300, loss = 0.04  learning rate = 0.002413  (8.5 examples/sec; 30.09 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:27:08.597993: step 17400, loss = 0.04  learning rate = 0.002413  (8.5 examples/sec; 30.12 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:27:38.535510: step 17500, loss = 0.05  learning rate = 0.002292  (8.6 examples/sec; 29.94 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:28:08.529529: step 17600, loss = 0.07  learning rate = 0.002292  (8.5 examples/sec; 29.99 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:28:38.362559: step 17700, loss = 0.09  learning rate = 0.002292  (8.6 examples/sec; 29.83 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:29:08.284480: step 17800, loss = 0.05  learning rate = 0.002178  (8.6 examples/sec; 29.92 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:29:38.259079: step 17900, loss = 0.07  learning rate = 0.002178  (8.5 examples/sec; 29.97 sec/batch)
Mini-Batch Accuracy: 1.00%
Validation Accuracy: 0.90%
Training Accuracy: 0.99%
Adding run metadata for 18000
2019-05-23 02:30:09.071301: step 18000, loss = 0.07  learning rate = 0.002069  (8.5 examples/sec; 30.15 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:30:39.233453: step 18100, loss = 0.06  learning rate = 0.002069  (8.5 examples/sec; 30.16 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:31:09.289946: step 18200, loss = 0.10  learning rate = 0.002069  (8.5 examples/sec; 30.06 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:31:39.349009: step 18300, loss = 0.03  learning rate = 0.001965  (8.5 examples/sec; 30.06 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:32:09.639678: step 18400, loss = 0.05  learning rate = 0.001965  (8.5 examples/sec; 30.29 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:32:39.539485: step 18500, loss = 0.05  learning rate = 0.001965  (8.6 examples/sec; 29.90 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:33:09.436939: step 18600, loss = 0.10  learning rate = 0.001867  (8.6 examples/sec; 29.90 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:33:39.470334: step 18700, loss = 0.04  learning rate = 0.001867  (8.5 examples/sec; 30.03 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:34:09.413945: step 18800, loss = 0.05  learning rate = 0.001774  (8.5 examples/sec; 29.94 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:34:39.384967: step 18900, loss = 0.05  learning rate = 0.001774  (8.5 examples/sec; 29.97 sec/batch)
Mini-Batch Accuracy: 0.99%
Validation Accuracy: 0.89%
Training Accuracy: 0.99%
Adding run metadata for 19000
2019-05-23 02:35:09.884798: step 19000, loss = 0.06  learning rate = 0.001774  (8.6 examples/sec; 29.81 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:35:39.969072: step 19100, loss = 0.07  learning rate = 0.001685  (8.5 examples/sec; 30.08 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:36:09.910524: step 19200, loss = 0.06  learning rate = 0.001685  (8.6 examples/sec; 29.94 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:36:39.880031: step 19300, loss = 0.05  learning rate = 0.001601  (8.5 examples/sec; 29.97 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:37:09.956599: step 19400, loss = 0.05  learning rate = 0.001601  (8.5 examples/sec; 30.08 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:37:39.788633: step 19500, loss = 0.06  learning rate = 0.001601  (8.6 examples/sec; 29.83 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:38:09.669504: step 19600, loss = 0.05  learning rate = 0.001521  (8.6 examples/sec; 29.88 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:38:39.602585: step 19700, loss = 0.05  learning rate = 0.001521  (8.6 examples/sec; 29.93 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:39:09.420919: step 19800, loss = 0.07  learning rate = 0.001445  (8.6 examples/sec; 29.82 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:39:39.393106: step 19900, loss = 0.10  learning rate = 0.001445  (8.5 examples/sec; 29.97 sec/batch)
Mini-Batch Accuracy: 0.99%
Validation Accuracy: 0.92%
Training Accuracy: 1.00%
Adding run metadata for 20000
2019-05-23 02:40:10.271599: step 20000, loss = 0.05  learning rate = 0.001445  (8.5 examples/sec; 30.24 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:40:40.342434: step 20100, loss = 0.06  learning rate = 0.001372  (8.5 examples/sec; 30.07 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:41:10.235697: step 20200, loss = 0.09  learning rate = 0.001372  (8.6 examples/sec; 29.89 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:41:40.207272: step 20300, loss = 0.04  learning rate = 0.001372  (8.5 examples/sec; 29.97 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:42:11.533284: step 20400, loss = 0.04  learning rate = 0.001304  (8.2 examples/sec; 31.33 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:42:41.989937: step 20500, loss = 0.05  learning rate = 0.001304  (8.4 examples/sec; 30.46 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:43:12.192542: step 20600, loss = 0.04  learning rate = 0.001239  (8.5 examples/sec; 30.20 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:43:42.282982: step 20700, loss = 0.04  learning rate = 0.001239  (8.5 examples/sec; 30.09 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:44:12.534461: step 20800, loss = 0.03  learning rate = 0.001239  (8.5 examples/sec; 30.25 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:44:42.937975: step 20900, loss = 0.04  learning rate = 0.001177  (8.4 examples/sec; 30.40 sec/batch)
Mini-Batch Accuracy: 1.00%
Validation Accuracy: 0.92%
Training Accuracy: 1.00%
Adding run metadata for 21000
2019-05-23 02:45:14.359568: step 21000, loss = 0.05  learning rate = 0.001177  (8.3 examples/sec; 30.79 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:45:44.691219: step 21100, loss = 0.06  learning rate = 0.001118  (8.4 examples/sec; 30.33 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:46:15.108970: step 21200, loss = 0.05  learning rate = 0.001118  (8.4 examples/sec; 30.42 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:46:45.670866: step 21300, loss = 0.03  learning rate = 0.001118  (8.4 examples/sec; 30.56 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:47:16.129107: step 21400, loss = 0.04  learning rate = 0.001062  (8.4 examples/sec; 30.46 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:47:46.314054: step 21500, loss = 0.05  learning rate = 0.001062  (8.5 examples/sec; 30.18 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:48:16.457659: step 21600, loss = 0.06  learning rate = 0.001009  (8.5 examples/sec; 30.14 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:48:46.549558: step 21700, loss = 0.05  learning rate = 0.001009  (8.5 examples/sec; 30.09 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:49:16.821921: step 21800, loss = 0.03  learning rate = 0.001009  (8.5 examples/sec; 30.27 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:49:46.976386: step 21900, loss = 0.06  learning rate = 0.000958  (8.5 examples/sec; 30.15 sec/batch)
Mini-Batch Accuracy: 0.99%
Validation Accuracy: 0.90%
Training Accuracy: 1.00%
Adding run metadata for 22000
2019-05-23 02:50:18.191393: step 22000, loss = 0.06  learning rate = 0.000958  (8.4 examples/sec; 30.59 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:50:48.324124: step 22100, loss = 0.07  learning rate = 0.000958  (8.5 examples/sec; 30.13 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:51:18.420427: step 22200, loss = 0.07  learning rate = 0.000911  (8.5 examples/sec; 30.10 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:51:48.823297: step 22300, loss = 0.06  learning rate = 0.000911  (8.4 examples/sec; 30.40 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:52:19.254279: step 22400, loss = 0.08  learning rate = 0.000865  (8.4 examples/sec; 30.43 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:52:49.529834: step 22500, loss = 0.06  learning rate = 0.000865  (8.5 examples/sec; 30.28 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:53:19.731391: step 22600, loss = 0.09  learning rate = 0.000865  (8.5 examples/sec; 30.20 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:53:49.931107: step 22700, loss = 0.05  learning rate = 0.000822  (8.5 examples/sec; 30.20 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:54:20.147974: step 22800, loss = 0.05  learning rate = 0.000822  (8.5 examples/sec; 30.22 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:54:50.361549: step 22900, loss = 0.04  learning rate = 0.000781  (8.5 examples/sec; 30.21 sec/batch)
Mini-Batch Accuracy: 1.00%
Validation Accuracy: 0.93%
Training Accuracy: 0.99%
Adding run metadata for 23000
2019-05-23 02:55:21.637687: step 23000, loss = 0.08  learning rate = 0.000781  (8.3 examples/sec; 30.66 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:55:51.882449: step 23100, loss = 0.10  learning rate = 0.000781  (8.5 examples/sec; 30.24 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:56:22.004800: step 23200, loss = 0.05  learning rate = 0.000742  (8.5 examples/sec; 30.12 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:56:52.405940: step 23300, loss = 0.04  learning rate = 0.000742  (8.4 examples/sec; 30.40 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:57:22.684845: step 23400, loss = 0.08  learning rate = 0.000705  (8.5 examples/sec; 30.28 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 02:57:52.842698: step 23500, loss = 0.04  learning rate = 0.000705  (8.5 examples/sec; 30.16 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:58:22.914634: step 23600, loss = 0.08  learning rate = 0.000705  (8.5 examples/sec; 30.07 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:58:53.021240: step 23700, loss = 0.04  learning rate = 0.000669  (8.5 examples/sec; 30.11 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 02:59:23.116869: step 23800, loss = 0.08  learning rate = 0.000669  (8.5 examples/sec; 30.10 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 02:59:53.302358: step 23900, loss = 0.06  learning rate = 0.000669  (8.5 examples/sec; 30.19 sec/batch)
Mini-Batch Accuracy: 1.00%
Validation Accuracy: 0.89%
Training Accuracy: 1.00%
Adding run metadata for 24000
2019-05-23 03:00:24.529642: step 24000, loss = 0.03  learning rate = 0.000636  (8.4 examples/sec; 30.61 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:00:54.682953: step 24100, loss = 0.12  learning rate = 0.000636  (8.5 examples/sec; 30.15 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:01:24.876628: step 24200, loss = 0.05  learning rate = 0.000604  (8.5 examples/sec; 30.19 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:01:55.539964: step 24300, loss = 0.03  learning rate = 0.000604  (8.3 examples/sec; 30.66 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:02:26.293970: step 24400, loss = 0.05  learning rate = 0.000604  (8.3 examples/sec; 30.75 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:02:56.897473: step 24500, loss = 0.09  learning rate = 0.000574  (8.4 examples/sec; 30.60 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:03:27.086975: step 24600, loss = 0.05  learning rate = 0.000574  (8.5 examples/sec; 30.19 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:03:57.228522: step 24700, loss = 0.08  learning rate = 0.000545  (8.5 examples/sec; 30.14 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:04:27.427582: step 24800, loss = 0.05  learning rate = 0.000545  (8.5 examples/sec; 30.20 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:04:57.730686: step 24900, loss = 0.08  learning rate = 0.000545  (8.4 examples/sec; 30.30 sec/batch)
Mini-Batch Accuracy: 0.99%
Validation Accuracy: 0.91%
Training Accuracy: 1.00%
Adding run metadata for 25000
2019-05-23 03:05:29.005380: step 25000, loss = 0.04  learning rate = 0.000518  (8.4 examples/sec; 30.65 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:05:59.000723: step 25100, loss = 0.04  learning rate = 0.000518  (8.5 examples/sec; 30.00 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:06:29.570835: step 25200, loss = 0.05  learning rate = 0.000492  (8.4 examples/sec; 30.57 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:07:00.011455: step 25300, loss = 0.07  learning rate = 0.000492  (8.4 examples/sec; 30.44 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:07:30.223259: step 25400, loss = 0.04  learning rate = 0.000492  (8.5 examples/sec; 30.21 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:08:00.377444: step 25500, loss = 0.04  learning rate = 0.000467  (8.5 examples/sec; 30.15 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:08:30.515742: step 25600, loss = 0.05  learning rate = 0.000467  (8.5 examples/sec; 30.14 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:09:00.722465: step 25700, loss = 0.07  learning rate = 0.000467  (8.5 examples/sec; 30.21 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:09:30.880043: step 25800, loss = 0.11  learning rate = 0.000444  (8.5 examples/sec; 30.16 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 03:10:01.152495: step 25900, loss = 0.04  learning rate = 0.000444  (8.5 examples/sec; 30.27 sec/batch)
Mini-Batch Accuracy: 1.00%
Validation Accuracy: 0.90%
Training Accuracy: 0.99%
Adding run metadata for 26000
2019-05-23 03:10:32.370644: step 26000, loss = 0.04  learning rate = 0.000422  (8.4 examples/sec; 30.60 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:11:02.636960: step 26100, loss = 0.06  learning rate = 0.000422  (8.5 examples/sec; 30.27 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:11:32.986795: step 26200, loss = 0.06  learning rate = 0.000422  (8.4 examples/sec; 30.35 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:12:03.527506: step 26300, loss = 0.07  learning rate = 0.000401  (8.4 examples/sec; 30.54 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:12:33.905855: step 26400, loss = 0.03  learning rate = 0.000401  (8.4 examples/sec; 30.38 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:13:04.156532: step 26500, loss = 0.04  learning rate = 0.000381  (8.5 examples/sec; 30.25 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:13:34.479939: step 26600, loss = 0.05  learning rate = 0.000381  (8.4 examples/sec; 30.32 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:14:05.023720: step 26700, loss = 0.06  learning rate = 0.000381  (8.4 examples/sec; 30.54 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:14:35.535768: step 26800, loss = 0.04  learning rate = 0.000362  (8.4 examples/sec; 30.51 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:15:06.081219: step 26900, loss = 0.08  learning rate = 0.000362  (8.4 examples/sec; 30.55 sec/batch)
Mini-Batch Accuracy: 0.99%
Validation Accuracy: 0.92%
Training Accuracy: 1.00%
Adding run metadata for 27000
2019-05-23 03:15:37.614929: step 27000, loss = 0.04  learning rate = 0.000344  (8.3 examples/sec; 30.89 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:16:08.083299: step 27100, loss = 0.06  learning rate = 0.000344  (8.4 examples/sec; 30.47 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:16:38.607148: step 27200, loss = 0.05  learning rate = 0.000344  (8.4 examples/sec; 30.52 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:17:09.191180: step 27300, loss = 0.04  learning rate = 0.000326  (8.4 examples/sec; 30.58 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:17:39.430788: step 27400, loss = 0.04  learning rate = 0.000326  (8.5 examples/sec; 30.24 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:18:09.728489: step 27500, loss = 0.08  learning rate = 0.000326  (8.4 examples/sec; 30.30 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:18:39.966205: step 27600, loss = 0.04  learning rate = 0.000310  (8.5 examples/sec; 30.24 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:19:10.229042: step 27700, loss = 0.05  learning rate = 0.000310  (8.5 examples/sec; 30.26 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:19:40.490353: step 27800, loss = 0.05  learning rate = 0.000295  (8.5 examples/sec; 30.26 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:20:11.118728: step 27900, loss = 0.08  learning rate = 0.000295  (8.4 examples/sec; 30.63 sec/batch)
Mini-Batch Accuracy: 0.99%
Validation Accuracy: 0.91%
Training Accuracy: 1.00%
Adding run metadata for 28000
2019-05-23 03:20:42.154679: step 28000, loss = 0.05  learning rate = 0.000295  (8.4 examples/sec; 30.41 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:21:12.408334: step 28100, loss = 0.04  learning rate = 0.000280  (8.5 examples/sec; 30.25 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:21:42.710198: step 28200, loss = 0.06  learning rate = 0.000280  (8.4 examples/sec; 30.30 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:22:13.245800: step 28300, loss = 0.07  learning rate = 0.000266  (8.4 examples/sec; 30.54 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:22:43.536673: step 28400, loss = 0.05  learning rate = 0.000266  (8.5 examples/sec; 30.29 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:23:13.861822: step 28500, loss = 0.07  learning rate = 0.000266  (8.4 examples/sec; 30.33 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:23:44.034930: step 28600, loss = 0.05  learning rate = 0.000253  (8.5 examples/sec; 30.17 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:24:14.269835: step 28700, loss = 0.08  learning rate = 0.000253  (8.5 examples/sec; 30.23 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:24:44.488601: step 28800, loss = 0.03  learning rate = 0.000240  (8.5 examples/sec; 30.22 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:25:15.248861: step 28900, loss = 0.05  learning rate = 0.000240  (8.3 examples/sec; 30.76 sec/batch)
Mini-Batch Accuracy: 0.99%
Validation Accuracy: 0.88%
Training Accuracy: 1.00%
Adding run metadata for 29000
2019-05-23 03:25:46.284606: step 29000, loss = 0.05  learning rate = 0.000240  (8.4 examples/sec; 30.39 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:26:16.477466: step 29100, loss = 0.05  learning rate = 0.000228  (8.5 examples/sec; 30.19 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:26:46.750745: step 29200, loss = 0.07  learning rate = 0.000228  (8.5 examples/sec; 30.27 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:27:17.224060: step 29300, loss = 0.06  learning rate = 0.000217  (8.4 examples/sec; 30.47 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:27:47.578032: step 29400, loss = 0.04  learning rate = 0.000217  (8.4 examples/sec; 30.35 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:28:17.876472: step 29500, loss = 0.04  learning rate = 0.000217  (8.4 examples/sec; 30.30 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:28:48.137350: step 29600, loss = 0.04  learning rate = 0.000206  (8.5 examples/sec; 30.26 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:29:18.490883: step 29700, loss = 0.05  learning rate = 0.000206  (8.4 examples/sec; 30.35 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:29:48.854058: step 29800, loss = 0.04  learning rate = 0.000206  (8.4 examples/sec; 30.36 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:30:19.543860: step 29900, loss = 0.04  learning rate = 0.000195  (8.3 examples/sec; 30.69 sec/batch)
Mini-Batch Accuracy: 0.99%
Validation Accuracy: 0.90%
Training Accuracy: 0.98%
Adding run metadata for 30000
2019-05-23 03:30:50.357628: step 30000, loss = 0.11  learning rate = 0.000195  (8.5 examples/sec; 30.20 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 03:31:20.634730: step 30100, loss = 0.06  learning rate = 0.000186  (8.5 examples/sec; 30.28 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:31:51.220097: step 30200, loss = 0.03  learning rate = 0.000186  (8.4 examples/sec; 30.59 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:32:21.672663: step 30300, loss = 0.05  learning rate = 0.000186  (8.4 examples/sec; 30.45 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:32:51.831090: step 30400, loss = 0.05  learning rate = 0.000176  (8.5 examples/sec; 30.16 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:33:22.025939: step 30500, loss = 0.05  learning rate = 0.000176  (8.5 examples/sec; 30.19 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:33:52.239319: step 30600, loss = 0.05  learning rate = 0.000168  (8.5 examples/sec; 30.21 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:34:22.463706: step 30700, loss = 0.04  learning rate = 0.000168  (8.5 examples/sec; 30.22 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:34:52.702303: step 30800, loss = 0.08  learning rate = 0.000168  (8.5 examples/sec; 30.24 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:35:23.365496: step 30900, loss = 0.03  learning rate = 0.000159  (8.3 examples/sec; 30.66 sec/batch)
Mini-Batch Accuracy: 1.00%
Validation Accuracy: 0.93%
Training Accuracy: 1.00%
Adding run metadata for 31000
2019-05-23 03:35:54.209925: step 31000, loss = 0.04  learning rate = 0.000159  (8.5 examples/sec; 30.22 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:36:24.425783: step 31100, loss = 0.03  learning rate = 0.000151  (8.5 examples/sec; 30.22 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:36:54.805175: step 31200, loss = 0.10  learning rate = 0.000151  (8.4 examples/sec; 30.38 sec/batch)
Mini-Batch Accuracy: 0.98%
2019-05-23 03:37:25.076401: step 31300, loss = 0.04  learning rate = 0.000151  (8.5 examples/sec; 30.27 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:37:55.267784: step 31400, loss = 0.04  learning rate = 0.000144  (8.5 examples/sec; 30.19 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:38:25.462717: step 31500, loss = 0.05  learning rate = 0.000144  (8.5 examples/sec; 30.19 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:38:55.674849: step 31600, loss = 0.03  learning rate = 0.000144  (8.5 examples/sec; 30.21 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:39:25.855139: step 31700, loss = 0.09  learning rate = 0.000136  (8.5 examples/sec; 30.18 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:39:56.087177: step 31800, loss = 0.04  learning rate = 0.000136  (8.5 examples/sec; 30.23 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:40:26.716632: step 31900, loss = 0.07  learning rate = 0.000130  (8.4 examples/sec; 30.63 sec/batch)
Mini-Batch Accuracy: 0.99%
Validation Accuracy: 0.91%
Training Accuracy: 1.00%
Adding run metadata for 32000
2019-05-23 03:40:57.567213: step 32000, loss = 0.04  learning rate = 0.000130  (8.5 examples/sec; 30.23 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:41:27.826679: step 32100, loss = 0.04  learning rate = 0.000130  (8.5 examples/sec; 30.26 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:41:58.377093: step 32200, loss = 0.11  learning rate = 0.000123  (8.4 examples/sec; 30.55 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:42:28.634772: step 32300, loss = 0.05  learning rate = 0.000123  (8.5 examples/sec; 30.26 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:42:58.816347: step 32400, loss = 0.04  learning rate = 0.000117  (8.5 examples/sec; 30.18 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:43:29.212655: step 32500, loss = 0.05  learning rate = 0.000117  (8.4 examples/sec; 30.40 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:43:59.616134: step 32600, loss = 0.05  learning rate = 0.000117  (8.4 examples/sec; 30.40 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:44:30.040928: step 32700, loss = 0.05  learning rate = 0.000111  (8.4 examples/sec; 30.42 sec/batch)
Mini-Batch Accuracy: 1.00%
2019-05-23 03:45:00.519931: step 32800, loss = 0.11  learning rate = 0.000111  (8.4 examples/sec; 30.48 sec/batch)
Mini-Batch Accuracy: 0.99%
2019-05-23 03:45:31.245703: step 32900, loss = 0.05  learning rate = 0.000106  (8.3 examples/sec; 30.73 sec/batch)
Mini-Batch Accuracy: 1.00%
Model saved in file: logs/svhn_classifier_logs/ckpt/classifier.ckpt
Test Accuracy: 0.91797%

(env) Brunos-MBP:tensorflow-svhn bambrozi$ pwd
/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn
(env) Brunos-MBP:tensorflow-svhn bambrozi$ ls -lh
total 280
-rw-r--r--   1 bambrozi  staff    59K 23 May 05:11 NOTES.md
-rwxr-xr-x   1 bambrozi  staff   2.7K 12 May 22:04 README.md
drwxr-xr-x   4 bambrozi  staff   128B 12 May 18:17 data
-rw-r--r--   1 bambrozi  staff   2.1K 12 May 22:20 digit_struct.py
-rw-r--r--   1 bambrozi  staff   3.0K 12 May 22:22 digit_struct.pyc
drwxr-xr-x   6 bambrozi  staff   192B 23 May 00:47 env
drwxr-xr-x  12 bambrozi  staff   384B 23 May 00:58 logs
-rw-r--r--   1 bambrozi  staff   2.7K 22 May 23:48 multi_digit_reader.py
-rw-r--r--   1 bambrozi  staff   9.9K 12 May 22:20 svhn_data.py
-rw-r--r--   1 bambrozi  staff    11K 12 May 22:22 svhn_data.pyc
-rw-r--r--   1 bambrozi  staff   6.1K 12 May 22:20 svhn_model.py
-rw-r--r--   1 bambrozi  staff   5.1K 12 May 22:22 svhn_model.pyc
-rw-r--r--   1 bambrozi  staff   8.6K 23 May 00:15 train_classifier.py
-rw-r--r--   1 bambrozi  staff   9.7K 23 May 00:22 train_regressor.py
(env) Brunos-MBP:tensorflow-svhn bambrozi$ tree logs
logs
├── board_train_writer
│   └── events.out.tfevents.1558569528.Brunos-MBP
├── board_train_writer-0.data-00000-of-00001
├── board_train_writer-0.index
├── board_train_writer-0.meta
├── board_valid_writer
│   └── events.out.tfevents.1558569528.Brunos-MBP
├── board_valid_writer-0.data-00000-of-00001
├── board_valid_writer-0.index
├── board_valid_writer-0.meta
├── checkpoint
└── svhn_classifier_logs
    └── ckpt
        ├── checkpoint
        ├── classifier.ckpt.data-00000-of-00001
        ├── classifier.ckpt.index
        └── classifier.ckpt.meta

4 directories, 13 files
(env) Brunos-MBP:tensorflow-svhn bambrozi$ ls -lh logs/svhn_classifier_logs/ckpt/
total 9128
-rw-r--r--  1 bambrozi  staff   201B 23 May 03:45 checkpoint
-rw-r--r--  1 bambrozi  staff   4.3M 23 May 03:45 classifier.ckpt.data-00000-of-00001
-rw-r--r--  1 bambrozi  staff   1.1K 23 May 03:45 classifier.ckpt.index
-rw-r--r--  1 bambrozi  staff   113K 23 May 03:45 classifier.ckpt.meta

############

(env) Brunos-MBP:tensorflow-svhn bambrozi$ python train_regressor.py 
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/lib/python2.7/site-packages/tensorflow/python/framework/op_def_library.py:263: colocate_with (from tensorflow.python.framework.ops) is dep
recated and will be removed in a future version.
Instructions for updating:
Colocations handled automatically by placer.
Starting without Saved Weights.
TrainData (30061, 64, 64, 3)
Valid Data (3341, 64, 64, 3)
Test Data (13068, 64, 64, 3)
2019-05-23 05:46:12.406726: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2 FMA
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/lib/python2.7/site-packages/tensorflow/python/util/tf_should_use.py:193: initialize_all_variables (from tensorflow.python.ops.variables) i
s deprecated and will be removed after 2017-03-02.
Instructions for updating:
Use `tf.global_variables_initializer` instead.
Model restored.
Validation Accuracy: 0.59
Training Set Accuracy: 0.43
Adding run metadata for 0
2019-05-23 05:46:38.317248: step 100, loss = 5.81  learning rate = 0.07  (1.2 examples/sec; 25.665 sec/batch)
Minibatch accuracy2: 0.62
2019-05-23 05:47:02.531962: step 200, loss = 6.15  learning rate = 0.07  (1.3 examples/sec; 23.973 sec/batch)
Minibatch accuracy2: 0.61


############

Classifier (BATCH_SIZE = 256 and NUM_EPOCHS = 10)
```
/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/bin/python /Applications/PyCharm.app/Contents/helpers/pydev/pydevconsole.py --mode=client --port=58574
/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/lib/python2.7/site-packages/IPython/core/interactiveshell.py:726: UserWarning: Attempting to work in a virtualenv. If you encounter problems, please install IPython inside the virtualenv.
  warn("Attempting to work in a virtualenv. If you encounter problems, please "
import sys; print('Python %s on %s' % (sys.version, sys.platform))
sys.path.extend(['/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn'])
Python 2.7.10 (default, Feb 22 2019, 21:17:52) 
Type "copyright", "credits" or "license" for more information.
IPython 5.8.0 -- An enhanced Interactive Python.
?         -> Introduction and overview of IPython's features.
%quickref -> Quick reference.
help      -> Python's own help system.
object?   -> Details about 'object', use 'object??' for extra details.
PyDev console: using IPython 5.8.0
Python 2.7.10 (default, Feb 22 2019, 21:17:52) 
[GCC 4.2.1 Compatible Apple LLVM 10.0.1 (clang-1001.0.37.14)] on darwin
runfile('/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/train_classifier.py', wdir='/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn')
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/lib/python2.7/site-packages/tensorflow/python/framework/op_def_library.py:263: colocate_with (from tensorflow.python.framework.ops) is deprecated and will be removed in a future version.
Instructions for updating:
Colocations handled automatically by placer.
Starting without Saved Weights.
Training (65931, 32, 32, 3)
Valid (7326, 32, 32, 3)
Test (26032, 32, 32, 3)
Using drop out
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/svhn_model.py:123: calling dropout (from tensorflow.python.ops.nn_ops) with keep_prob is deprecated and will be removed in a future version.
Instructions for updating:
Please use `rate` instead of `keep_prob`. Rate should be set to `rate = 1 - keep_prob`.
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/train_classifier.py:71: softmax_cross_entropy_with_logits (from tensorflow.python.ops.nn_ops) is deprecated and will be removed in a future version.
Instructions for updating:
Future major versions of TensorFlow will allow gradients to flow
into the labels input on backprop by default.
See `tf.nn.softmax_cross_entropy_with_logits_v2`.
Not using dropout
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/lib/python2.7/site-packages/tensorflow/python/util/tf_should_use.py:193: initialize_all_variables (from tensorflow.python.ops.variables) is deprecated and will be removed after 2017-03-02.
Instructions for updating:
Use `tf.global_variables_initializer` instead.
2019-05-12 22:35:50.348072: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2 FMA
Validation Accuracy: 0.11%
Training Accuracy: 0.13%
Adding run metadata for 0
2019-05-12 22:35:51.796044: step 0, loss = 2.28  learning rate = 0.075000  (352.2 examples/sec; 0.73 sec/batch)
Mini-Batch Accuracy: 0.05%

(...)

Mini-Batch Accuracy: 0.95%
2019-05-12 22:45:06.387072: step 1900, loss = 0.30  learning rate = 0.052375  (8.9 examples/sec; 28.79 sec/batch)
Mini-Batch Accuracy: 0.93%
Validation Accuracy: 0.90%
Training Accuracy: 0.96%
Adding run metadata for 2000
2019-05-12 22:45:35.745231: step 2000, loss = 0.16  learning rate = 0.052375  (8.9 examples/sec; 28.76 sec/batch)
Mini-Batch Accuracy: 0.95%
2019-05-12 22:46:04.535938: step 2100, loss = 0.22  learning rate = 0.049757  (8.9 examples/sec; 28.79 sec/batch)
Mini-Batch Accuracy: 0.95%
2019-05-12 22:46:33.176015: step 2200, loss = 0.24  learning rate = 0.049757  (8.9 examples/sec; 28.64 sec/batch)
Mini-Batch Accuracy: 0.93%
2019-05-12 22:47:01.718892: step 2300, loss = 0.34  learning rate = 0.049757  (9.0 examples/sec; 28.54 sec/batch)
Mini-Batch Accuracy: 0.93%
2019-05-12 22:47:30.538166: step 2400, loss = 0.37  learning rate = 0.047269  (8.9 examples/sec; 28.82 sec/batch)
Mini-Batch Accuracy: 0.89%
2019-05-12 22:47:59.338596: step 2500, loss = 0.25  learning rate = 0.047269  (8.9 examples/sec; 28.80 sec/batch)
Mini-Batch Accuracy: 0.93%
Model saved in file: classifier.ckpt
Test Accuracy: 0.91406%
```

Regression: (BATCH_SIZE = 32 and NUM_EPOCHS = 10)
```
/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/bin/python /Applications/PyCharm.app/Contents/helpers/pydev/pydevconsole.py --mode=client --port=58743
/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/lib/python2.7/site-packages/IPython/core/interactiveshell.py:726: UserWarning: Attempting to work in a virtualenv. If you encounter problems, please install IPython inside the virtualenv.
  warn("Attempting to work in a virtualenv. If you encounter problems, please "
import sys; print('Python %s on %s' % (sys.version, sys.platform))
sys.path.extend(['/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn'])
Python 2.7.10 (default, Feb 22 2019, 21:17:52) 
Type "copyright", "credits" or "license" for more information.
IPython 5.8.0 -- An enhanced Interactive Python.
?         -> Introduction and overview of IPython's features.
%quickref -> Quick reference.
help      -> Python's own help system.
object?   -> Details about 'object', use 'object??' for extra details.
PyDev console: using IPython 5.8.0
Python 2.7.10 (default, Feb 22 2019, 21:17:52) 
[GCC 4.2.1 Compatible Apple LLVM 10.0.1 (clang-1001.0.37.14)] on darwin
runfile('/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/train_regressor.py', wdir='/Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn')
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/lib/python2.7/site-packages/tensorflow/python/framework/op_def_library.py:263: colocate_with (from tensorflow.python.framework.ops) is deprecated and will be removed in a future version.
Instructions for updating:
Colocations handled automatically by placer.
Starting without Saved Weights.
TrainData (30061, 64, 64, 3)
Valid Data (3341, 64, 64, 3)
Test Data (13068, 64, 64, 3)
2019-05-12 23:33:18.994250: I tensorflow/core/platform/cpu_feature_guard.cc:141] Your CPU supports instructions that this TensorFlow binary was not compiled to use: AVX2 FMA
WARNING:tensorflow:From /Users/bambrozi/workspace/github.com/bambrozio/tensorflow-svhn/env/lib/python2.7/site-packages/tensorflow/python/util/tf_should_use.py:193: initialize_all_variables (from tensorflow.python.ops.variables) is deprecated and will be removed after 2017-03-02.
Instructions for updating:
Use `tf.global_variables_initializer` instead.
Model restored.
Validation Accuracy: 0.61
Training Set Accuracy: 0.44
Adding run metadata for 0
2019-05-12 23:33:43.875866: step 100, loss = 5.80  learning rate = 0.07  (1.3 examples/sec; 24.651 sec/batch)
Minibatch accuracy2: 0.62

(...)

2019-05-13 00:04:44.315360: step 8500, loss = 5.53  learning rate = 0.05  (1.5 examples/sec; 21.415 sec/batch)
Minibatch accuracy2: 0.62
2019-05-13 00:05:05.967146: step 8600, loss = 6.39  learning rate = 0.05  (1.5 examples/sec; 21.436 sec/batch)
Minibatch accuracy2: 0.59
2019-05-13 00:05:27.639811: step 8700, loss = 6.07  learning rate = 0.05  (1.5 examples/sec; 21.458 sec/batch)
Minibatch accuracy2: 0.62
2019-05-13 00:05:49.304660: step 8800, loss = 6.80  learning rate = 0.05  (1.5 examples/sec; 21.446 sec/batch)
Minibatch accuracy2: 0.58
2019-05-13 00:06:10.933294: step 8900, loss = 5.91  learning rate = 0.05  (1.5 examples/sec; 21.414 sec/batch)
Minibatch accuracy2: 0.62
Validation Accuracy: 0.63
Training Set Accuracy: 0.60
Adding run metadata for 9000
2019-05-13 00:06:54.628490: step 9100, loss = 5.85  learning rate = 0.05  (0.7 examples/sec; 43.481 sec/batch)
Minibatch accuracy2: 0.61
2019-05-13 00:07:16.316061: step 9200, loss = 6.41  learning rate = 0.05  (1.5 examples/sec; 21.472 sec/batch)
Minibatch accuracy2: 0.60
2019-05-13 00:07:37.976779: step 9300, loss = 5.84  learning rate = 0.05  (1.5 examples/sec; 21.437 sec/batch)
Minibatch accuracy2: 0.64
Test accuracy: 0.66
Model saved in file: regression.ckpt
```
