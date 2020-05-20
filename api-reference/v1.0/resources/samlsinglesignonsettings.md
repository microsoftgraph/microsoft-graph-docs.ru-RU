---
title: Тип ресурса Самлсинглесигнонсеттингс
description: Представляет параметры единого входа SAML.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 1f6af4e7a1eb88a42f8ac72cefc55609b76bf4c4
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290555"
---
# <a name="samlsinglesignonsettings-resource-type"></a><span data-ttu-id="3aca4-103">Тип ресурса Самлсинглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="3aca4-103">samlSingleSignOnSettings resource type</span></span>

<span data-ttu-id="3aca4-104">Представляет контейнер для параметров, связанных с единым входом SAML.</span><span class="sxs-lookup"><span data-stu-id="3aca4-104">Represents a container for settings related to SAML single sign-on.</span></span>

## <a name="properties"></a><span data-ttu-id="3aca4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3aca4-105">Properties</span></span>

| <span data-ttu-id="3aca4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3aca4-106">Property</span></span> | <span data-ttu-id="3aca4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3aca4-107">Type</span></span> | <span data-ttu-id="3aca4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3aca4-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3aca4-109">релайстате</span><span class="sxs-lookup"><span data-stu-id="3aca4-109">relayState</span></span>|<span data-ttu-id="3aca4-110">String</span><span class="sxs-lookup"><span data-stu-id="3aca4-110">String</span></span>| <span data-ttu-id="3aca4-111">Относительный URI, по которому поставщик услуг перенаправляется после завершения процесса единого входа.</span><span class="sxs-lookup"><span data-stu-id="3aca4-111">The relative URI the service provider would redirect to after completion of the single sign-on flow.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="3aca4-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3aca4-112">JSON representation</span></span>
<span data-ttu-id="3aca4-113">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3aca4-113">Here is a JSON representation of the resource.</span></span>

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