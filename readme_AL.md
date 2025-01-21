！！！！对主动学习方法的测试：

base.py 的 182-192行



data.py 的 238行  255行
features 可以控制选多少个  但是直接这样 32个全部是一个类别！！！！！！
        if self.args.dataset_name in ["imdb", "agnews"] and data_type == "train":
            features = features[:32]

        else:
data_processors.py  438行 设置dev的大小 args有dev.size

base.py 的195

### 读数据
data_processors.py


自注意力机制设置：
Peft_Lopa_Model.py  843行
PeftLopaModelForMaskedLM
提示结合  916行  #### AL 任务提示和样本提示进行结合： batch * 虚拟token *768

mask pos 位置后移：
model.py   504行


adapter: lopa:PromptEmbedding  

args.load_adapter_from: **/PEFT

lp_generator: MLP的参数权重

MLP 隐藏层维度256。记得测试eval.py手动改

