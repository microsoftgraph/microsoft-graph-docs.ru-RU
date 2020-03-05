---
title: Тип ресурса конфигурации
description: Задает дополнительные идентификаторы приложений, которым разрешено управлять Екстерналконнектион и индексировать содержимое в Екстерналконнектион.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: be4fa7bd8f4b44842bd6dbc9876d0dd19fe466fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507501"
---
# <a name="configuration-resource-type"></a><span data-ttu-id="ae450-103">Тип ресурса конфигурации</span><span class="sxs-lookup"><span data-stu-id="ae450-103">configuration resource type</span></span>

<span data-ttu-id="ae450-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ae450-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae450-105">Задает дополнительные идентификаторы приложений, которым разрешено управлять Екстерналконнектион и индексировать содержимое в [екстерналконнектион](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="ae450-105">Specifies additional application IDs that are allowed to manage the externalConnection and to index content in a [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="ae450-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae450-106">Properties</span></span>

| <span data-ttu-id="ae450-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae450-107">Property</span></span>       | <span data-ttu-id="ae450-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ae450-108">Type</span></span>              | <span data-ttu-id="ae450-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ae450-109">Description</span></span> |
|:---------------|:------------------|:------------|
| <span data-ttu-id="ae450-110">аусоризедаппс</span><span class="sxs-lookup"><span data-stu-id="ae450-110">authorizedApps</span></span> | <span data-ttu-id="ae450-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ae450-111">String collection</span></span> | <span data-ttu-id="ae450-112">Коллекция идентификаторов приложений для зарегистрированных приложений Azure Active Directory, которым разрешено управлять Екстерналконнектион и индексировать контент в Екстерналконнектион.</span><span class="sxs-lookup"><span data-stu-id="ae450-112">A collection of application IDs for registered Azure Active Directory apps that are allowed to manage the externalConnection and to index content in the externalConnection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ae450-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae450-113">JSON representation</span></span>

<span data-ttu-id="ae450-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae450-114">The following is a JSON representation of the resource.</span></span>

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
