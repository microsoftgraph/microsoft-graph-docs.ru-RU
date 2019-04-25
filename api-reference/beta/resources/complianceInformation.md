---
title: " Тип ресурса Комплианцеинформатион"
description: Этот ресурс содержит данные соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
ms.openlocfilehash: 7a3968e6e043d2019100870061c5e34b03b1b8bd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543366"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="d0fec-103">Тип ресурса Комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="d0fec-103">complianceInformation resource type</span></span>

<span data-ttu-id="d0fec-104">Содержит данные соответствия требованиям, связанные с контролем безопасного рейтинга.</span><span class="sxs-lookup"><span data-stu-id="d0fec-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="d0fec-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0fec-105">Property</span></span> |<span data-ttu-id="d0fec-106">Тип</span><span class="sxs-lookup"><span data-stu-id="d0fec-106">Type</span></span> |<span data-ttu-id="d0fec-107">Описание</span><span class="sxs-lookup"><span data-stu-id="d0fec-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="d0fec-108">Цертификатионнаме</span><span class="sxs-lookup"><span data-stu-id="d0fec-108">certificationName</span></span> | <span data-ttu-id="d0fec-109">string</span><span class="sxs-lookup"><span data-stu-id="d0fec-109">string</span></span> | <span data-ttu-id="d0fec-110">Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171).</span><span class="sxs-lookup"><span data-stu-id="d0fec-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="d0fec-111">Цертификатионконтролс</span><span class="sxs-lookup"><span data-stu-id="d0fec-111">certificationControls</span></span> | <span data-ttu-id="d0fec-112">Коллекция [цертификатионконтрол](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="d0fec-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="d0fec-113">Коллекция элементов управления сертификацией, связанных с сертификацией</span><span class="sxs-lookup"><span data-stu-id="d0fec-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d0fec-114">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d0fec-114">JSON representation</span></span>

<span data-ttu-id="d0fec-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0fec-115">The following is a JSON representation of the resource.</span></span>

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
