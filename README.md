import time

def get_input(prompt):
    return input(prompt).strip()

def main():
    print("欢迎使用表白程序！")
    time.sleep(1)
    
    # 获取用户输入
    name = get_input("请输入对方的名字: ")
    favorite_color = get_input("请输入对方最喜欢的颜色: ")
    favorite_food = get_input("请输入对方最喜欢的食物: ")
    special_memory = get_input("请输入你们之间的一段特别回忆: ")
    
    time.sleep(1)
    print("\n生成你的表白信息中...\n")
    time.sleep(2)
    
    # 生成表白信息
    confession = (
        f"亲爱的{name}，\n\n"
        f"从我们第一次见面，我就知道你是特别的。你的微笑像是{favorite_color}的阳光，"
        f"照亮了我的每一天。每次我们一起享受{favorite_food}，我都感到无比的幸福。\n\n"
        f"我永远不会忘记我们一起经历的那个特别时刻：{special_memory}。"
        f"那一刻，我意识到你就是我想要共度一生的人。\n\n"
        f"{name}，我希望未来的每一天都有你在我身边。让我们一起创造更多美好的回忆吧！\n\n"
        f"爱你的，\n[你的名字]"
    )
    
    print(confession)

if __name__ == "__main__":
    main()
