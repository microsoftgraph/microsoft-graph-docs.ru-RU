---
title: " Тип ресурса complianceInformation"
description: Этот ресурс содержит соответствия данные, связанные с безопасного элемента управления показателя.
ms.openlocfilehash: a32670c6d11d391834358b769ae938a67b3d8aad
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380961"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="c88a3-103">Тип ресурса complianceInformation</span><span class="sxs-lookup"><span data-stu-id="c88a3-103">complianceInformation resource type</span></span>

<span data-ttu-id="c88a3-104">Соответствие требованиям содержит данные, связанные с безопасного элемента управления показателя.</span><span class="sxs-lookup"><span data-stu-id="c88a3-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="c88a3-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="c88a3-105">Property</span></span> |<span data-ttu-id="c88a3-106">Тип</span><span class="sxs-lookup"><span data-stu-id="c88a3-106">Type</span></span> |<span data-ttu-id="c88a3-107">Описание</span><span class="sxs-lookup"><span data-stu-id="c88a3-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="c88a3-108">certificationName</span><span class="sxs-lookup"><span data-stu-id="c88a3-108">certificationName</span></span> | <span data-ttu-id="c88a3-109">строка</span><span class="sxs-lookup"><span data-stu-id="c88a3-109">string</span></span> | <span data-ttu-id="c88a3-110">Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800 171)</span><span class="sxs-lookup"><span data-stu-id="c88a3-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="c88a3-111">certificationControls</span><span class="sxs-lookup"><span data-stu-id="c88a3-111">certificationControls</span></span> | <span data-ttu-id="c88a3-112">[certificationControl](certificationcontrol.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c88a3-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="c88a3-113">Коллекция элементов управления сертификации, связанные с сертификации</span><span class="sxs-lookup"><span data-stu-id="c88a3-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c88a3-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c88a3-114">JSON representation</span></span>

<span data-ttu-id="c88a3-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c88a3-115">The following is a JSON representation of the resource.</span></span>

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
