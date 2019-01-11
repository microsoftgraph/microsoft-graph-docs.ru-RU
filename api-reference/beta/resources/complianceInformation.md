---
title: " Тип ресурса complianceInformation"
description: Этот ресурс содержит соответствия данные, связанные с безопасного элемента управления показателя.
localization_priority: Normal
ms.openlocfilehash: 7a3968e6e043d2019100870061c5e34b03b1b8bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820603"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="7f89e-103">Тип ресурса complianceInformation</span><span class="sxs-lookup"><span data-stu-id="7f89e-103">complianceInformation resource type</span></span>

<span data-ttu-id="7f89e-104">Соответствие требованиям содержит данные, связанные с безопасного элемента управления показателя.</span><span class="sxs-lookup"><span data-stu-id="7f89e-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="7f89e-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f89e-105">Property</span></span> |<span data-ttu-id="7f89e-106">Тип</span><span class="sxs-lookup"><span data-stu-id="7f89e-106">Type</span></span> |<span data-ttu-id="7f89e-107">Описание</span><span class="sxs-lookup"><span data-stu-id="7f89e-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="7f89e-108">certificationName</span><span class="sxs-lookup"><span data-stu-id="7f89e-108">certificationName</span></span> | <span data-ttu-id="7f89e-109">string</span><span class="sxs-lookup"><span data-stu-id="7f89e-109">string</span></span> | <span data-ttu-id="7f89e-110">Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800 171)</span><span class="sxs-lookup"><span data-stu-id="7f89e-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="7f89e-111">certificationControls</span><span class="sxs-lookup"><span data-stu-id="7f89e-111">certificationControls</span></span> | <span data-ttu-id="7f89e-112">[certificationControl](certificationcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7f89e-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="7f89e-113">Коллекция элементов управления сертификации, связанные с сертификации</span><span class="sxs-lookup"><span data-stu-id="7f89e-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7f89e-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f89e-114">JSON representation</span></span>

<span data-ttu-id="7f89e-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f89e-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.complianceInformation"
}-->

```json
{
  "certificationName": "String",
  "certificationControls": "Collection(microsoft.graph.complianceInformation)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
