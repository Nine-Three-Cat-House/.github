# **🐱 Nine Three Cattery (九三猫舍)**

**“We don't change the world, we sleep on it.”**

**我们不改变世界，我们踩在世界上睡觉。**

[📖 关于项目](https://dictionary.cambridge.org/zhs/%E8%AF%8D%E5%85%B8/%E8%8B%B1%E8%AF%AD-%E6%B1%89%E8%AF%AD-%E7%AE%80%E4%BD%93/about) • [🚀 核心架构](https://dictionary.cambridge.org/zhs/%E8%AF%8D%E5%85%B8/%E8%8B%B1%E8%AF%AD-%E6%B1%89%E8%AF%AD-%E7%AE%80%E4%BD%93/architecture) • [⚙️ 组织模块](https://dictionary.cambridge.org/zhs/%E8%AF%8D%E5%85%B8/%E8%8B%B1%E8%AF%AD-%E6%B1%89%E8%AF%AD-%E7%AE%80%E4%BD%93/module) • [📦 安装指南](https://dictionary.cambridge.org/zhs/%E8%AF%8D%E5%85%B8/%E8%8B%B1%E8%AF%AD-%E6%B1%89%E8%AF%AD-%E7%AE%80%E4%BD%93/installation) • [🤝 贡献代码](https://dictionary.cambridge.org/zhs/%E8%AF%8D%E5%85%B8/%E8%8B%B1%E8%AF%AD-%E6%B1%89%E8%AF%AD-%E7%AE%80%E4%BD%93/contribution)

## **📖 About (关于项目)**

**九三猫舍 (Nine Three Cattery a.k.a. Nine Three Cat House / Jiusan Cat Society)** 是一个基于生物本能的去中心化自治组织 (DAO)，致力于维护人类作为铲屎官的基本尊严（如有），并探索宇宙终极真理。

本项目不生产猫，仅提供被猫统治的运行时环境 (Runtime Environment)。

### **核心哲学 (Core Philosophy)**

**警告**：本项目具有高度成瘾性，且存在严重的内存泄漏（Memory Leak），具体表现为家里的猫粮总是莫名其妙消失。

* **九 (Nine)**: Max\_Lives \= 9 —— 冗余生命系统，容错率极高。
* **三 (Three)**: 三大核心线程 —— Eat(), Sleep(), Rot() (摆烂)。
* **猫舍 (Cattery)**: 也就是你的家，现在是狐务器机房 🦊。

## **🚀 Architecture (核心架构)**

本项目基于 **Pythonic Laziness** 逻辑构建。以下是系统的核心循环逻辑：

```Python
class JiusanCatSociety:
    def __init__(self):
        self.boss = "Cat"
        self.servant = "Human"
        self.logic = None  # Deprecated
    
    def main_loop(self):
        while True:
            status = self.check_cat_status()
            
            if status == "HUNGRY":
                Human.open_can(speed="MAX")
            elif status == "BORED":
                Human.push_item_off_table(target="Water Cup")
            elif status == "ZOOMIES":
                # 凌晨3点执行跑酷协议
                World.simulate_earthquake(time="03:00 AM")
            else:
                # 默认状态：占用键盘
                self.occupy_keyboard()
    
    def handle_error(self):
        print("错误：猫永远是对的。")
        raise HumanFaultException("请反思你自己")
```

### **依赖关系图 (Dependency Graph)**

```
graph TD
    A[👑 猫 (Root User)] -->|统治| B(人类)
    B -->|生产罐头| A
    B -->|提供膝盖| A
    B -->|清理猫砂| A
    
    subgraph 核心资源
    C[纸箱]
    D[阳光]
    E[键盘]
    end  
    
    A -->|霸占| C
    A -->|追逐| D
    A -->|踩踏| E
```

## **⚙️ Modules (组织模块)**

我们在 src/departments 下维护以下核心微服务：

| 模块名称 | 状态 | 描述 | 负责人 |
| :---- | :---- | :---- | :---- |
| **Sunlight\_Committee** (中央晒太阳委员会) | 🟢 Running | 追踪全屋光照变化，实现自动寻热导航。 | 三花猫 |
| **Parkour\_Monitor** (夜间跑酷监察司) | 🟡 Idle | 负责在 03:00 AM 准时唤醒人类，测试其心率。🐱：三点几啦，饮茶先啦。 | 缅因猫 |
| **Budget\_Audit** (猫粮预算审计处) | 🔴 Overflow | 无论预算多少，永远显示“资金不足”。 | 橘猫 |
| **Gravity\_Test** (重力势能测试局) | 🟢 Active | 验证地球引力，将桌上物品推落。 | 狸花猫 |

## **📦 Installation (入社/安装指南)**

想要将本项目 Deploy 到您的生活中，请确保满足以下依赖：

### **Prerequisites (环境要求)**

* **OS**: 任何物理空间（推荐：狭窄的缝隙）。  
* **Hardware**: 一个温暖的膝盖 (Knee v2.0+)。  
* **Software**: 无限的耐心 (Patience Unlimited Edition)。

### **Setup (配置)**

在您的 mindset.config.json 中添加以下配置：

```JSON
{
  "allow_scratching": true,
  "dignity_level": 0,
  "accept_hairballs": "always",
  "ideology": "Cat is God"
}
```

运行安装命令：

```zsh
# 注意：此操作不可撤销  
npm install cat-lord --global --save-dev
```

## **🤝 Contributing (贡献指南)**

我们非常欢迎 Pull Requests，但请遵循以下 **Code of Conduct**：

1. **Issue 提交**：如果你发现猫咬人，这不是 Bug，是 Feature。请勿提交 Issue。  
2. **代码合并**：任何试图让猫洗澡的代码 (wash\_cat.exe) 都会导致分支冲突并引发流血事件。  
3. **赞助项目**：我们接受 Freeze-dried chicken (冻干鸡肉) 和 Canned Tuna (金枪鱼罐头) 作为捐赠。

### **荣誉贡献者**

* **Zongmin Zhang (Nagato)**: 首席铲屎官 / 长期饭票。  

## **📄 License**

本项目采用 [**WTFPL**](https://www.wtfpl.net/) (Do What The F\*ck You Want To Public License) 修改版：

* 你可以保持沉默。
* 但你所说的一切都将被猫咪无视。
* 最终解释权归 **一只对世界毫不在乎的猫** 所有。

**Star ⭐ this repo if you are currently serving a cat.**

Designed with ❤️ by Zongmin Zhang (Nagato)

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
