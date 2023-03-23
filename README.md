# CTRAN: CNN-Transformer-based Network for Natural Language Understanding
Implementation on pytorch as described in <https://arxiv.org/abs/2303.10606>.

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/ctran-cnn-transformer-based-network-for/intent-detection-on-snips)](https://paperswithcode.com/sota/intent-detection-on-snips?p=ctran-cnn-transformer-based-network-for)[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/ctran-cnn-transformer-based-network-for/slot-filling-on-snips)](https://paperswithcode.com/sota/slot-filling-on-snips?p=ctran-cnn-transformer-based-network-for) <br>
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/ctran-cnn-transformer-based-network-for/slot-filling-on-atis)](https://paperswithcode.com/sota/slot-filling-on-atis?p=ctran-cnn-transformer-based-network-for)[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/ctran-cnn-transformer-based-network-for/intent-detection-on-atis)](https://paperswithcode.com/sota/intent-detection-on-atis?p=ctran-cnn-transformer-based-network-for)
## Introduction
![CTran CNN Transformer Model Architecture](https://github.com/rafiep/CTran/raw/main/.images/ctran.png)
We propose CTRAN, a novel CNN-Transformer-based encoder-decoder network. For the encoder, BERT is used as word embedding. Then, Convolutional layer is used on word embeddings and it's output is restructured using window feature sequence. The final part of the encoder is stacked Transformer encoders. The decoder comprises self-attention and a linear layer to produce output probabilities for Intent-detection. Finally, we propose Aligned Transformer Decoder followed by a fully connected layer for Slot-filling task.
## Requirements
- A Cuda capable GPU
- Python
- Pytorch
- Jupyter

## Dependencies
```
numpy==1.23.5
scikit_learn==1.2.2
torch==1.13.0
tqdm==4.64.1
transformers==4.25.1
```
## Runtime
On Windows 10 With an RTX 3080 and BERT~base~, the approximate training time for ATIS dataset is 46.71 seconds for each epoch.
On the same setup, SNIPS training time is 119.5 seconds for each loop.
## Citation
If you use any part of our code, please consider citing our paper as follows:
```
@article{rafiepour2023ctran,
  title={CTRAN: CNN-Transformer-based Network for Natural Language Understanding},
  author={Rafiepour, Mehrdad and Sartakhti, Javad Salimi},
  journal={arXiv preprint arXiv:2303.10606},
  year={2023}
}
```

## License
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)<br>
   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.

