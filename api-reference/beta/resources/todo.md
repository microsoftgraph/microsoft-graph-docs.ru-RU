---
title: Тип ресурса todo
description: Представляет службы дел, доступные пользователю.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 99b2936cf84c5cfdc25a39ff6f0e35518658d0ff
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46850048"
---
# <a name="todo-resource-type"></a><span data-ttu-id="5bd05-103">Тип ресурса todo</span><span class="sxs-lookup"><span data-stu-id="5bd05-103">todo resource type</span></span>

<span data-ttu-id="5bd05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bd05-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5bd05-105">Представляет службы дел, доступные пользователю.</span><span class="sxs-lookup"><span data-stu-id="5bd05-105">Represents the To Do services available to a user.</span></span>

<span data-ttu-id="5bd05-106">Наследуется от [объекта.](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="5bd05-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5bd05-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5bd05-107">Methods</span></span>
|<span data-ttu-id="5bd05-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5bd05-108">Method</span></span>|<span data-ttu-id="5bd05-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="5bd05-109">Return type</span></span>|<span data-ttu-id="5bd05-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5bd05-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5bd05-111">Списки</span><span class="sxs-lookup"><span data-stu-id="5bd05-111">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="5bd05-112">[Коллекция todoTaskList](todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="5bd05-112">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="5bd05-113">Получение всех списков задач в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bd05-113">Get all the task lists in the user's mailbox.</span></span> |
|[<span data-ttu-id="5bd05-114">Создание объекта todoTaskList</span><span class="sxs-lookup"><span data-stu-id="5bd05-114">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="5bd05-115">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="5bd05-115">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="5bd05-116">Создание списка задач в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bd05-116">Create a To Do task list in the user's mailbox.</span></span> |

## <a name="properties"></a><span data-ttu-id="5bd05-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="5bd05-117">Properties</span></span>
<span data-ttu-id="5bd05-118">Нет</span><span class="sxs-lookup"><span data-stu-id="5bd05-118">None</span></span>

## <a name="relationships"></a><span data-ttu-id="5bd05-119">Связи</span><span class="sxs-lookup"><span data-stu-id="5bd05-119">Relationships</span></span>
|<span data-ttu-id="5bd05-120">Связь</span><span class="sxs-lookup"><span data-stu-id="5bd05-120">Relationship</span></span>|<span data-ttu-id="5bd05-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5bd05-121">Type</span></span>|<span data-ttu-id="5bd05-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5bd05-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bd05-123">lists</span><span class="sxs-lookup"><span data-stu-id="5bd05-123">lists</span></span>|<span data-ttu-id="5bd05-124">[Коллекция todoTaskList](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="5bd05-124">[todoTaskList](../resources/todotasklist.md) collection</span></span>| <span data-ttu-id="5bd05-125">Списки задач в почтовом ящике пользователей.</span><span class="sxs-lookup"><span data-stu-id="5bd05-125">The task lists in the users mailbox.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5bd05-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5bd05-126">JSON representation</span></span>
<span data-ttu-id="5bd05-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5bd05-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todo",
  "id": "String"
}
```

