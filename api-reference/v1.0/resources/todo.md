---
title: Тип ресурса TODO
description: Представляет службы To Do, доступные пользователю.
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: aa468c6d6556ad70d3650e40fb3fd01c46ccdb35
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48797467"
---
# <a name="todo-resource-type"></a><span data-ttu-id="6b312-103">Тип ресурса TODO</span><span class="sxs-lookup"><span data-stu-id="6b312-103">todo resource type</span></span>

<span data-ttu-id="6b312-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b312-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b312-105">Представляет службы To Do, доступные пользователю.</span><span class="sxs-lookup"><span data-stu-id="6b312-105">Represents the To Do services available to a user.</span></span>

<span data-ttu-id="6b312-106">Наследуется от [объекта Entity](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="6b312-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6b312-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6b312-107">Methods</span></span>
|<span data-ttu-id="6b312-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6b312-108">Method</span></span>|<span data-ttu-id="6b312-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="6b312-109">Return type</span></span>|<span data-ttu-id="6b312-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6b312-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6b312-111">Перечисление списков</span><span class="sxs-lookup"><span data-stu-id="6b312-111">List lists</span></span>](../api/todo-list-lists.md) | <span data-ttu-id="6b312-112">Коллекция [todoTaskList](todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="6b312-112">[todoTaskList](todotasklist.md) collection</span></span> | <span data-ttu-id="6b312-113">Получение всех списков задач в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="6b312-113">Get all the task lists in the user's mailbox.</span></span> |
|[<span data-ttu-id="6b312-114">Создание Тодотасклист</span><span class="sxs-lookup"><span data-stu-id="6b312-114">Create todoTaskList</span></span>](../api/todo-post-lists.md) | [<span data-ttu-id="6b312-115">todoTaskList</span><span class="sxs-lookup"><span data-stu-id="6b312-115">todoTaskList</span></span>](todotasklist.md) | <span data-ttu-id="6b312-116">Создание списка задач To Do в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="6b312-116">Create a To Do task list in the user's mailbox.</span></span> |

## <a name="properties"></a><span data-ttu-id="6b312-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b312-117">Properties</span></span>
<span data-ttu-id="6b312-118">Нет</span><span class="sxs-lookup"><span data-stu-id="6b312-118">None</span></span>

## <a name="relationships"></a><span data-ttu-id="6b312-119">Связи</span><span class="sxs-lookup"><span data-stu-id="6b312-119">Relationships</span></span>
|<span data-ttu-id="6b312-120">Связь</span><span class="sxs-lookup"><span data-stu-id="6b312-120">Relationship</span></span>|<span data-ttu-id="6b312-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6b312-121">Type</span></span>|<span data-ttu-id="6b312-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6b312-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b312-123">lists</span><span class="sxs-lookup"><span data-stu-id="6b312-123">lists</span></span>|<span data-ttu-id="6b312-124">Коллекция [todoTaskList](../resources/todotasklist.md)</span><span class="sxs-lookup"><span data-stu-id="6b312-124">[todoTaskList](../resources/todotasklist.md) collection</span></span>| <span data-ttu-id="6b312-125">Списки задач в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="6b312-125">The task lists in the users mailbox.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6b312-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b312-126">JSON representation</span></span>
<span data-ttu-id="6b312-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b312-127">The following is a JSON representation of the resource.</span></span>
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



