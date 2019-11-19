---
title: Тип ресурса конфигурации
description: Задает дополнительные идентификаторы приложений, которым разрешено управлять Екстерналконнектион и индексировать содержимое в Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c7808d014ee2ab19fda9eceb6064375cf5904d52
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704152"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="4336e-103">Тип ресурса конфигурации</span><span class="sxs-lookup"><span data-stu-id="4336e-103">configuration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4336e-104">Задает дополнительные идентификаторы приложений, которым разрешено управлять Екстерналконнектион и индексировать содержимое в [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="4336e-104">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="4336e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4336e-105">Properties</span></span>

| <span data-ttu-id="4336e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4336e-106">Property</span></span>       | <span data-ttu-id="4336e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4336e-107">Type</span></span>              | <span data-ttu-id="4336e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4336e-108">Description</span></span> |
|:---------------|:------------------|:------------|
| <span data-ttu-id="4336e-109">аусоризедаппс</span><span class="sxs-lookup"><span data-stu-id="4336e-109">authorizedApps</span></span> | <span data-ttu-id="4336e-110">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4336e-110">String collection</span></span> | <span data-ttu-id="4336e-111">Коллекция идентификаторов приложений для зарегистрированных приложений Azure Active Directory, которым разрешено управлять Екстерналконнектион и индексировать контент в Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="4336e-111">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4336e-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4336e-112">JSON representation</span></span>

<span data-ttu-id="4336e-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4336e-113">The following is a JSON representation of the resource.</span></span>

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
