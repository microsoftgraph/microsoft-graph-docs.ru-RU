---
title: тип ресурса конфигурации
description: Указывает дополнительные ID-адреса приложений, которые разрешены для управления внешним подключением и индексации контента в externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8a82c5e9e4cbd915d5a7e11b9e162bc510628ecf
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366781"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="6f1cf-103">тип ресурса конфигурации</span><span class="sxs-lookup"><span data-stu-id="6f1cf-103">configuration resource type</span></span>

<span data-ttu-id="6f1cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f1cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f1cf-105">Указывает дополнительные ID-адреса приложений, которые разрешены для управления внешним подключением и индексации контента [в externalConnection.](../resources/externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="6f1cf-105">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6f1cf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f1cf-106">Properties</span></span>

| <span data-ttu-id="6f1cf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f1cf-107">Property</span></span>       | <span data-ttu-id="6f1cf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6f1cf-108">Type</span></span>              | <span data-ttu-id="6f1cf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6f1cf-109">Description</span></span> |
|:---------------|:------------------|:------------|
| <span data-ttu-id="6f1cf-110">authorizedApps</span><span class="sxs-lookup"><span data-stu-id="6f1cf-110">authorizedApps</span></span> | <span data-ttu-id="6f1cf-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6f1cf-111">String collection</span></span> | <span data-ttu-id="6f1cf-112">Коллекция ID-приложений для зарегистрированных Azure Active Directory приложений, которые разрешены для управления внешним подключением и индексации контента в externalConnection.</span><span class="sxs-lookup"><span data-stu-id="6f1cf-112">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6f1cf-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f1cf-113">JSON representation</span></span>

<span data-ttu-id="6f1cf-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f1cf-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.configuration",
  "baseType": null
}-->

```json
{
  "authorizedApps": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "configuration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


