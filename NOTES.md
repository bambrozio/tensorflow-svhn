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

(...)
2019-05-23 06:38:46.538080: step 14100, loss = 0.79  learning rate = 0.03  (0.7 examples/sec; 44.870 sec/batch)
Minibatch accuracy2: 0.94
2019-05-23 06:39:08.761247: step 14200, loss = 1.16  learning rate = 0.03  (1.5 examples/sec; 22.006 sec/batch)
Minibatch accuracy2: 0.93
2019-05-23 06:39:31.015520: step 14300, loss = 1.01  learning rate = 0.03  (1.5 examples/sec; 22.037 sec/batch)
Minibatch accuracy2: 0.93
2019-05-23 06:39:53.258833: step 14400, loss = 0.46  learning rate = 0.03  (1.5 examples/sec; 22.029 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 06:40:16.221667: step 14500, loss = 0.88  learning rate = 0.03  (1.4 examples/sec; 22.750 sec/batch)
Minibatch accuracy2: 0.95
2019-05-23 06:40:38.373752: step 14600, loss = 0.72  learning rate = 0.03  (1.5 examples/sec; 21.940 sec/batch)
Minibatch accuracy2: 0.95
2019-05-23 06:41:00.620773: step 14700, loss = 0.54  learning rate = 0.03  (1.5 examples/sec; 22.031 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 06:41:22.963882: step 14800, loss = 0.57  learning rate = 0.03  (1.4 examples/sec; 22.126 sec/batch)
Minibatch accuracy2: 0.96
2019-05-23 06:41:45.208566: step 14900, loss = 0.53  learning rate = 0.03  (1.5 examples/sec; 21.986 sec/batch)
Minibatch accuracy2: 0.97
Validation Accuracy: 0.94
Training Set Accuracy: 0.95
Adding run metadata for 15000
2019-05-23 06:42:30.409995: step 15100, loss = 0.67  learning rate = 0.03  (0.7 examples/sec; 44.979 sec/batch)
Minibatch accuracy2: 0.94
2019-05-23 06:42:52.604580: step 15200, loss = 0.67  learning rate = 0.03  (1.5 examples/sec; 21.976 sec/batch)
Minibatch accuracy2: 0.96
2019-05-23 06:43:14.874891: step 15300, loss = 0.65  learning rate = 0.03  (1.5 examples/sec; 22.056 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 06:43:37.129213: step 15400, loss = 0.51  learning rate = 0.03  (1.5 examples/sec; 22.038 sec/batch)
Minibatch accuracy2: 0.97
2019-05-23 06:43:59.310420: step 15500, loss = 0.39  learning rate = 0.03  (1.5 examples/sec; 21.964 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 06:44:21.586204: step 15600, loss = 0.94  learning rate = 0.03  (1.5 examples/sec; 22.060 sec/batch)
Minibatch accuracy2: 0.95
2019-05-23 06:44:43.836252: step 15700, loss = 0.78  learning rate = 0.03  (1.5 examples/sec; 22.031 sec/batch)
Minibatch accuracy2: 0.95
2019-05-23 06:45:06.137967: step 15800, loss = 0.60  learning rate = 0.03  (1.5 examples/sec; 22.067 sec/batch)
Minibatch accuracy2: 0.96
2019-05-23 06:45:29.030524: step 15900, loss = 0.38  learning rate = 0.03  (1.4 examples/sec; 22.669 sec/batch)
Minibatch accuracy2: 0.98
Validation Accuracy: 0.96
Training Set Accuracy: 1.00
Adding run metadata for 16000
2019-05-23 06:46:14.012273: step 16100, loss = 0.80  learning rate = 0.03  (0.7 examples/sec; 44.759 sec/batch)
Minibatch accuracy2: 0.96
2019-05-23 06:46:36.346504: step 16200, loss = 0.35  learning rate = 0.03  (1.4 examples/sec; 22.085 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 06:46:58.679836: step 16300, loss = 0.53  learning rate = 0.03  (1.4 examples/sec; 22.112 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 06:47:21.021859: step 16400, loss = 0.26  learning rate = 0.03  (1.4 examples/sec; 22.123 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 06:47:43.277142: step 16500, loss = 0.61  learning rate = 0.03  (1.5 examples/sec; 22.029 sec/batch)
Minibatch accuracy2: 0.97
2019-05-23 06:48:05.454637: step 16600, loss = 0.73  learning rate = 0.03  (1.5 examples/sec; 21.965 sec/batch)
Minibatch accuracy2: 0.96
2019-05-23 06:48:27.732643: step 16700, loss = 0.79  learning rate = 0.03  (1.5 examples/sec; 22.060 sec/batch)
Minibatch accuracy2: 0.96
2019-05-23 06:48:50.051057: step 16800, loss = 0.33  learning rate = 0.03  (1.4 examples/sec; 22.095 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 06:49:12.276928: step 16900, loss = 0.32  learning rate = 0.03  (1.5 examples/sec; 21.991 sec/batch)
Minibatch accuracy2: 0.99
Validation Accuracy: 0.90
Training Set Accuracy: 0.96
Adding run metadata for 17000
2019-05-23 06:49:57.333268: step 17100, loss = 0.49  learning rate = 0.03  (0.7 examples/sec; 44.840 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 06:50:20.352187: step 17200, loss = 0.67  learning rate = 0.03  (1.4 examples/sec; 22.801 sec/batch)
Minibatch accuracy2: 0.96
2019-05-23 06:50:42.377819: step 17300, loss = 0.86  learning rate = 0.03  (1.5 examples/sec; 21.806 sec/batch)
Minibatch accuracy2: 0.96
2019-05-23 06:51:04.520411: step 17400, loss = 0.53  learning rate = 0.03  (1.5 examples/sec; 21.926 sec/batch)
Minibatch accuracy2: 0.97
2019-05-23 06:51:26.916760: step 17500, loss = 0.75  learning rate = 0.03  (1.4 examples/sec; 22.182 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 06:51:49.114834: step 17600, loss = 0.38  learning rate = 0.03  (1.5 examples/sec; 21.983 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 06:52:11.459923: step 17700, loss = 0.72  learning rate = 0.03  (1.4 examples/sec; 22.126 sec/batch)
Minibatch accuracy2: 0.96
2019-05-23 06:52:33.720863: step 17800, loss = 0.30  learning rate = 0.03  (1.5 examples/sec; 22.040 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 06:52:56.383744: step 17900, loss = 0.40  learning rate = 0.03  (1.4 examples/sec; 22.302 sec/batch)
Minibatch accuracy2: 0.97
Validation Accuracy: 0.95
Training Set Accuracy: 1.00
Adding run metadata for 18000
2019-05-23 06:53:41.776299: step 18100, loss = 0.49  learning rate = 0.03  (0.7 examples/sec; 45.176 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 06:54:04.207954: step 18200, loss = 0.49  learning rate = 0.03  (1.4 examples/sec; 22.212 sec/batch)
Minibatch accuracy2: 0.96
2019-05-23 06:54:26.769795: step 18300, loss = 0.50  learning rate = 0.03  (1.4 examples/sec; 22.336 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 06:54:49.101181: step 18400, loss = 0.58  learning rate = 0.03  (1.4 examples/sec; 22.114 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 06:55:12.229457: step 18500, loss = 0.36  learning rate = 0.03  (1.4 examples/sec; 22.888 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 06:55:34.902810: step 18600, loss = 0.39  learning rate = 0.03  (1.4 examples/sec; 22.456 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 06:55:57.528048: step 18700, loss = 0.33  learning rate = 0.03  (1.4 examples/sec; 22.384 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 06:56:19.963669: step 18800, loss = 0.52  learning rate = 0.03  (1.4 examples/sec; 22.212 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 06:56:42.525129: step 18900, loss = 0.62  learning rate = 0.03  (1.4 examples/sec; 22.331 sec/batch)
Minibatch accuracy2: 0.97
Validation Accuracy: 0.93
Training Set Accuracy: 0.99
Adding run metadata for 19000
2019-05-23 06:57:28.243380: step 19100, loss = 0.39  learning rate = 0.03  (0.7 examples/sec; 45.495 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 06:57:50.706084: step 19200, loss = 0.69  learning rate = 0.03  (1.4 examples/sec; 22.235 sec/batch)
Minibatch accuracy2: 0.97
2019-05-23 06:58:13.288473: step 19300, loss = 0.83  learning rate = 0.03  (1.4 examples/sec; 22.338 sec/batch)
Minibatch accuracy2: 0.96
2019-05-23 06:58:35.762809: step 19400, loss = 0.29  learning rate = 0.03  (1.4 examples/sec; 22.250 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 06:58:58.254255: step 19500, loss = 0.73  learning rate = 0.03  (1.4 examples/sec; 22.273 sec/batch)
Minibatch accuracy2: 0.95
2019-05-23 06:59:20.790413: step 19600, loss = 0.41  learning rate = 0.03  (1.4 examples/sec; 22.310 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 06:59:43.313841: step 19700, loss = 0.47  learning rate = 0.03  (1.4 examples/sec; 22.304 sec/batch)
Minibatch accuracy2: 0.96
2019-05-23 07:00:05.898924: step 19800, loss = 0.66  learning rate = 0.03  (1.4 examples/sec; 22.355 sec/batch)
Minibatch accuracy2: 0.96
2019-05-23 07:00:28.957574: step 19900, loss = 0.44  learning rate = 0.03  (1.4 examples/sec; 22.842 sec/batch)
Minibatch accuracy2: 0.98
Validation Accuracy: 0.93
Training Set Accuracy: 0.96
Adding run metadata for 20000
2019-05-23 07:01:14.485124: step 20100, loss = 0.49  learning rate = 0.02  (0.7 examples/sec; 45.302 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 07:01:37.074230: step 20200, loss = 0.18  learning rate = 0.02  (1.4 examples/sec; 22.373 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:01:59.584178: step 20300, loss = 0.36  learning rate = 0.02  (1.4 examples/sec; 22.261 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:02:22.145783: step 20400, loss = 0.52  learning rate = 0.02  (1.4 examples/sec; 22.337 sec/batch)
Minibatch accuracy2: 0.97
2019-05-23 07:02:44.522178: step 20500, loss = 0.55  learning rate = 0.02  (1.4 examples/sec; 22.150 sec/batch)
Minibatch accuracy2: 0.94
2019-05-23 07:03:07.017278: step 20600, loss = 0.34  learning rate = 0.02  (1.4 examples/sec; 22.274 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 07:03:29.433771: step 20700, loss = 0.48  learning rate = 0.02  (1.4 examples/sec; 22.193 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:03:51.919278: step 20800, loss = 0.39  learning rate = 0.02  (1.4 examples/sec; 22.265 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:04:14.427471: step 20900, loss = 0.15  learning rate = 0.02  (1.4 examples/sec; 22.286 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.94
Training Set Accuracy: 1.00
Adding run metadata for 21000
2019-05-23 07:04:59.885784: step 21100, loss = 0.55  learning rate = 0.02  (0.7 examples/sec; 45.236 sec/batch)
Minibatch accuracy2: 0.96
2019-05-23 07:05:23.335235: step 21200, loss = 0.23  learning rate = 0.02  (1.4 examples/sec; 23.226 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:05:45.858108: step 21300, loss = 0.25  learning rate = 0.02  (1.4 examples/sec; 22.303 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:06:08.295846: step 21400, loss = 0.25  learning rate = 0.02  (1.4 examples/sec; 22.218 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:06:30.833029: step 21500, loss = 0.25  learning rate = 0.02  (1.4 examples/sec; 22.311 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:06:53.317042: step 21600, loss = 0.29  learning rate = 0.02  (1.4 examples/sec; 22.268 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:07:16.035573: step 21700, loss = 0.30  learning rate = 0.02  (1.4 examples/sec; 22.495 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:07:38.405616: step 21800, loss = 0.36  learning rate = 0.02  (1.4 examples/sec; 22.149 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 07:08:00.882999: step 21900, loss = 0.26  learning rate = 0.02  (1.4 examples/sec; 22.262 sec/batch)
Minibatch accuracy2: 0.99
Validation Accuracy: 0.92
Training Set Accuracy: 1.00
Adding run metadata for 22000
2019-05-23 07:08:46.216101: step 22100, loss = 0.56  learning rate = 0.02  (0.7 examples/sec; 45.115 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:09:08.617410: step 22200, loss = 0.16  learning rate = 0.02  (1.4 examples/sec; 22.182 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:09:31.098316: step 22300, loss = 0.37  learning rate = 0.02  (1.4 examples/sec; 22.266 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:09:53.733597: step 22400, loss = 0.32  learning rate = 0.02  (1.4 examples/sec; 22.410 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:10:16.999457: step 22500, loss = 0.35  learning rate = 0.02  (1.4 examples/sec; 23.016 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:10:39.382323: step 22600, loss = 0.38  learning rate = 0.02  (1.4 examples/sec; 22.160 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:11:01.917822: step 22700, loss = 0.36  learning rate = 0.02  (1.4 examples/sec; 22.315 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:11:24.456734: step 22800, loss = 0.25  learning rate = 0.02  (1.4 examples/sec; 22.315 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:11:46.918284: step 22900, loss = 0.13  learning rate = 0.02  (1.4 examples/sec; 22.243 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.94
Training Set Accuracy: 0.99
Adding run metadata for 23000
2019-05-23 07:12:32.544533: step 23100, loss = 0.16  learning rate = 0.02  (0.7 examples/sec; 45.399 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:12:55.089688: step 23200, loss = 0.23  learning rate = 0.02  (1.4 examples/sec; 22.297 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:13:17.548166: step 23300, loss = 0.08  learning rate = 0.02  (1.4 examples/sec; 22.235 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:13:40.046224: step 23400, loss = 0.37  learning rate = 0.02  (1.4 examples/sec; 22.274 sec/batch)
Minibatch accuracy2: 0.98
2019-05-23 07:14:02.600672: step 23500, loss = 0.11  learning rate = 0.02  (1.4 examples/sec; 22.330 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:14:25.089404: step 23600, loss = 0.22  learning rate = 0.02  (1.4 examples/sec; 22.245 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:14:47.440461: step 23700, loss = 0.38  learning rate = 0.02  (1.4 examples/sec; 22.130 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:15:10.270610: step 23800, loss = 0.36  learning rate = 0.02  (1.4 examples/sec; 22.559 sec/batch)
Minibatch accuracy2: 0.97
2019-05-23 07:15:33.099311: step 23900, loss = 0.19  learning rate = 0.02  (1.4 examples/sec; 22.605 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.92
Training Set Accuracy: 1.00
Adding run metadata for 24000
2019-05-23 07:16:18.491191: step 24100, loss = 0.20  learning rate = 0.02  (0.7 examples/sec; 45.166 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:16:41.004469: step 24200, loss = 0.13  learning rate = 0.02  (1.4 examples/sec; 22.295 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:17:03.687261: step 24300, loss = 0.22  learning rate = 0.02  (1.4 examples/sec; 22.462 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:17:26.242279: step 24400, loss = 0.23  learning rate = 0.02  (1.4 examples/sec; 22.332 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:17:48.758658: step 24500, loss = 0.15  learning rate = 0.02  (1.4 examples/sec; 22.293 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:18:11.257659: step 24600, loss = 0.19  learning rate = 0.02  (1.4 examples/sec; 22.278 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:18:33.719430: step 24700, loss = 0.21  learning rate = 0.02  (1.4 examples/sec; 22.241 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:18:56.098439: step 24800, loss = 0.20  learning rate = 0.02  (1.4 examples/sec; 22.162 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:19:18.611204: step 24900, loss = 0.31  learning rate = 0.02  (1.4 examples/sec; 22.294 sec/batch)
Minibatch accuracy2: 0.99
Validation Accuracy: 0.90
Training Set Accuracy: 1.00
Adding run metadata for 25000
2019-05-23 07:20:04.348872: step 25100, loss = 0.09  learning rate = 0.02  (0.7 examples/sec; 45.503 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:20:27.565962: step 25200, loss = 0.28  learning rate = 0.02  (1.4 examples/sec; 22.999 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:20:50.050336: step 25300, loss = 0.18  learning rate = 0.02  (1.4 examples/sec; 22.262 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:21:12.585793: step 25400, loss = 0.30  learning rate = 0.02  (1.4 examples/sec; 22.312 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:21:35.020838: step 25500, loss = 0.16  learning rate = 0.02  (1.4 examples/sec; 22.199 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:21:57.490127: step 25600, loss = 0.18  learning rate = 0.02  (1.4 examples/sec; 22.247 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:22:20.156783: step 25700, loss = 0.17  learning rate = 0.02  (1.4 examples/sec; 22.447 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:22:42.596791: step 25800, loss = 0.26  learning rate = 0.02  (1.4 examples/sec; 22.220 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:23:04.943854: step 25900, loss = 0.19  learning rate = 0.02  (1.4 examples/sec; 22.128 sec/batch)
Minibatch accuracy2: 0.99
Validation Accuracy: 0.92
Training Set Accuracy: 0.99
Adding run metadata for 26000
2019-05-23 07:23:50.424739: step 26100, loss = 0.20  learning rate = 0.02  (0.7 examples/sec; 45.263 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:24:12.889331: step 26200, loss = 0.11  learning rate = 0.02  (1.4 examples/sec; 22.246 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:24:35.347579: step 26300, loss = 0.17  learning rate = 0.02  (1.4 examples/sec; 22.237 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:24:57.829907: step 26400, loss = 0.12  learning rate = 0.02  (1.4 examples/sec; 22.266 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:25:21.183822: step 26500, loss = 0.14  learning rate = 0.02  (1.4 examples/sec; 23.135 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:25:43.510796: step 26600, loss = 0.14  learning rate = 0.02  (1.4 examples/sec; 22.094 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:26:05.984644: step 26700, loss = 0.17  learning rate = 0.02  (1.4 examples/sec; 22.252 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:26:28.511367: step 26800, loss = 0.09  learning rate = 0.02  (1.4 examples/sec; 22.307 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:26:51.050830: step 26900, loss = 0.10  learning rate = 0.02  (1.4 examples/sec; 22.318 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.94
Training Set Accuracy: 1.00
Adding run metadata for 27000
2019-05-23 07:27:36.684301: step 27100, loss = 0.09  learning rate = 0.02  (0.7 examples/sec; 45.415 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:27:59.169275: step 27200, loss = 0.23  learning rate = 0.02  (1.4 examples/sec; 22.256 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:28:21.712019: step 27300, loss = 0.26  learning rate = 0.02  (1.4 examples/sec; 22.323 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:28:44.047118: step 27400, loss = 0.12  learning rate = 0.02  (1.4 examples/sec; 22.113 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:29:06.570923: step 27500, loss = 0.14  learning rate = 0.02  (1.4 examples/sec; 22.301 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:29:29.132265: step 27600, loss = 0.07  learning rate = 0.02  (1.4 examples/sec; 22.342 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:29:51.595021: step 27700, loss = 0.17  learning rate = 0.02  (1.4 examples/sec; 22.243 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:30:14.636428: step 27800, loss = 0.20  learning rate = 0.02  (1.4 examples/sec; 22.788 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:30:37.254020: step 27900, loss = 0.21  learning rate = 0.02  (1.4 examples/sec; 22.394 sec/batch)
Minibatch accuracy2: 0.99
Validation Accuracy: 0.93
Training Set Accuracy: 1.00
Adding run metadata for 28000
2019-05-23 07:31:22.924728: step 28100, loss = 0.13  learning rate = 0.02  (0.7 examples/sec; 45.456 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:31:45.477113: step 28200, loss = 0.14  learning rate = 0.02  (1.4 examples/sec; 22.337 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:32:08.221127: step 28300, loss = 0.10  learning rate = 0.02  (1.4 examples/sec; 22.518 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:32:30.840766: step 28400, loss = 0.06  learning rate = 0.02  (1.4 examples/sec; 22.398 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:32:53.329198: step 28500, loss = 0.10  learning rate = 0.02  (1.4 examples/sec; 22.272 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:33:15.934350: step 28600, loss = 0.09  learning rate = 0.02  (1.4 examples/sec; 22.379 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:33:38.407025: step 28700, loss = 0.15  learning rate = 0.02  (1.4 examples/sec; 22.253 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:34:00.946723: step 28800, loss = 0.19  learning rate = 0.02  (1.4 examples/sec; 22.320 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:34:23.400210: step 28900, loss = 0.16  learning rate = 0.02  (1.4 examples/sec; 22.226 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.93
Training Set Accuracy: 1.00
Adding run metadata for 29000
2019-05-23 07:35:09.212288: step 29100, loss = 0.10  learning rate = 0.02  (0.7 examples/sec; 45.571 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:35:32.305059: step 29200, loss = 0.08  learning rate = 0.02  (1.4 examples/sec; 22.870 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:35:54.756328: step 29300, loss = 0.09  learning rate = 0.02  (1.4 examples/sec; 22.226 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:36:17.385047: step 29400, loss = 0.11  learning rate = 0.02  (1.4 examples/sec; 22.410 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:36:39.921543: step 29500, loss = 0.09  learning rate = 0.01  (1.4 examples/sec; 22.314 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:37:02.485601: step 29600, loss = 0.19  learning rate = 0.01  (1.4 examples/sec; 22.347 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:37:25.149863: step 29700, loss = 0.07  learning rate = 0.01  (1.4 examples/sec; 22.420 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:37:47.643118: step 29800, loss = 0.14  learning rate = 0.01  (1.4 examples/sec; 22.273 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:38:10.182616: step 29900, loss = 0.31  learning rate = 0.01  (1.4 examples/sec; 22.319 sec/batch)
Minibatch accuracy2: 0.99
Validation Accuracy: 0.90
Training Set Accuracy: 1.00
Adding run metadata for 30000
2019-05-23 07:38:55.669790: step 30100, loss = 0.10  learning rate = 0.01  (0.7 examples/sec; 45.264 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:39:18.344769: step 30200, loss = 0.17  learning rate = 0.01  (1.4 examples/sec; 22.438 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:39:40.893083: step 30300, loss = 0.06  learning rate = 0.01  (1.4 examples/sec; 22.325 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:40:03.417395: step 30400, loss = 0.08  learning rate = 0.01  (1.4 examples/sec; 22.303 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:40:26.755290: step 30500, loss = 0.11  learning rate = 0.01  (1.4 examples/sec; 23.114 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:40:49.272219: step 30600, loss = 0.14  learning rate = 0.01  (1.4 examples/sec; 22.303 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:41:11.847728: step 30700, loss = 0.13  learning rate = 0.01  (1.4 examples/sec; 22.357 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:41:34.261873: step 30800, loss = 0.17  learning rate = 0.01  (1.4 examples/sec; 22.194 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:41:56.927810: step 30900, loss = 0.09  learning rate = 0.01  (1.4 examples/sec; 22.445 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.95
Training Set Accuracy: 1.00
Adding run metadata for 31000
2019-05-23 07:42:42.584054: step 31100, loss = 0.11  learning rate = 0.01  (0.7 examples/sec; 45.435 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:43:05.079930: step 31200, loss = 0.08  learning rate = 0.01  (1.4 examples/sec; 22.250 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:43:28.153673: step 31300, loss = 0.17  learning rate = 0.01  (1.4 examples/sec; 22.846 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:43:51.036447: step 31400, loss = 0.06  learning rate = 0.01  (1.4 examples/sec; 22.661 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:44:13.556503: step 31500, loss = 0.08  learning rate = 0.01  (1.4 examples/sec; 22.283 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:44:36.067553: step 31600, loss = 0.06  learning rate = 0.01  (1.4 examples/sec; 22.296 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:44:58.626245: step 31700, loss = 0.13  learning rate = 0.01  (1.4 examples/sec; 22.338 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:45:21.962861: step 31800, loss = 0.13  learning rate = 0.01  (1.4 examples/sec; 23.116 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:45:44.407332: step 31900, loss = 0.15  learning rate = 0.01  (1.4 examples/sec; 22.226 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.89
Training Set Accuracy: 1.00
Adding run metadata for 32000
2019-05-23 07:46:30.095327: step 32100, loss = 0.08  learning rate = 0.01  (0.7 examples/sec; 45.468 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:46:52.734857: step 32200, loss = 0.19  learning rate = 0.01  (1.4 examples/sec; 22.411 sec/batch)
Minibatch accuracy2: 0.99
2019-05-23 07:47:15.440671: step 32300, loss = 0.08  learning rate = 0.01  (1.4 examples/sec; 22.487 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:47:37.960969: step 32400, loss = 0.13  learning rate = 0.01  (1.4 examples/sec; 22.301 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:48:00.588374: step 32500, loss = 0.08  learning rate = 0.01  (1.4 examples/sec; 22.397 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:48:23.171030: step 32600, loss = 0.08  learning rate = 0.01  (1.4 examples/sec; 22.356 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:48:45.636397: step 32700, loss = 0.07  learning rate = 0.01  (1.4 examples/sec; 22.245 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:49:08.241168: step 32800, loss = 0.07  learning rate = 0.01  (1.4 examples/sec; 22.385 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 07:49:30.780146: step 32900, loss = 0.14  learning rate = 0.01  (1.4 examples/sec; 22.314 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.93
Training Set Accuracy: 1.00
Adding run metadata for 33000

(...)

2019-05-23 10:29:33.895826: step 71800, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.858 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:29:59.785411: step 71900, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.569 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.89
Training Set Accuracy: 1.00
Adding run metadata for 72000
2019-05-23 10:30:54.993136: step 72100, loss = 0.03  learning rate = 0.00  (0.6 examples/sec; 54.953 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:31:20.544382: step 72200, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.308 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:31:45.301190: step 72300, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.473 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:32:11.454623: step 72400, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 25.847 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:32:40.373865: step 72500, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 28.638 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:33:11.009498: step 72600, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 30.362 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:33:38.955778: step 72700, loss = 0.07  learning rate = 0.00  (1.2 examples/sec; 27.662 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:34:07.000441: step 72800, loss = 0.07  learning rate = 0.00  (1.2 examples/sec; 27.788 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:34:34.743535: step 72900, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 27.460 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.93
Training Set Accuracy: 1.00
Adding run metadata for 73000
2019-05-23 10:35:31.730222: step 73100, loss = 0.05  learning rate = 0.00  (0.6 examples/sec; 56.706 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:36:02.239879: step 73200, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 30.235 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:36:31.698079: step 73300, loss = 0.07  learning rate = 0.00  (1.1 examples/sec; 29.197 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:36:59.969689: step 73400, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 27.876 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:37:28.772523: step 73500, loss = 0.06  learning rate = 0.00  (1.1 examples/sec; 28.532 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:37:59.064210: step 73600, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 30.023 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:38:27.927247: step 73700, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 28.493 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:38:59.614928: step 73800, loss = 0.07  learning rate = 0.00  (1.0 examples/sec; 31.397 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:39:27.822245: step 73900, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 27.921 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.89
Training Set Accuracy: 1.00
Adding run metadata for 74000
2019-05-23 10:40:24.453075: step 74100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 56.333 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:40:52.611609: step 74200, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 27.863 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:41:21.333116: step 74300, loss = 0.06  learning rate = 0.00  (1.1 examples/sec; 28.458 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:41:49.066987: step 74400, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 27.472 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:42:16.800160: step 74500, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 27.456 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:42:44.832551: step 74600, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 27.753 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:43:12.645246: step 74700, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 27.543 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:43:40.779357: step 74800, loss = 0.06  learning rate = 0.00  (1.1 examples/sec; 27.854 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:44:08.937536: step 74900, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 27.889 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.91
Training Set Accuracy: 1.00
Adding run metadata for 75000
2019-05-23 10:45:05.656613: step 75100, loss = 0.05  learning rate = 0.00  (0.6 examples/sec; 56.450 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:45:34.451996: step 75200, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 28.514 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:46:02.514628: step 75300, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 27.777 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:46:30.705763: step 75400, loss = 0.09  learning rate = 0.00  (1.1 examples/sec; 27.898 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:46:58.912990: step 75500, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 27.932 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:47:27.143940: step 75600, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 27.965 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:47:55.288432: step 75700, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 27.828 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:48:23.326461: step 75800, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 27.761 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:48:51.484824: step 75900, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 27.879 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.88
Training Set Accuracy: 1.00
Adding run metadata for 76000
2019-05-23 10:49:48.574031: step 76100, loss = 0.06  learning rate = 0.00  (0.6 examples/sec; 56.816 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:50:17.568805: step 76200, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 28.715 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:50:45.981879: step 76300, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 28.120 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:51:14.337584: step 76400, loss = 0.06  learning rate = 0.00  (1.1 examples/sec; 28.089 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:51:42.508706: step 76500, loss = 0.08  learning rate = 0.00  (1.1 examples/sec; 27.906 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:52:11.027928: step 76600, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 28.241 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:52:39.301454: step 76700, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 27.996 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:53:07.612068: step 76800, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 28.063 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:53:35.207238: step 76900, loss = 0.07  learning rate = 0.00  (1.2 examples/sec; 27.314 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.91
Training Set Accuracy: 1.00
Adding run metadata for 77000
2019-05-23 10:54:28.221975: step 77100, loss = 0.03  learning rate = 0.00  (0.6 examples/sec; 52.760 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:54:55.159583: step 77200, loss = 0.02  learning rate = 0.00  (1.2 examples/sec; 26.656 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:55:21.076434: step 77300, loss = 0.07  learning rate = 0.00  (1.2 examples/sec; 25.661 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:55:47.402563: step 77400, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.059 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:56:12.959719: step 77500, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.285 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:56:38.532529: step 77600, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 25.258 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:57:03.810424: step 77700, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.022 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:57:29.111416: step 77800, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.058 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:57:54.544962: step 77900, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.178 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.94
Training Set Accuracy: 1.00
Adding run metadata for 78000
2019-05-23 10:58:45.939408: step 78100, loss = 0.08  learning rate = 0.00  (0.6 examples/sec; 51.146 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:59:11.434020: step 78200, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.226 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 10:59:36.788569: step 78300, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.086 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:00:03.112990: step 78400, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.083 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:00:28.929778: step 78500, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.558 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:00:53.838781: step 78600, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.671 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:01:18.482454: step 78700, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.397 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:01:44.095860: step 78800, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.361 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:02:09.205017: step 78900, loss = 0.07  learning rate = 0.00  (1.3 examples/sec; 24.868 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.93
Training Set Accuracy: 1.00
Adding run metadata for 79000
2019-05-23 11:02:59.782729: step 79100, loss = 0.05  learning rate = 0.00  (0.6 examples/sec; 50.309 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:03:25.316555: step 79200, loss = 0.07  learning rate = 0.00  (1.3 examples/sec; 25.285 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:03:50.432605: step 79300, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.874 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:04:15.379381: step 79400, loss = 0.06  learning rate = 0.00  (1.3 examples/sec; 24.703 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:04:40.527261: step 79500, loss = 0.06  learning rate = 0.00  (1.3 examples/sec; 24.888 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:05:05.319282: step 79600, loss = 0.06  learning rate = 0.00  (1.3 examples/sec; 24.548 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:05:30.300552: step 79700, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.727 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:05:55.764603: step 79800, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 25.215 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:06:20.759788: step 79900, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.742 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.95
Training Set Accuracy: 1.00
Adding run metadata for 80000
2019-05-23 11:07:12.943188: step 80100, loss = 0.06  learning rate = 0.00  (0.6 examples/sec; 51.929 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:07:38.364838: step 80200, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.142 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:08:03.675141: step 80300, loss = 0.06  learning rate = 0.00  (1.3 examples/sec; 25.061 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:08:28.320313: step 80400, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.402 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:08:53.003500: step 80500, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.445 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:09:18.187125: step 80600, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.938 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:09:43.010991: step 80700, loss = 0.07  learning rate = 0.00  (1.3 examples/sec; 24.567 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:10:08.834077: step 80800, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 25.545 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:10:33.965598: step 80900, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.895 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.94
Training Set Accuracy: 1.00
Adding run metadata for 81000
2019-05-23 11:11:24.506731: step 81100, loss = 0.06  learning rate = 0.00  (0.6 examples/sec; 50.281 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:11:49.326632: step 81200, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.558 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:12:13.786348: step 81300, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.218 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:12:41.013604: step 81400, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.968 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:13:09.259451: step 81500, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 27.958 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:13:36.272621: step 81600, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 26.733 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:14:03.990175: step 81700, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 27.459 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:14:30.146045: step 81800, loss = 0.08  learning rate = 0.00  (1.2 examples/sec; 25.904 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:14:57.941346: step 81900, loss = 0.07  learning rate = 0.00  (1.2 examples/sec; 27.537 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.93
Training Set Accuracy: 1.00
Adding run metadata for 82000
2019-05-23 11:15:51.799096: step 82100, loss = 0.03  learning rate = 0.00  (0.6 examples/sec; 53.598 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:16:18.343521: step 82200, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.294 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:16:43.603772: step 82300, loss = 0.07  learning rate = 0.00  (1.3 examples/sec; 25.004 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:17:10.152917: step 82400, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.280 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:17:36.667351: step 82500, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.245 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:18:03.432308: step 82600, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.509 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:18:30.269735: step 82700, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.591 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:18:56.457573: step 82800, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 25.906 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:19:23.358670: step 82900, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 26.632 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.94
Training Set Accuracy: 1.00
Adding run metadata for 83000
2019-05-23 11:20:17.654770: step 83100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 54.037 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:20:44.936690: step 83200, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 27.041 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:21:11.291086: step 83300, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 26.106 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:21:36.826844: step 83400, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.285 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:22:02.683209: step 83500, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 25.601 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:22:30.429755: step 83600, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 27.462 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:22:57.854559: step 83700, loss = 0.02  learning rate = 0.00  (1.2 examples/sec; 27.168 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:23:24.796465: step 83800, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.616 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:23:51.438974: step 83900, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.319 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.93
Training Set Accuracy: 1.00
Adding run metadata for 84000
2019-05-23 11:24:44.792984: step 84100, loss = 0.03  learning rate = 0.00  (0.6 examples/sec; 53.088 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:25:12.309628: step 84200, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 27.264 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:25:39.610407: step 84300, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 27.037 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:26:05.712866: step 84400, loss = 0.08  learning rate = 0.00  (1.2 examples/sec; 25.845 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:26:32.938092: step 84500, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.961 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:26:59.241058: step 84600, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.061 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:27:27.712631: step 84700, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 28.169 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:27:55.867416: step 84800, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 27.899 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:28:21.971397: step 84900, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 25.854 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.93
Training Set Accuracy: 1.00
Adding run metadata for 85000
2019-05-23 11:29:15.856509: step 85100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 53.634 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:29:43.519271: step 85200, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 27.399 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:30:09.986773: step 85300, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.199 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:30:36.324097: step 85400, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.052 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:31:03.220949: step 85500, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.599 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:31:30.220047: step 85600, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.746 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:31:56.911643: step 85700, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.441 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:32:22.981899: step 85800, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 25.802 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:32:50.035476: step 85900, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.804 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.94
Training Set Accuracy: 1.00
Adding run metadata for 86000
2019-05-23 11:33:43.674997: step 86100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 53.371 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:34:11.035909: step 86200, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 27.096 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:34:38.135438: step 86300, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.837 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:35:04.641070: step 86400, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.215 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:35:32.082039: step 86500, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 27.178 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:35:59.132850: step 86600, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.752 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:36:26.415139: step 86700, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.953 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:36:51.530594: step 86800, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.875 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:37:18.171519: step 86900, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.365 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.92
Training Set Accuracy: 1.00
Adding run metadata for 87000
2019-05-23 11:38:11.247950: step 87100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 52.743 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:38:37.888646: step 87200, loss = 0.07  learning rate = 0.00  (1.2 examples/sec; 26.374 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:39:04.424524: step 87300, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.281 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:39:30.626791: step 87400, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 25.912 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:39:57.271690: step 87500, loss = 0.02  learning rate = 0.00  (1.2 examples/sec; 26.396 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:40:23.014102: step 87600, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.491 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:40:48.643931: step 87700, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.384 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:41:13.977901: step 87800, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.076 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:41:40.086229: step 87900, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 25.836 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.90
Training Set Accuracy: 1.00
Adding run metadata for 88000
2019-05-23 11:42:32.894922: step 88100, loss = 0.07  learning rate = 0.00  (0.6 examples/sec; 52.574 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:42:56.644157: step 88200, loss = 0.03  learning rate = 0.00  (1.4 examples/sec; 23.513 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:43:21.770966: step 88300, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.884 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:43:46.317068: step 88400, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.298 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:44:11.197160: step 88500, loss = 0.06  learning rate = 0.00  (1.3 examples/sec; 24.626 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:44:36.258855: step 88600, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.821 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:45:00.864904: step 88700, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.345 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:45:26.860923: step 88800, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 25.758 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:45:51.950957: step 88900, loss = 0.09  learning rate = 0.00  (1.3 examples/sec; 24.843 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.89
Training Set Accuracy: 1.00
Adding run metadata for 89000
2019-05-23 11:46:43.110862: step 89100, loss = 0.05  learning rate = 0.00  (0.6 examples/sec; 50.874 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:47:08.706909: step 89200, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.325 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:47:34.165752: step 89300, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.209 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:47:59.868506: step 89400, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 25.440 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:48:24.673252: step 89500, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.544 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:48:49.423341: step 89600, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.504 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:49:14.236335: step 89700, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.566 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:49:39.287011: step 89800, loss = 0.06  learning rate = 0.00  (1.3 examples/sec; 24.809 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:50:04.029071: step 89900, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.500 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.96
Training Set Accuracy: 1.00
Adding run metadata for 90000
2019-05-23 11:50:54.510937: step 90100, loss = 0.03  learning rate = 0.00  (0.6 examples/sec; 50.223 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:51:19.416692: step 90200, loss = 0.06  learning rate = 0.00  (1.3 examples/sec; 24.660 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:51:44.201851: step 90300, loss = 0.08  learning rate = 0.00  (1.3 examples/sec; 24.536 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:52:09.066410: step 90400, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.628 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:52:34.617080: step 90500, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.303 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:53:00.355285: step 90600, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.482 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:53:25.658030: step 90700, loss = 0.02  learning rate = 0.00  (1.3 examples/sec; 25.055 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:53:50.528500: step 90800, loss = 0.06  learning rate = 0.00  (1.3 examples/sec; 24.625 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:54:15.515742: step 90900, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.740 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.93
Training Set Accuracy: 1.00
Adding run metadata for 91000
2019-05-23 11:55:06.664615: step 91100, loss = 0.05  learning rate = 0.00  (0.6 examples/sec; 50.898 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:55:34.306952: step 91200, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 27.360 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:55:59.559546: step 91300, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.011 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:56:24.950925: step 91400, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.105 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:56:54.581036: step 91500, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 29.366 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:57:21.082163: step 91600, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.245 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:57:46.830869: step 91700, loss = 0.07  learning rate = 0.00  (1.3 examples/sec; 25.499 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:58:11.375397: step 91800, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.312 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:58:35.458635: step 91900, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 23.853 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.89
Training Set Accuracy: 1.00
Adding run metadata for 92000
2019-05-23 11:59:25.585757: step 92100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 49.868 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 11:59:51.005800: step 92200, loss = 0.07  learning rate = 0.00  (1.3 examples/sec; 25.154 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:00:16.239150: step 92300, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.999 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:00:40.405314: step 92400, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 23.931 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:01:06.812409: step 92500, loss = 0.07  learning rate = 0.00  (1.2 examples/sec; 26.143 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:01:35.213345: step 92600, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 28.107 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:02:02.543777: step 92700, loss = 0.02  learning rate = 0.00  (1.2 examples/sec; 27.068 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:02:29.998701: step 92800, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 27.180 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:02:57.129185: step 92900, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.858 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.90
Training Set Accuracy: 1.00
Adding run metadata for 93000
2019-05-23 12:03:51.816926: step 93100, loss = 0.06  learning rate = 0.00  (0.6 examples/sec; 54.416 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:04:19.065151: step 93200, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.984 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:04:45.906811: step 93300, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 26.586 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:05:12.820683: step 93400, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.645 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:05:39.604126: step 93500, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.520 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:06:06.030708: step 93600, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.182 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:06:30.562782: step 93700, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.288 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:06:55.086204: step 93800, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.270 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:07:19.687640: step 93900, loss = 0.07  learning rate = 0.00  (1.3 examples/sec; 24.337 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.96
Training Set Accuracy: 1.00
Adding run metadata for 94000
2019-05-23 12:08:10.399604: step 94100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 50.459 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:08:35.207766: step 94200, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.546 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:09:03.264592: step 94300, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 27.734 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:09:32.326833: step 94400, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 28.786 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:10:00.598797: step 94500, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 27.991 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:10:29.312213: step 94600, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 28.447 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:10:57.530473: step 94700, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 27.940 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:11:27.180844: step 94800, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 29.398 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:11:50.704808: step 94900, loss = 0.03  learning rate = 0.00  (1.4 examples/sec; 23.292 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.89
Training Set Accuracy: 1.00
Adding run metadata for 95000
2019-05-23 12:12:38.539855: step 95100, loss = 0.05  learning rate = 0.00  (0.7 examples/sec; 47.609 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:13:02.525157: step 95200, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 23.758 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:13:26.558082: step 95300, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 23.787 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:13:50.402240: step 95400, loss = 0.04  learning rate = 0.00  (1.4 examples/sec; 23.615 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:14:14.342659: step 95500, loss = 0.04  learning rate = 0.00  (1.4 examples/sec; 23.700 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:14:38.603132: step 95600, loss = 0.02  learning rate = 0.00  (1.3 examples/sec; 24.014 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:15:04.467503: step 95700, loss = 0.06  learning rate = 0.00  (1.3 examples/sec; 25.595 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:15:31.414810: step 95800, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.705 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:15:57.515479: step 95900, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 25.859 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.90
Training Set Accuracy: 1.00
Adding run metadata for 96000
2019-05-23 12:16:51.736135: step 96100, loss = 0.03  learning rate = 0.00  (0.6 examples/sec; 53.945 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:17:19.567142: step 96200, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 27.586 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:17:45.317375: step 96300, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.500 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:18:10.293155: step 96400, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.721 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:18:36.322601: step 96500, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 25.775 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:19:01.195314: step 96600, loss = 0.06  learning rate = 0.00  (1.3 examples/sec; 24.604 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:19:26.209564: step 96700, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.770 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:19:50.920757: step 96800, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.472 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:20:16.002388: step 96900, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.819 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.96
Training Set Accuracy: 1.00
Adding run metadata for 97000
2019-05-23 12:21:09.607923: step 97100, loss = 0.03  learning rate = 0.00  (0.6 examples/sec; 53.315 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:21:35.486565: step 97200, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 25.631 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:22:00.196035: step 97300, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.472 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:22:25.478996: step 97400, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.030 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:22:53.785546: step 97500, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 27.999 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:23:19.902742: step 97600, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 25.865 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:23:44.579563: step 97700, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.431 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:24:09.195343: step 97800, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.368 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:24:34.188716: step 97900, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.752 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.93
Training Set Accuracy: 1.00
Adding run metadata for 98000
2019-05-23 12:25:30.830763: step 98100, loss = 0.05  learning rate = 0.00  (0.6 examples/sec; 56.326 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:25:58.383735: step 98200, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 27.290 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:26:26.109341: step 98300, loss = 0.07  learning rate = 0.00  (1.2 examples/sec; 27.446 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:26:55.486858: step 98400, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 29.116 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:27:22.551055: step 98500, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.810 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:27:49.478027: step 98600, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.665 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:28:15.185939: step 98700, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.427 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:28:40.456909: step 98800, loss = 0.02  learning rate = 0.00  (1.3 examples/sec; 25.029 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:29:06.088863: step 98900, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.366 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.90
Training Set Accuracy: 1.00
Adding run metadata for 99000
2019-05-23 12:29:59.178113: step 99100, loss = 0.03  learning rate = 0.00  (0.6 examples/sec; 52.832 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:30:27.821706: step 99200, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 28.393 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:30:55.728876: step 99300, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 27.643 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:31:22.021693: step 99400, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 26.020 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:31:49.200610: step 99500, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.889 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:32:17.106846: step 99600, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 27.618 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:32:42.782727: step 99700, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 25.358 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:33:08.287605: step 99800, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.254 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:33:34.766585: step 99900, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.178 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.91
Training Set Accuracy: 1.00
Adding run metadata for 100000
2019-05-23 12:34:25.603694: step 100100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 50.596 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:34:50.491197: step 100200, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.644 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:35:16.711291: step 100300, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 25.937 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:35:45.160378: step 100400, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 28.142 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:36:11.693237: step 100500, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.258 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:36:40.376662: step 100600, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 28.419 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:37:08.218205: step 100700, loss = 0.07  learning rate = 0.00  (1.2 examples/sec; 27.584 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:37:37.021245: step 100800, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 28.494 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:38:06.401923: step 100900, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 29.073 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.94
Training Set Accuracy: 1.00
Adding run metadata for 101000
2019-05-23 12:39:01.819182: step 101100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 55.127 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:39:29.769779: step 101200, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 27.676 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:39:59.153838: step 101300, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 29.096 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:40:28.824185: step 101400, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 29.414 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:40:57.441808: step 101500, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 28.319 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:41:25.342299: step 101600, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 27.620 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:41:52.185303: step 101700, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.575 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:42:21.749357: step 101800, loss = 0.02  learning rate = 0.00  (1.1 examples/sec; 29.305 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:42:47.735345: step 101900, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 25.732 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.94
Training Set Accuracy: 1.00
Adding run metadata for 102000
2019-05-23 12:43:38.750219: step 102100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 50.762 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:44:04.201335: step 102200, loss = 0.06  learning rate = 0.00  (1.3 examples/sec; 25.209 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:44:33.144820: step 102300, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 28.610 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:45:00.524231: step 102400, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 27.122 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:45:27.182126: step 102500, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.410 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:45:54.310189: step 102600, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.801 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:46:20.425176: step 102700, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 25.857 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:46:46.240067: step 102800, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.563 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:47:12.235926: step 102900, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 25.755 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.93
Training Set Accuracy: 1.00
Adding run metadata for 103000
2019-05-23 12:48:04.921493: step 103100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 52.426 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:48:31.007456: step 103200, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 25.837 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:48:59.272798: step 103300, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 28.024 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:49:26.164200: step 103400, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.602 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:49:55.340887: step 103500, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 28.841 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:50:25.068097: step 103600, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 29.172 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:50:54.107625: step 103700, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 28.715 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:51:23.133302: step 103800, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 28.768 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:51:51.583099: step 103900, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 28.131 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.98
Training Set Accuracy: 1.00
Adding run metadata for 104000
2019-05-23 12:52:49.092018: step 104100, loss = 0.03  learning rate = 0.00  (0.6 examples/sec; 57.259 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:53:16.119966: step 104200, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.785 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:53:44.525915: step 104300, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 28.135 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:54:10.774098: step 104400, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 25.994 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:54:37.637890: step 104500, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.574 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:55:04.015808: step 104600, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.121 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:55:32.269380: step 104700, loss = 0.06  learning rate = 0.00  (1.1 examples/sec; 27.954 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:55:59.219046: step 104800, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.653 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:56:25.697821: step 104900, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.234 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.97
Training Set Accuracy: 1.00
Adding run metadata for 105000
2019-05-23 12:57:20.007198: step 105100, loss = 0.05  learning rate = 0.00  (0.6 examples/sec; 54.056 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:57:46.330140: step 105200, loss = 0.02  learning rate = 0.00  (1.2 examples/sec; 26.061 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:58:12.939517: step 105300, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.352 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:58:38.928187: step 105400, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 25.714 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:59:06.024002: step 105500, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.835 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:59:32.099089: step 105600, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 25.825 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 12:59:58.144892: step 105700, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 25.791 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:00:27.591885: step 105800, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 29.209 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:00:54.485580: step 105900, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.644 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.94
Training Set Accuracy: 1.00
Adding run metadata for 106000
2019-05-23 13:01:48.666766: step 106100, loss = 0.03  learning rate = 0.00  (0.6 examples/sec; 53.831 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:02:16.840672: step 106200, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 27.918 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:02:43.948522: step 106300, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.852 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:03:12.205372: step 106400, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 28.012 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:03:37.918182: step 106500, loss = 0.07  learning rate = 0.00  (1.3 examples/sec; 25.426 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:04:03.793992: step 106600, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 25.636 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:04:29.662442: step 106700, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 25.601 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:04:55.558212: step 106800, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 25.644 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:05:22.073543: step 106900, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.265 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.93
Training Set Accuracy: 1.00
Adding run metadata for 107000
2019-05-23 13:06:14.544309: step 107100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 52.222 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:06:39.986122: step 107200, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.197 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:07:05.332291: step 107300, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.082 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:07:30.510862: step 107400, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.930 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:07:55.596370: step 107500, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.842 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:08:20.778157: step 107600, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.929 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:08:45.772886: step 107700, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.746 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:09:10.846449: step 107800, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.812 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:09:35.948920: step 107900, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 24.858 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.94
Training Set Accuracy: 1.00
Adding run metadata for 108000
2019-05-23 13:10:26.917900: step 108100, loss = 0.06  learning rate = 0.00  (0.6 examples/sec; 50.693 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:10:51.720180: step 108200, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.553 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:11:16.815609: step 108300, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.842 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:11:41.814385: step 108400, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.752 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:12:06.825400: step 108500, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.766 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:12:31.835718: step 108600, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.761 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:12:56.960591: step 108700, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 24.871 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:13:22.144884: step 108800, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 24.936 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:13:50.595147: step 108900, loss = 0.06  learning rate = 0.00  (1.1 examples/sec; 28.172 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.94
Training Set Accuracy: 1.00
Adding run metadata for 109000
2019-05-23 13:14:43.871277: step 109100, loss = 0.06  learning rate = 0.00  (0.6 examples/sec; 53.020 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:15:10.557423: step 109200, loss = 0.02  learning rate = 0.00  (1.2 examples/sec; 26.328 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:15:37.365746: step 109300, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.484 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:16:04.346556: step 109400, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.726 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:16:32.121516: step 109500, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 27.532 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:16:59.778901: step 109600, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 27.363 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:17:26.641662: step 109700, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.542 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:17:55.040995: step 109800, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 28.143 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:18:23.225687: step 109900, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 27.885 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.91
Training Set Accuracy: 1.00
Adding run metadata for 110000
2019-05-23 13:19:18.287989: step 110100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 54.756 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:19:46.815749: step 110200, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 28.193 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:20:14.486577: step 110300, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 27.371 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:20:43.722924: step 110400, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 28.915 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:21:11.693257: step 110500, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 27.677 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:21:44.275503: step 110600, loss = 0.02  learning rate = 0.00  (1.0 examples/sec; 32.325 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:22:11.601543: step 110700, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 27.043 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:22:38.936589: step 110800, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 27.059 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:23:08.075716: step 110900, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 28.763 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.93
Training Set Accuracy: 1.00
Adding run metadata for 111000
2019-05-23 13:24:02.724028: step 111100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 54.385 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:24:29.150491: step 111200, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 26.182 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:24:56.281695: step 111300, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 26.874 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:25:24.554342: step 111400, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 28.017 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:25:51.915793: step 111500, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 27.110 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:26:20.103576: step 111600, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 27.916 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:26:50.057710: step 111700, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 29.704 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:27:17.076642: step 111800, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 26.770 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:27:43.698761: step 111900, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.369 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.96
Training Set Accuracy: 1.00
Adding run metadata for 112000
2019-05-23 13:28:36.106809: step 112100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 52.150 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:29:02.101138: step 112200, loss = 0.07  learning rate = 0.00  (1.2 examples/sec; 25.736 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:29:28.216554: step 112300, loss = 0.07  learning rate = 0.00  (1.2 examples/sec; 25.860 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:29:54.250195: step 112400, loss = 0.08  learning rate = 0.00  (1.2 examples/sec; 25.780 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:30:20.539643: step 112500, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.029 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:30:46.154507: step 112600, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.356 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:31:12.127372: step 112700, loss = 0.01  learning rate = 0.00  (1.2 examples/sec; 25.726 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:31:38.060157: step 112800, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 25.675 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:32:04.179073: step 112900, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 25.870 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.95
Training Set Accuracy: 1.00
Adding run metadata for 113000
2019-05-23 13:32:56.290311: step 113100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 51.861 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:33:22.069394: step 113200, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.524 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:33:48.217913: step 113300, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 25.847 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:34:14.838254: step 113400, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 26.362 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:34:41.392044: step 113500, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.314 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:35:07.599773: step 113600, loss = 0.02  learning rate = 0.00  (1.2 examples/sec; 25.931 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:35:37.665993: step 113700, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 29.803 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:36:04.536291: step 113800, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.582 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:36:31.905334: step 113900, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 27.105 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.93
Training Set Accuracy: 1.00
Adding run metadata for 114000
2019-05-23 13:37:27.923217: step 114100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 55.668 sec/batch)
Minibatch accuracy2: 1.00

2019-05-23 13:37:54.288836: step 114200, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.118 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:38:21.920204: step 114300, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 27.289 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:38:50.916159: step 114400, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 28.736 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:39:19.493436: step 114500, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 28.314 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:39:47.728407: step 114600, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 27.940 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:40:15.116809: step 114700, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 27.095 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:40:43.640445: step 114800, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 28.207 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:41:11.784758: step 114900, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 27.900 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.91
Training Set Accuracy: 1.00
Adding run metadata for 115000
2019-05-23 13:42:08.223250: step 115100, loss = 0.05  learning rate = 0.00  (0.6 examples/sec; 56.124 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:42:38.356592: step 115200, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 29.878 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:43:05.679874: step 115300, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 27.003 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:43:33.635003: step 115400, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 27.677 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:43:59.852136: step 115500, loss = 0.02  learning rate = 0.00  (1.2 examples/sec; 25.959 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:44:24.861404: step 115600, loss = 0.02  learning rate = 0.00  (1.3 examples/sec; 24.760 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:44:50.131679: step 115700, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.026 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:45:15.771285: step 115800, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 25.370 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:45:41.456864: step 115900, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 25.436 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.96
Training Set Accuracy: 1.00
Adding run metadata for 116000
2019-05-23 13:46:32.732331: step 116100, loss = 0.04  learning rate = 0.00  (0.6 examples/sec; 51.025 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:46:58.195819: step 116200, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.218 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:47:23.620557: step 116300, loss = 0.06  learning rate = 0.00  (1.3 examples/sec; 25.169 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:47:48.934676: step 116400, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 25.067 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:48:14.761405: step 116500, loss = 0.05  learning rate = 0.00  (1.3 examples/sec; 25.577 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:48:40.812756: step 116600, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 25.757 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:49:08.447629: step 116700, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 27.376 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:49:38.821049: step 116800, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 30.101 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:50:05.159282: step 116900, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 26.055 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.91
Training Set Accuracy: 1.00
Adding run metadata for 117000
2019-05-23 13:50:59.942951: step 117100, loss = 0.03  learning rate = 0.00  (0.6 examples/sec; 54.529 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:51:27.422408: step 117200, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 27.225 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:51:54.195165: step 117300, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 26.521 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:52:22.999413: step 117400, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 28.514 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:52:52.732315: step 117500, loss = 0.05  learning rate = 0.00  (1.1 examples/sec; 29.400 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:53:21.311968: step 117600, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 28.332 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:53:49.516167: step 117700, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 27.904 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:54:17.569535: step 117800, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 27.754 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:54:45.720209: step 117900, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 27.848 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.92
Training Set Accuracy: 1.00
Adding run metadata for 118000
2019-05-23 13:55:43.620312: step 118100, loss = 0.03  learning rate = 0.00  (0.6 examples/sec; 57.639 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:56:10.515829: step 118200, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 26.641 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:56:37.841880: step 118300, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 27.054 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:57:05.174831: step 118400, loss = 0.02  learning rate = 0.00  (1.2 examples/sec; 27.031 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:57:31.692750: step 118500, loss = 0.05  learning rate = 0.00  (1.2 examples/sec; 26.261 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:57:57.566537: step 118600, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 25.613 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:58:23.647034: step 118700, loss = 0.07  learning rate = 0.00  (1.2 examples/sec; 25.828 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:58:49.426024: step 118800, loss = 0.03  learning rate = 0.00  (1.3 examples/sec; 25.522 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 13:59:15.216308: step 118900, loss = 0.04  learning rate = 0.00  (1.3 examples/sec; 25.522 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.96
Training Set Accuracy: 1.00
Adding run metadata for 119000
2019-05-23 14:00:08.072655: step 119100, loss = 0.05  learning rate = 0.00  (0.6 examples/sec; 52.592 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 14:00:34.354755: step 119200, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.027 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 14:01:04.553130: step 119300, loss = 0.04  learning rate = 0.00  (1.1 examples/sec; 29.754 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 14:01:31.866994: step 119400, loss = 0.06  learning rate = 0.00  (1.2 examples/sec; 27.059 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 14:01:58.184319: step 119500, loss = 0.04  learning rate = 0.00  (1.2 examples/sec; 26.070 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 14:02:25.476619: step 119600, loss = 0.03  learning rate = 0.00  (1.2 examples/sec; 27.045 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 14:02:53.590664: step 119700, loss = 0.06  learning rate = 0.00  (1.1 examples/sec; 27.829 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 14:03:23.723585: step 119800, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 29.842 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 14:03:52.470473: step 119900, loss = 0.03  learning rate = 0.00  (1.1 examples/sec; 28.464 sec/batch)
Minibatch accuracy2: 1.00
Validation Accuracy: 0.92
Training Set Accuracy: 1.00
Adding run metadata for 120000
2019-05-23 14:04:53.428661: step 120100, loss = 0.04  learning rate = 0.00  (0.5 examples/sec; 60.703 sec/batch)
Minibatch accuracy2: 1.00
2019-05-23 14:05:21.610912: step 120200, loss = 0.02  learning rate = 0.00  (1.1 examples/sec; 27.926 sec/batch)
Minibatch accuracy2: 1.00
Test accuracy: 0.93