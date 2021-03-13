---
title: тип ресурса domainIdentitySource
description: Тип domainIdentitySource определяет домен, не связанный с клиентом, в качестве источника удостоверений для связанной организации.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ae616c98b2ca20ec4e5d9c7aceeba5bdeb538e81
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759666"
---
# <a name="domainidentitysource-resource-type"></a><span data-ttu-id="e1547-103">тип ресурса domainIdentitySource</span><span class="sxs-lookup"><span data-stu-id="e1547-103">domainIdentitySource resource type</span></span>

<span data-ttu-id="e1547-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1547-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1547-105">Используется в источниках удостоверений [подключеннойорганизации.](connectedOrganization.md)</span><span class="sxs-lookup"><span data-stu-id="e1547-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="e1547-106">Это значение указывает на то, что этот тип определяет домен как источник удостоверений `@odata.type` `#microsoft.graph.domainIdentitySource` для связанной организации.</span><span class="sxs-lookup"><span data-stu-id="e1547-106">The `@odata.type` value `#microsoft.graph.domainIdentitySource` indicates that this type identifies a domain as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="e1547-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1547-107">Properties</span></span>

| <span data-ttu-id="e1547-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1547-108">Property</span></span>                     | <span data-ttu-id="e1547-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e1547-109">Type</span></span>                      | <span data-ttu-id="e1547-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e1547-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="e1547-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e1547-111">displayName</span></span> |<span data-ttu-id="e1547-112">String</span><span class="sxs-lookup"><span data-stu-id="e1547-112">String</span></span> | <span data-ttu-id="e1547-113">Имя источника удостоверений, как правило, также доменное имя.</span><span class="sxs-lookup"><span data-stu-id="e1547-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="e1547-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1547-114">Read only.</span></span> |
| <span data-ttu-id="e1547-115">domainName</span><span class="sxs-lookup"><span data-stu-id="e1547-115">domainName</span></span> |<span data-ttu-id="e1547-116">String</span><span class="sxs-lookup"><span data-stu-id="e1547-116">String</span></span> | <span data-ttu-id="e1547-117">Доменное имя.</span><span class="sxs-lookup"><span data-stu-id="e1547-117">The domain name.</span></span> <span data-ttu-id="e1547-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1547-118">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e1547-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="e1547-119">Relationships</span></span>

<span data-ttu-id="e1547-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e1547-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1547-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e1547-121">JSON representation</span></span>

<span data-ttu-id="e1547-122">Ниже приводится представление JSON этого типа.</span><span class="sxs-lookup"><span data-stu-id="e1547-122">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainIdentitySource",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainIdentitySource resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


