---
title: тип ресурса конфигурации
description: Указывает дополнительные ID-адреса приложений, которые разрешены для управления внешним подключением и индексации контента в externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 05fbf022c11cf318281831d1b4e8572646875a06
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467831"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="5cdd3-103">тип ресурса конфигурации</span><span class="sxs-lookup"><span data-stu-id="5cdd3-103">configuration resource type</span></span>

<span data-ttu-id="5cdd3-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="5cdd3-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cdd3-105">Указывает дополнительные ID-адреса приложений, которые разрешены для управления внешним подключением и индексации контента [в externalConnection.](../resources/externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="5cdd3-105">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5cdd3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5cdd3-106">Properties</span></span>

| <span data-ttu-id="5cdd3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cdd3-107">Property</span></span>       | <span data-ttu-id="5cdd3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5cdd3-108">Type</span></span>              | <span data-ttu-id="5cdd3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5cdd3-109">Description</span></span> |
|:---------------|:------------------|:------------|
| <span data-ttu-id="5cdd3-110">authorizedAppIds</span><span class="sxs-lookup"><span data-stu-id="5cdd3-110">authorizedAppIds</span></span> | <span data-ttu-id="5cdd3-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5cdd3-111">String collection</span></span> | <span data-ttu-id="5cdd3-112">Коллекция ID-приложений для зарегистрированных Azure Active Directory приложений, которые разрешены для управления внешним подключением и индексации контента в externalConnection.</span><span class="sxs-lookup"><span data-stu-id="5cdd3-112">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span> |

> [!NOTE]
> <span data-ttu-id="5cdd3-113">Свойство `authorizedAppIds` было ранее названо `authorizedApps` .</span><span class="sxs-lookup"><span data-stu-id="5cdd3-113">The `authorizedAppIds` property was previously named `authorizedApps`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cdd3-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5cdd3-114">JSON representation</span></span>

<span data-ttu-id="5cdd3-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5cdd3-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.configuration",
  "baseType": null
}-->

```json
{
  "authorizedAppIds": ["String"]
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
