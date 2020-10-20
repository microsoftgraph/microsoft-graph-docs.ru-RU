---
title: Тип ресурса Програмресаурце
description: Представляет ссылку на объект, который является целевым объектом проверки доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5ad3720587523e6937b4c3713a1c5a8c06d1e6e5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601498"
---
# <a name="programresource-resource-type"></a><span data-ttu-id="a99ab-103">Тип ресурса Програмресаурце</span><span class="sxs-lookup"><span data-stu-id="a99ab-103">programResource resource type</span></span>

<span data-ttu-id="a99ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a99ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a99ab-105">Объект **програмресаурце** , содержащийся в объекте [програмконтрол](programcontrol.md) , представляет ссылку на объект, который является целевым объектом проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="a99ab-105">The **programResource** object, contained within a [programControl](programcontrol.md) object, represents a reference to an object that is the target of the access review.</span></span>

<span data-ttu-id="a99ab-106">Этот тип наследуется от [Identity](identity.md).</span><span class="sxs-lookup"><span data-stu-id="a99ab-106">This type inherits from [identity](identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a99ab-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a99ab-107">Properties</span></span>

| <span data-ttu-id="a99ab-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a99ab-108">Property</span></span> | <span data-ttu-id="a99ab-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a99ab-109">Type</span></span> | <span data-ttu-id="a99ab-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a99ab-110">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="a99ab-111">type</span><span class="sxs-lookup"><span data-stu-id="a99ab-111">type</span></span> | <span data-ttu-id="a99ab-112">String</span><span class="sxs-lookup"><span data-stu-id="a99ab-112">String</span></span> | <span data-ttu-id="a99ab-113">Тип ресурса, указывающий, является ли он группой или приложением.</span><span class="sxs-lookup"><span data-stu-id="a99ab-113">Type of the resource, indicating whether it is a group or an app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a99ab-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a99ab-114">JSON representation</span></span>

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
