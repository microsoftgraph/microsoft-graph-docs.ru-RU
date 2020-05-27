---
title: Тип ресурса Самлсинглесигнонсеттингс
description: Представляет параметры единого входа SAML.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 60d7f28de54cd772ac440e6f72f61cd2bb08fe00
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383870"
---
# <a name="samlsinglesignonsettings-resource-type"></a><span data-ttu-id="b8940-103">Тип ресурса Самлсинглесигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="b8940-103">samlSingleSignOnSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8940-104">Представляет контейнер для параметров, связанных с единым входом SAML.</span><span class="sxs-lookup"><span data-stu-id="b8940-104">Represents a container for settings related to SAML single sign-on.</span></span>

## <a name="properties"></a><span data-ttu-id="b8940-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8940-105">Properties</span></span>

| <span data-ttu-id="b8940-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8940-106">Property</span></span> | <span data-ttu-id="b8940-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b8940-107">Type</span></span> | <span data-ttu-id="b8940-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b8940-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b8940-109">релайстате</span><span class="sxs-lookup"><span data-stu-id="b8940-109">relayState</span></span>|<span data-ttu-id="b8940-110">String</span><span class="sxs-lookup"><span data-stu-id="b8940-110">String</span></span>| <span data-ttu-id="b8940-111">Относительный URI, по которому поставщик услуг перенаправляется после завершения процесса единого входа.</span><span class="sxs-lookup"><span data-stu-id="b8940-111">The relative URI the service provider would redirect to after completion of the single sign-on flow.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="b8940-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8940-112">JSON representation</span></span>
<span data-ttu-id="b8940-113">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8940-113">Here is a JSON representation of the resource.</span></span>

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
