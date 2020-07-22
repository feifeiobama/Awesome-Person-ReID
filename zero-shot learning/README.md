## Zero-shot learning notes

### Transductive zero-shot learning

| proc.   | title                                                        | method                                                       | motivation                                     |
| ------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ---------------------------------------------- |
| NIPS'19 | [Transductive Zero-Shot Learning with Visual Structure Constraint](https://papers.nips.cc/paper/9188-transductive-zero-shot-learning-with-visual-structure-constraint.pdf) | VSC: align unseen semantic centers and visual centers + filter out unrelated images | visual structure prior + unrelated test images |

### Generalized zero-shot learning

| proc.   | title                                                        | method                                                       | motivation                                     |
| ------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ---------------------------------------------- |
| CVPR'20 | [Generalized Zero-Shot Learning Via Over-Complete Distribution](https://arxiv.org/pdf/2004.00666.pdf) | OCD: generate hard samples between classes + OBTL & CL       | generated unseen class contains no hard sample |
| CVPR'20 | [Episode-based Prototype Generating Network for Zero-Shot Learning](https://arxiv.org/pdf/1909.03360.pdf) | E-PGN: simulate ZSL in each episode + visual-semantic interaction with CL | instability of generative approach             |
