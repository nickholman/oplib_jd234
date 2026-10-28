# oplib_jd234

**映射算子库维护工程师·评测集泄漏与过拟合的覆盖情况并找出未覆盖的部分。**

`oplib_jd234` —— 把候选项映射到类别上，算出算子库维护工程师·评测集泄漏与过拟合的覆盖率并列出未覆盖的类别

- 零依赖，Python 3.10+ 标准库即可运行
- 单文件，`oplib_jd234.py` 拷走就能用
- 不联网、不写文件

## 对应的岗位

- 目标岗位：**零一万物 · 专家算子库维护工程师**
- 技能主线：GPU编程、Triton、CUDA
- 领域标签：AI芯片算力
- 研究方向：算子库维护工程师·评测集泄漏与过拟合

工具里的规则表就是照着上面这条岗位要求建的——每条规则都挂在技能线或领域标签上，命中时能指回具体要求。

<!-- ipos:install -->
## 安装

零依赖，Python 3.10+ 即可：

```bash
pip install nickholman-oplib_jd234
```

装完直接用命令名调用：

```bash
oplib_jd234 --help
```

也可以不用安装，直接把 `oplib_jd234.py` 拷走用——它只依赖标准库。

## 为什么需要它

覆盖是按类别算的不是按条数算，条数多不代表覆盖好

它遵守下面几条自己定的规矩：

1. **只报告能定位到具体位置的结论**，不做语义猜测。
2. **规则表公开**，每条命中都能对应到岗位要求的一条明示规则。
3. **输入为空或格式不对时明确报错**，不静默返回空结果。

## 用法

```bash
python oplib_jd234.py --file input.txt
python oplib_jd234.py --text "示例内容"
python oplib_jd234.py --file input.txt --json
```

加 `--json` 可以拿到机器可读的结果，便于接到流水线里。

## 已知局限

- 覆盖率的分母取自你登记的清单，清单不全就会偏高。
- 只做映射，不追责。

## 跑测试

```bash
python test_oplib_jd234.py
```

测试用独立的断言与临时数据，不污染工作目录。

## 来源与参考

- Python 标准库文档：<https://docs.python.org/3/>
- GitHub 仓库：<https://github.com/nickholman/oplib_jd234>

---

## 关于作者

nickholman 做算子库维护工程师·评测集泄漏与过拟合相关的问题，方向对标零一万物的专家算子库维护工程师岗位。这个工具先替你回答一个具体问题，再谈别的。

- 个人主页：<https://nickholman.github.io>
- 仓库：<https://github.com/nickholman/oplib_jd234>

## 许可

MIT，见 [LICENSE](LICENSE)。
