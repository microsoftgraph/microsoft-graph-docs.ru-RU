---
title: сложный тип requestorManager
description: Определяет отношение к другому пользователю в клиенте, которому будет разрешено в качестве утвержденного.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b4bfd42854a55ec2daa9e380c539a25479b0e933
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761081"
---
# <a name="requestormanager-complex-type"></a><span data-ttu-id="04cbc-103">сложный тип requestorManager</span><span class="sxs-lookup"><span data-stu-id="04cbc-103">requestorManager complex type</span></span>

<span data-ttu-id="04cbc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04cbc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04cbc-105">Используется в параметрах утверждения политики назначения [пакета доступа.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="04cbc-105">Used in the approval settings of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="04cbc-106">Это подтип [userSet,](userset.md)в котором значение указывает, что администратор запрашиваемого пользователя должен `@odata.type` `#microsoft.graph.requestorManager` быть одобрением.</span><span class="sxs-lookup"><span data-stu-id="04cbc-106">It is a subtype of [userSet](userset.md), in which the `@odata.type` value `#microsoft.graph.requestorManager` indicates that a requesting user's manager is to be the approver.</span></span>  <span data-ttu-id="04cbc-107">При создании этапа утверждения политики назначения пакетов доступа с помощью requestorManager также включаем другого участника, например одного пользователя или члена группы, в случае, если у запрашиваемого пользователя нет менеджера.</span><span class="sxs-lookup"><span data-stu-id="04cbc-107">When creating an access package assignment policy approval stage with requestorManager, also include another approver, such as a single user or group member, in case the requesting user does not have a manager.</span></span>


## <a name="properties"></a><span data-ttu-id="04cbc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="04cbc-108">Properties</span></span>


| <span data-ttu-id="04cbc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="04cbc-109">Property</span></span>                     | <span data-ttu-id="04cbc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="04cbc-110">Type</span></span>                      | <span data-ttu-id="04cbc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="04cbc-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="04cbc-112">isBackup</span><span class="sxs-lookup"><span data-stu-id="04cbc-112">isBackup</span></span> | <span data-ttu-id="04cbc-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="04cbc-113">Boolean</span></span> | <span data-ttu-id="04cbc-114">Для диспетчера на стадии утверждения указывает, является ли он резервным утверждением резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="04cbc-114">For a manager in an approval stage, indicates whether the manager is a backup fallback approver.</span></span> |
|<span data-ttu-id="04cbc-115">managerLevel</span><span class="sxs-lookup"><span data-stu-id="04cbc-115">managerLevel</span></span> | <span data-ttu-id="04cbc-116">Int32</span><span class="sxs-lookup"><span data-stu-id="04cbc-116">Int32</span></span> | <span data-ttu-id="04cbc-117">Иерархический уровень руководителя в отношении запросителя.</span><span class="sxs-lookup"><span data-stu-id="04cbc-117">The hierarchical level of the manager with respect to the requestor.</span></span> <span data-ttu-id="04cbc-118">Например, у непосредственного менеджера запросителя будет managerLevel 1, а у менеджера менеджера запросителя будет managerLevel 2.</span><span class="sxs-lookup"><span data-stu-id="04cbc-118">For example, the direct manager of a requestor would have a managerLevel of 1, while the manager of the requestor's manager would have a managerLevel of 2.</span></span> <span data-ttu-id="04cbc-119">Значение по умолчанию для managerLevel — 1.</span><span class="sxs-lookup"><span data-stu-id="04cbc-119">Default value for managerLevel is 1.</span></span> <span data-ttu-id="04cbc-120">Возможные значения для этого свойства варьируются от 1 до 2.</span><span class="sxs-lookup"><span data-stu-id="04cbc-120">Possible values for this property range from 1 to 2.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="04cbc-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04cbc-121">JSON representation</span></span>

<span data-ttu-id="04cbc-122">Ниже приводится представление JSON этого типа.</span><span class="sxs-lookup"><span data-stu-id="04cbc-122">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorManager",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "isBackup": false,
  "managerLevel": 1
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestorManager complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


