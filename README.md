使用Python编写衬衣管理软件
在当今的数字化时代，管理库存变得越来越重要。为了有效地管理衬衣库存，我们可以编写一个简单的软件应用。本文将介绍如何使用Python编写一个基本的衬衣管理软件，涵盖衬衣的添加、删除、更新和查询功能。

1. 环境准备
首先，确保你已经安装了Python。如果没有安装，可以从Python官网下载并安装最新版本的Python。

2. 定义数据结构
为了存储衬衣信息，我们将使用一个列表，每个元素是一个包含衬衣详情的字典。

python
shirts = []
3. 添加衬衣（Create）
我们将定义一个函数来添加新的衬衣到库存中。每个衬衣包含id、brand、size和quantity等信息。

python
def add_shirt(shirt_id, brand, size, quantity):
    shirt = {
        'id': shirt_id,
        'brand': brand,
        'size': size,
        'quantity': quantity
    }
    shirts.append(shirt)
    print(f"Shirt {shirt_id} added successfully.")
