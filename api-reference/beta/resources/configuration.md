---
title: Тип ресурса конфигурации
description: Задает дополнительные идентификаторы приложений, которым разрешено управлять Екстерналконнектион и индексировать содержимое в Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 080a966ae9435c189a34155d108e1c48235ffb07
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938893"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="20a72-103">Тип ресурса конфигурации</span><span class="sxs-lookup"><span data-stu-id="20a72-103">configuration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20a72-104">Задает дополнительные идентификаторы приложений, которым разрешено управлять Екстерналконнектион и индексировать содержимое в [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="20a72-104">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="20a72-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="20a72-105">Properties</span></span>

| <span data-ttu-id="20a72-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="20a72-106">Property</span></span>       | <span data-ttu-id="20a72-107">Тип</span><span class="sxs-lookup"><span data-stu-id="20a72-107">Type</span></span>              | <span data-ttu-id="20a72-108">Описание</span><span class="sxs-lookup"><span data-stu-id="20a72-108">Description</span></span> |
|:---------------|:------------------|:------------|
| <span data-ttu-id="20a72-109">аусоризедаппс</span><span class="sxs-lookup"><span data-stu-id="20a72-109">authorizedApps</span></span> | <span data-ttu-id="20a72-110">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="20a72-110">String collection</span></span> | <span data-ttu-id="20a72-111">Коллекция идентификаторов приложений для зарегистрированных приложений Azure Active Directory, которым разрешено управлять Екстерналконнектион и индексировать контент в Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="20a72-111">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="20a72-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20a72-112">JSON representation</span></span>

<span data-ttu-id="20a72-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20a72-113">The following is a JSON representation of the resource.</span></span>

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
