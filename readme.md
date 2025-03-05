<div align="left">
    <img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="40%" align="left" style="margin-right: 15px"/>
    <div style="display: inline-block;">
        <h2 style="display: inline-block; vertical-align: middle; margin-top: 0;">YOLO-KAN</h2>
        <p>
</p>
        <p>
	<img src="https://img.shields.io/github/license/shankswhite/YOLO-KAN?style=flat-square&logo=opensourceinitiative&logoColor=white&color=A931EC" alt="license">
	<img src="https://img.shields.io/github/last-commit/shankswhite/YOLO-KAN?style=flat-square&logo=git&logoColor=white&color=A931EC" alt="last-commit">
	<img src="https://img.shields.io/github/languages/top/shankswhite/YOLO-KAN?style=flat-square&color=A931EC" alt="repo-top-language">
	<img src="https://img.shields.io/github/languages/count/shankswhite/YOLO-KAN?style=flat-square&color=A931EC" alt="repo-language-count">

<br clear="left"/>

##  Authors

Xiaofeng Zhao, NEU CS Student



Themina Amjad, NEU Professor



Jeongkyu Lee, NEU Professor

---

##  Overview

<code>❯ Traditional Multi-Layer Perceptrons (MLPs) typically employ fixed activation functions and large weight matrices to learn the complex patterns present in these representations. This leads towards large growth in parameters but decreases the interpretability of the model. Kolmogorov-Arnold Networks (KANs) instead employ learnable activation functions inspired by the Kolmogorov–Arnold representation theorem, which is a more flexible way to model nonlinear relationships without inflating the counts of parameters excessively. This study proposes YOLO-KAN, a model based on YOLOv11n, where newly designed KAN modules replace portions of the traditional MLP structures of the backbone. The ablation experiments show that one of the proposed YOLO-KAN models achieves a 1.84\% improvement in precision over the yolov11n model in the COCO dataset. These findings suggest that KANs can match or surpass traditional MLPs in computer vision object detection, including large-scale datasets such as COCO. The result can help the community in designing versatile, real-time object detectors for a range of object recognition tasks.</code>

---

##  Architecture

![yolo-arch]<img width="1216" alt="yolo-kan-arch" src="https://github.com/user-attachments/assets/ac396832-e416-4426-a0a2-67d4dfea944f" />




![yolo-kan-flatten](https://github.com/user-attachments/assets/0cfaf4c8-1f0b-4b7a-8b24-4603cf8564b4)


---

##  Project Structure

```sh
└── YOLO-KAN/
    ├── .github
    │   ├── ISSUE_TEMPLATE
    │   ├── dependabot.yml
    │   └── workflows
    ├── 11-1-7.pt
    ├── 11-2-1.pt
    ├── 11-2-3.pt
    ├── 11-2-5-2.pt
    ├── 11-2-5.pt
    ├── 11-2-7.pt
    ├── 11-2-depthwise.pt
    ├── 11-2-maxpool.pt
    ├── 11-official-2.pt
    ├── 11-official.pt
    ├── CITATION.cff
    ├── CONTRIBUTING.md
    ├── LICENSE
    ├── README.md
    ├── README.zh-CN.md
    ├── docker
    │   ├── Dockerfile
    │   ├── Dockerfile-arm64
    │   ├── Dockerfile-conda
    │   ├── Dockerfile-cpu
    │   ├── Dockerfile-jetson-jetpack4
    │   ├── Dockerfile-jetson-jetpack5
    │   ├── Dockerfile-jetson-jetpack6
    │   ├── Dockerfile-python
    │   └── Dockerfile-runner
    ├── docs
    │   ├── README.md
    │   ├── build_docs.py
    │   ├── build_reference.py
    │   ├── coming_soon_template.md
    │   ├── en
    │   ├── mkdocs_github_authors.yaml
    │   └── overrides
    ├── examples
    │   ├── README.md
    │   ├── YOLOv8-Action-Recognition
    │   ├── YOLOv8-CPP-Inference
    │   ├── YOLOv8-LibTorch-CPP-Inference
    │   ├── YOLOv8-ONNXRuntime
    │   ├── YOLOv8-ONNXRuntime-CPP
    │   ├── YOLOv8-ONNXRuntime-Rust
    │   ├── YOLOv8-OpenCV-ONNX-Python
    │   ├── YOLOv8-OpenCV-int8-tflite-Python
    │   ├── YOLOv8-OpenVINO-CPP-Inference
    │   ├── YOLOv8-Region-Counter
    │   ├── YOLOv8-SAHI-Inference-Video
    │   ├── YOLOv8-Segmentation-ONNXRuntime-Python
    │   ├── heatmaps.ipynb
    │   ├── hub.ipynb
    │   ├── object_counting.ipynb
    │   ├── object_tracking.ipynb
    │   └── tutorial.ipynb
    ├── exp10-new
    │   ├── yolov8n-c3k2-6
    │   └── yolov8n-c3k2-62
    ├── export.py
    ├── get_COCO_metrice.py
    ├── get_FPS.py
    ├── get_model_erf.py
    ├── heatmap.py
    ├── main_profile.py
    ├── mkdocs.yml
    ├── plot_result.py
    ├── pyproject.toml
    ├── tests
    │   ├── __init__.py
    │   ├── conftest.py
    │   ├── test_cli.py
    │   ├── test_cuda.py
    │   ├── test_engine.py
    │   ├── test_explorer.py
    │   ├── test_exports.py
    │   ├── test_integrations.py
    │   ├── test_python.py
    │   └── test_solutions.py
    ├── text.py
    ├── train.py
    ├── ultralytics
    │   ├── __init__.py
    │   ├── assets
    │   ├── cfg
    │   ├── data
    │   ├── engine
    │   ├── hub
    │   ├── models
    │   ├── nn
    │   ├── solutions
    │   ├── trackers
    │   └── utils
    ├── val.py
    ├── yolo2coco.py
    └── yolov11.py
```


###  Project Index
<details open>
	<summary><b><code>YOLO-KAN/</code></b></summary>
	<details> <!-- __root__ Submodule -->
		<summary><b>__root__</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/get_COCO_metrice.py'>get_COCO_metrice.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/heatmap.py'>heatmap.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/mkdocs.yml'>mkdocs.yml</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/CITATION.cff'>CITATION.cff</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/val.py'>val.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/yolo2coco.py'>yolo2coco.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/11-2-1.pt'>11-2-1.pt</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/pyproject.toml'>pyproject.toml</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/11-2-5.pt'>11-2-5.pt</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/get_FPS.py'>get_FPS.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/export.py'>export.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/11-1-7.pt'>11-1-7.pt</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/11-official.pt'>11-official.pt</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/11-2-7.pt'>11-2-7.pt</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/11-2-5-2.pt'>11-2-5-2.pt</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/yolov11.py'>yolov11.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/plot_result.py'>plot_result.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/get_model_erf.py'>get_model_erf.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/11-2-3.pt'>11-2-3.pt</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/main_profile.py'>main_profile.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/11-official-2.pt'>11-official-2.pt</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/text.py'>text.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/train.py'>train.py</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/11-2-maxpool.pt'>11-2-maxpool.pt</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/11-2-depthwise.pt'>11-2-depthwise.pt</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			</table>
		</blockquote>
	</details>
	<details> <!-- docker Submodule -->
		<summary><b>docker</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/docker/Dockerfile-runner'>Dockerfile-runner</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/docker/Dockerfile-arm64'>Dockerfile-arm64</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/docker/Dockerfile'>Dockerfile</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/docker/Dockerfile-jetson-jetpack4'>Dockerfile-jetson-jetpack4</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/docker/Dockerfile-jetson-jetpack5'>Dockerfile-jetson-jetpack5</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/docker/Dockerfile-python'>Dockerfile-python</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/docker/Dockerfile-jetson-jetpack6'>Dockerfile-jetson-jetpack6</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/docker/Dockerfile-cpu'>Dockerfile-cpu</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/docker/Dockerfile-conda'>Dockerfile-conda</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			</table>
		</blockquote>
	</details>
	<details> <!-- exp10-new Submodule -->
		<summary><b>exp10-new</b></summary>
		<blockquote>
			<details>
				<summary><b>yolov8n-c3k2-62</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/exp10-new/yolov8n-c3k2-62/args.yaml'>args.yaml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/exp10-new/yolov8n-c3k2-62/events.out.tfevents.1728025389.DESKTOP-H91QBA0.1196.0'>events.out.tfevents.1728025389.DESKTOP-H91QBA0.1196.0</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>yolov8n-c3k2-6</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/exp10-new/yolov8n-c3k2-6/args.yaml'>args.yaml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
		</blockquote>
	</details>
	<details> <!-- examples Submodule -->
		<summary><b>examples</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/hub.ipynb'>hub.ipynb</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/object_counting.ipynb'>object_counting.ipynb</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/object_tracking.ipynb'>object_tracking.ipynb</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/heatmaps.ipynb'>heatmaps.ipynb</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/tutorial.ipynb'>tutorial.ipynb</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			</table>
			<details>
				<summary><b>YOLOv8-CPP-Inference</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-CPP-Inference/inference.h'>inference.h</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-CPP-Inference/CMakeLists.txt'>CMakeLists.txt</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-CPP-Inference/main.cpp'>main.cpp</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-CPP-Inference/inference.cpp'>inference.cpp</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>YOLOv8-SAHI-Inference-Video</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-SAHI-Inference-Video/yolov8_sahi.py'>yolov8_sahi.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>YOLOv8-LibTorch-CPP-Inference</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-LibTorch-CPP-Inference/main.cc'>main.cc</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-LibTorch-CPP-Inference/CMakeLists.txt'>CMakeLists.txt</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>YOLOv8-Region-Counter</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-Region-Counter/yolov8_region_counter.py'>yolov8_region_counter.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>YOLOv8-OpenCV-ONNX-Python</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-OpenCV-ONNX-Python/main.py'>main.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>YOLOv8-OpenCV-int8-tflite-Python</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-OpenCV-int8-tflite-Python/main.py'>main.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>YOLOv8-ONNXRuntime</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-ONNXRuntime/main.py'>main.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>YOLOv8-Action-Recognition</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-Action-Recognition/action_recognition.py'>action_recognition.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>YOLOv8-OpenVINO-CPP-Inference</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-OpenVINO-CPP-Inference/main.cc'>main.cc</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-OpenVINO-CPP-Inference/inference.h'>inference.h</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-OpenVINO-CPP-Inference/CMakeLists.txt'>CMakeLists.txt</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-OpenVINO-CPP-Inference/inference.cc'>inference.cc</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>YOLOv8-ONNXRuntime-CPP</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-ONNXRuntime-CPP/inference.h'>inference.h</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-ONNXRuntime-CPP/CMakeLists.txt'>CMakeLists.txt</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-ONNXRuntime-CPP/main.cpp'>main.cpp</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-ONNXRuntime-CPP/inference.cpp'>inference.cpp</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>YOLOv8-Segmentation-ONNXRuntime-Python</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-Segmentation-ONNXRuntime-Python/main.py'>main.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>YOLOv8-ONNXRuntime-Rust</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-ONNXRuntime-Rust/Cargo.toml'>Cargo.toml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
					<details>
						<summary><b>src</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-ONNXRuntime-Rust/src/yolo_result.rs'>yolo_result.rs</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-ONNXRuntime-Rust/src/lib.rs'>lib.rs</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-ONNXRuntime-Rust/src/main.rs'>main.rs</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-ONNXRuntime-Rust/src/ort_backend.rs'>ort_backend.rs</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-ONNXRuntime-Rust/src/model.rs'>model.rs</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/examples/YOLOv8-ONNXRuntime-Rust/src/cli.rs'>cli.rs</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							</table>
						</blockquote>
					</details>
				</blockquote>
			</details>
		</blockquote>
	</details>
	<details> <!-- .github Submodule -->
		<summary><b>.github</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/.github/dependabot.yml'>dependabot.yml</a></b></td>
				<td><code>❯ REPLACE-ME</code></td>
			</tr>
			</table>
			<details>
				<summary><b>workflows</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/.github/workflows/ci.yaml'>ci.yaml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/.github/workflows/links.yml'>links.yml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/.github/workflows/publish.yml'>publish.yml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/.github/workflows/format.yml'>format.yml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/.github/workflows/cla.yml'>cla.yml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/.github/workflows/stale.yml'>stale.yml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/.github/workflows/merge-main-into-prs.yml'>merge-main-into-prs.yml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/.github/workflows/docs.yml'>docs.yml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/.github/workflows/docker.yaml'>docker.yaml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/.github/workflows/codeql.yaml'>codeql.yaml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>ISSUE_TEMPLATE</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/.github/ISSUE_TEMPLATE/bug-report.yml'>bug-report.yml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/.github/ISSUE_TEMPLATE/config.yml'>config.yml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/.github/ISSUE_TEMPLATE/feature-request.yml'>feature-request.yml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/.github/ISSUE_TEMPLATE/question.yml'>question.yml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
		</blockquote>
	</details>
	<details> <!-- ultralytics Submodule -->
		<summary><b>ultralytics</b></summary>
		<blockquote>
			<details>
				<summary><b>nn</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/nn/tasks.py'>tasks.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/nn/autobackend.py'>autobackend.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
					<details>
						<summary><b>modules</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/nn/modules/activation.py'>activation.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/nn/modules/utils.py'>utils.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/nn/modules/transformer.py'>transformer.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/nn/modules/head.py'>head.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/nn/modules/conv.py'>conv.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/nn/modules/block.py'>block.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							</table>
						</blockquote>
					</details>
				</blockquote>
			</details>
			<details>
				<summary><b>solutions</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/solutions/heatmap.py'>heatmap.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/solutions/distance_calculation.py'>distance_calculation.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/solutions/object_counter.py'>object_counter.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/solutions/queue_management.py'>queue_management.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/solutions/parking_management.py'>parking_management.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/solutions/ai_gym.py'>ai_gym.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/solutions/streamlit_inference.py'>streamlit_inference.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/solutions/analytics.py'>analytics.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/solutions/speed_estimation.py'>speed_estimation.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>utils</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/instance.py'>instance.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/metrics.py'>metrics.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/files.py'>files.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/triton.py'>triton.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/autobatch.py'>autobatch.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/checks.py'>checks.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/plotting.py'>plotting.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/downloads.py'>downloads.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/tal.py'>tal.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/ops.py'>ops.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/loss.py'>loss.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/patches.py'>patches.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/errors.py'>errors.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/tuner.py'>tuner.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/benchmarks.py'>benchmarks.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/dist.py'>dist.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/torch_utils.py'>torch_utils.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
					<details>
						<summary><b>callbacks</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/callbacks/comet.py'>comet.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/callbacks/wb.py'>wb.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/callbacks/mlflow.py'>mlflow.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/callbacks/clearml.py'>clearml.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/callbacks/raytune.py'>raytune.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/callbacks/dvc.py'>dvc.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/callbacks/hub.py'>hub.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/callbacks/base.py'>base.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/callbacks/tensorboard.py'>tensorboard.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/utils/callbacks/neptune.py'>neptune.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							</table>
						</blockquote>
					</details>
				</blockquote>
			</details>
			<details>
				<summary><b>models</b></summary>
				<blockquote>
					<details>
						<summary><b>fastsam</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/fastsam/val.py'>val.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/fastsam/predict.py'>predict.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/fastsam/model.py'>model.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/fastsam/utils.py'>utils.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							</table>
						</blockquote>
					</details>
					<details>
						<summary><b>sam</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/sam/build.py'>build.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/sam/amg.py'>amg.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/sam/predict.py'>predict.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/sam/model.py'>model.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							</table>
							<details>
								<summary><b>modules</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/sam/modules/decoders.py'>decoders.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/sam/modules/memory_attention.py'>memory_attention.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/sam/modules/encoders.py'>encoders.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/sam/modules/utils.py'>utils.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/sam/modules/transformer.py'>transformer.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/sam/modules/blocks.py'>blocks.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/sam/modules/tiny_encoder.py'>tiny_encoder.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/sam/modules/sam.py'>sam.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									</table>
								</blockquote>
							</details>
						</blockquote>
					</details>
					<details>
						<summary><b>nas</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/nas/val.py'>val.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/nas/predict.py'>predict.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/nas/model.py'>model.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							</table>
						</blockquote>
					</details>
					<details>
						<summary><b>utils</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/utils/ops.py'>ops.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/utils/loss.py'>loss.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							</table>
						</blockquote>
					</details>
					<details>
						<summary><b>yolo</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/model.py'>model.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							</table>
							<details>
								<summary><b>obb</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/obb/val.py'>val.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/obb/predict.py'>predict.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/obb/train.py'>train.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									</table>
								</blockquote>
							</details>
							<details>
								<summary><b>detect</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/detect/val.py'>val.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/detect/predict.py'>predict.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/detect/train.py'>train.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									</table>
								</blockquote>
							</details>
							<details>
								<summary><b>classify</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/classify/val.py'>val.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/classify/predict.py'>predict.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/classify/train.py'>train.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									</table>
								</blockquote>
							</details>
							<details>
								<summary><b>segment</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/segment/val.py'>val.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/segment/predict.py'>predict.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/segment/train.py'>train.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									</table>
								</blockquote>
							</details>
							<details>
								<summary><b>world</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/world/train_world.py'>train_world.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/world/train.py'>train.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									</table>
								</blockquote>
							</details>
							<details>
								<summary><b>pose</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/pose/val.py'>val.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/pose/predict.py'>predict.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/yolo/pose/train.py'>train.py</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									</table>
								</blockquote>
							</details>
						</blockquote>
					</details>
					<details>
						<summary><b>rtdetr</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/rtdetr/val.py'>val.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/rtdetr/predict.py'>predict.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/rtdetr/model.py'>model.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/models/rtdetr/train.py'>train.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							</table>
						</blockquote>
					</details>
				</blockquote>
			</details>
			<details>
				<summary><b>trackers</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/trackers/bot_sort.py'>bot_sort.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/trackers/track.py'>track.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/trackers/byte_tracker.py'>byte_tracker.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/trackers/basetrack.py'>basetrack.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
					<details>
						<summary><b>utils</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/trackers/utils/gmc.py'>gmc.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/trackers/utils/matching.py'>matching.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/trackers/utils/kalman_filter.py'>kalman_filter.py</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							</table>
						</blockquote>
					</details>
				</blockquote>
			</details>
			<details>
				<summary><b>cfg</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/default.yaml'>default.yaml</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
					<details>
						<summary><b>datasets</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/african-wildlife.yaml'>african-wildlife.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/DOTAv1.5.yaml'>DOTAv1.5.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/coco8.yaml'>coco8.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/coco128.yaml'>coco128.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/coco.yaml'>coco.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/coco128-seg.yaml'>coco128-seg.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/brain-tumor.yaml'>brain-tumor.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/coco-pose.yaml'>coco-pose.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/dota8.yaml'>dota8.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/GlobalWheat2020.yaml'>GlobalWheat2020.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/DOTAv1.yaml'>DOTAv1.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/crack-seg.yaml'>crack-seg.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/lvis.yaml'>lvis.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/VisDrone.yaml'>VisDrone.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/coco8-pose.yaml'>coco8-pose.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/hand-keypoints.yaml'>hand-keypoints.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/SKU-110K.yaml'>SKU-110K.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/Objects365.yaml'>Objects365.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/xView.yaml'>xView.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/Argoverse.yaml'>Argoverse.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/tiger-pose.yaml'>tiger-pose.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/open-images-v7.yaml'>open-images-v7.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/ImageNet.yaml'>ImageNet.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/signature.yaml'>signature.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/carparts-seg.yaml'>carparts-seg.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/package-seg.yaml'>package-seg.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/VOC.yaml'>VOC.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/datasets/coco8-seg.yaml'>coco8-seg.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							</table>
						</blockquote>
					</details>
					<details>
						<summary><b>models</b></summary>
						<blockquote>
							<details>
								<summary><b>v6</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v6/yolov6.yaml'>yolov6.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									</table>
								</blockquote>
							</details>
							<details>
								<summary><b>v8</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-seg.yaml'>yolov8-seg.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-ghost-p2.yaml'>yolov8-ghost-p2.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-p6.yaml'>yolov8-p6.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-seg-p6.yaml'>yolov8-seg-p6.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-cls-resnet50.yaml'>yolov8-cls-resnet50.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-worldv2.yaml'>yolov8-worldv2.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-rtdetr.yaml'>yolov8-rtdetr.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-obb.yaml'>yolov8-obb.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-pose.yaml'>yolov8-pose.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-cls-resnet101.yaml'>yolov8-cls-resnet101.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-p2.yaml'>yolov8-p2.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-ghost-p6.yaml'>yolov8-ghost-p6.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8.yaml'>yolov8.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-pose-p6.yaml'>yolov8-pose-p6.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-cls.yaml'>yolov8-cls.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-world.yaml'>yolov8-world.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v8/yolov8-ghost.yaml'>yolov8-ghost.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									</table>
								</blockquote>
							</details>
							<details>
								<summary><b>v9</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v9/yolov9e.yaml'>yolov9e.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v9/yolov9c.yaml'>yolov9c.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v9/yolov9t.yaml'>yolov9t.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v9/yolov9e-seg.yaml'>yolov9e-seg.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v9/yolov9m.yaml'>yolov9m.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v9/yolov9c-seg.yaml'>yolov9c-seg.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v9/yolov9s.yaml'>yolov9s.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									</table>
								</blockquote>
							</details>
							<details>
								<summary><b>rt-detr</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/rt-detr/rtdetr-l.yaml'>rtdetr-l.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/rt-detr/rtdetr-x.yaml'>rtdetr-x.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/rt-detr/rtdetr-resnet101.yaml'>rtdetr-resnet101.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/rt-detr/rtdetr-resnet50.yaml'>rtdetr-resnet50.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									</table>
								</blockquote>
							</details>
							<details>
								<summary><b>11</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/11/yolo11.yaml'>yolo11.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/11/yolo11-seg.yaml'>yolo11-seg.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/11/yolo11-pose.yaml'>yolo11-pose.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/11/yolo11-cls.yaml'>yolo11-cls.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/11/yolo11-KAN2.yaml'>yolo11-KAN2.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/11/yolo11-KAN.yaml'>yolo11-KAN.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/11/yolo11-KAN3.yaml'>yolo11-KAN3.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/11/yolo11-obb.yaml'>yolo11-obb.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									</table>
								</blockquote>
							</details>
							<details>
								<summary><b>v5</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v5/yolov5.yaml'>yolov5.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v5/yolov5-p6.yaml'>yolov5-p6.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									</table>
								</blockquote>
							</details>
							<details>
								<summary><b>v3</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v3/yolov3-spp.yaml'>yolov3-spp.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v3/yolov3-tiny.yaml'>yolov3-tiny.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v3/yolov3.yaml'>yolov3.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									</table>
								</blockquote>
							</details>
							<details>
								<summary><b>v10</b></summary>
								<blockquote>
									<table>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v10/yolov10b.yaml'>yolov10b.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v10/yolov10n.yaml'>yolov10n.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v10/yolov10m.yaml'>yolov10m.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v10/yolov10x.yaml'>yolov10x.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v10/yolov10l.yaml'>yolov10l.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									<tr>
										<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/models/v10/yolov10s.yaml'>yolov10s.yaml</a></b></td>
										<td><code>❯ REPLACE-ME</code></td>
									</tr>
									</table>
								</blockquote>
							</details>
						</blockquote>
					</details>
					<details>
						<summary><b>trackers</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/trackers/bytetrack.yaml'>bytetrack.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/cfg/trackers/botsort.yaml'>botsort.yaml</a></b></td>
								<td><code>❯ REPLACE-ME</code></td>
							</tr>
							</table>
						</blockquote>
					</details>
				</blockquote>
			</details>
			<details>
				<summary><b>engine</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/engine/validator.py'>validator.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/engine/predictor.py'>predictor.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/engine/results.py'>results.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/engine/exporter.py'>exporter.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/engine/model.py'>model.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/engine/trainer.py'>trainer.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/engine/tuner.py'>tuner.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
			<details>
				<summary><b>hub</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/hub/auth.py'>auth.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/hub/session.py'>session.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/shankswhite/YOLO-KAN/blob/master/ultralytics/hub/utils.py'>utils.py</a></b></td>
						<td><code>❯ REPLACE-ME</code></td>
					</tr>
					</table>
				</blockquote>
			</details>
		</blockquote>
	</details>
</details>

---
##  Getting Started

###  Prerequisites

Before getting started with YOLO-KAN, ensure your runtime environment meets the following requirements:

- **Programming Language:** Python, Ultralytics
- **Container Runtime:** Docker


###  Installation

Install YOLO-KAN using one of the following methods:

**Build from source:**

1. Clone the YOLO-KAN repository:
```sh
❯ git clone https://github.com/shankswhite/YOLO-KAN
```

2. Navigate to the project directory:
```sh
❯ cd YOLO-KAN
```

---
