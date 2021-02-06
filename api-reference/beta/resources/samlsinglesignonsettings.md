---
title: Тип ресурса samlSingleSignOnSettings
description: Представляет параметры единого входов SAML.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 0b82f334196bcd9f7799a3a7a3ef7b5374571ac4
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136143"
---
# <a name="samlsinglesignonsettings-resource-type"></a><span data-ttu-id="742a1-103">Тип ресурса samlSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="742a1-103">samlSingleSignOnSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="742a1-104">Представляет контейнер для параметров, связанных с единым входом SAML.</span><span class="sxs-lookup"><span data-stu-id="742a1-104">Represents a container for settings related to SAML single sign-on.</span></span>

## <a name="properties"></a><span data-ttu-id="742a1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="742a1-105">Properties</span></span>

| <span data-ttu-id="742a1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="742a1-106">Property</span></span> | <span data-ttu-id="742a1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="742a1-107">Type</span></span> | <span data-ttu-id="742a1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="742a1-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="742a1-109">relayState</span><span class="sxs-lookup"><span data-stu-id="742a1-109">relayState</span></span>|<span data-ttu-id="742a1-110">Строка</span><span class="sxs-lookup"><span data-stu-id="742a1-110">String</span></span>| <span data-ttu-id="742a1-111">Относительный URI, на который поставщик службы перенаправляется после завершения потока единого входов.</span><span class="sxs-lookup"><span data-stu-id="742a1-111">The relative URI the service provider would redirect to after completion of the single sign-on flow.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="742a1-112">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="742a1-112">JSON representation</span></span>
<span data-ttu-id="742a1-113">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="742a1-113">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.samlSingleSignOnSettings"
}-->

```json
{
    "relayState": "string",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "samlSingleSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


