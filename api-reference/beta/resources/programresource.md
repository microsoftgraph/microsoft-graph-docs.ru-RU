---
title: тип ресурса programResource
description: Представляет ссылку на объект, который является объектом обзора доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0ef610650887b1d34569465bd5babb7ec91c194d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761830"
---
# <a name="programresource-resource-type"></a><span data-ttu-id="84a9a-103">тип ресурса programResource</span><span class="sxs-lookup"><span data-stu-id="84a9a-103">programResource resource type</span></span>

<span data-ttu-id="84a9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84a9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84a9a-105">Объект **programResource,** содержащийся в [объекте programControl,](programcontrol.md) представляет ссылку на объект, который является объектом, объектом обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="84a9a-105">The **programResource** object, contained within a [programControl](programcontrol.md) object, represents a reference to an object that is the target of the access review.</span></span>

<span data-ttu-id="84a9a-106">Этот тип наследует от [удостоверения](identity.md).</span><span class="sxs-lookup"><span data-stu-id="84a9a-106">This type inherits from [identity](identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="84a9a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="84a9a-107">Properties</span></span>

| <span data-ttu-id="84a9a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="84a9a-108">Property</span></span> | <span data-ttu-id="84a9a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="84a9a-109">Type</span></span> | <span data-ttu-id="84a9a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="84a9a-110">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="84a9a-111">type</span><span class="sxs-lookup"><span data-stu-id="84a9a-111">type</span></span> | <span data-ttu-id="84a9a-112">String</span><span class="sxs-lookup"><span data-stu-id="84a9a-112">String</span></span> | <span data-ttu-id="84a9a-113">Тип ресурса, указывающий, является ли он группой или приложением.</span><span class="sxs-lookup"><span data-stu-id="84a9a-113">Type of the resource, indicating whether it is a group or an app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="84a9a-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84a9a-114">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.programResource"
}-->
```json
{
  "type": "string"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "programResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
