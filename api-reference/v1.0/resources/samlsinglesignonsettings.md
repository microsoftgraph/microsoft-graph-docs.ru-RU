---
title: тип ресурса samlSingleSignOnSettings
description: Представляет параметры единого входного знака SAML.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: c923c4c5b7294abb78e7fe93f852f14304601de6
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761088"
---
# <a name="samlsinglesignonsettings-resource-type"></a><span data-ttu-id="36d39-103">тип ресурса samlSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="36d39-103">samlSingleSignOnSettings resource type</span></span>

<span data-ttu-id="36d39-104">Представляет контейнер для параметров, связанных с одним входом SAML.</span><span class="sxs-lookup"><span data-stu-id="36d39-104">Represents a container for settings related to SAML single sign-on.</span></span>

## <a name="properties"></a><span data-ttu-id="36d39-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="36d39-105">Properties</span></span>

| <span data-ttu-id="36d39-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="36d39-106">Property</span></span> | <span data-ttu-id="36d39-107">Тип</span><span class="sxs-lookup"><span data-stu-id="36d39-107">Type</span></span> | <span data-ttu-id="36d39-108">Описание</span><span class="sxs-lookup"><span data-stu-id="36d39-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="36d39-109">relayState</span><span class="sxs-lookup"><span data-stu-id="36d39-109">relayState</span></span>|<span data-ttu-id="36d39-110">String</span><span class="sxs-lookup"><span data-stu-id="36d39-110">String</span></span>| <span data-ttu-id="36d39-111">Относительный URI, на который поставщик услуг перенаправляет после завершения единого потока входов.</span><span class="sxs-lookup"><span data-stu-id="36d39-111">The relative URI the service provider would redirect to after completion of the single sign-on flow.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="36d39-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36d39-112">JSON representation</span></span>
<span data-ttu-id="36d39-113">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36d39-113">Here is a JSON representation of the resource.</span></span>

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
