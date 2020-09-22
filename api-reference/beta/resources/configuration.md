---
title: Тип ресурса конфигурации
description: Задает дополнительные идентификаторы приложений, которым разрешено управлять Екстерналконнектион и индексировать содержимое в Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bd267c77a9904564e8b2b7f592f207204d9396b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994220"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="7126f-103">Тип ресурса конфигурации</span><span class="sxs-lookup"><span data-stu-id="7126f-103">configuration resource type</span></span>

<span data-ttu-id="7126f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7126f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7126f-105">Задает дополнительные идентификаторы приложений, которым разрешено управлять Екстерналконнектион и индексировать содержимое в [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="7126f-105">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="7126f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7126f-106">Properties</span></span>

| <span data-ttu-id="7126f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7126f-107">Property</span></span>       | <span data-ttu-id="7126f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7126f-108">Type</span></span>              | <span data-ttu-id="7126f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7126f-109">Description</span></span> |
|:---------------|:------------------|:------------|
| <span data-ttu-id="7126f-110">аусоризедаппс</span><span class="sxs-lookup"><span data-stu-id="7126f-110">authorizedApps</span></span> | <span data-ttu-id="7126f-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7126f-111">String collection</span></span> | <span data-ttu-id="7126f-112">Коллекция идентификаторов приложений для зарегистрированных приложений Azure Active Directory, которым разрешено управлять Екстерналконнектион и индексировать контент в Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="7126f-112">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7126f-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7126f-113">JSON representation</span></span>

<span data-ttu-id="7126f-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7126f-114">The following is a JSON representation of the resource.</span></span>

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


