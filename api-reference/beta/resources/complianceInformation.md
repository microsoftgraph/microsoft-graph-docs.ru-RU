---
title: " Тип ресурса Комплианцеинформатион"
description: Этот ресурс содержит данные соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b93e01bf6274591282fd5e486bebb878672d8cc3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973232"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="ce70d-103">Тип ресурса Комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="ce70d-103">complianceInformation resource type</span></span>

<span data-ttu-id="ce70d-104">Содержит данные соответствия требованиям, связанные с контролем безопасного рейтинга.</span><span class="sxs-lookup"><span data-stu-id="ce70d-104">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="ce70d-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce70d-105">Property</span></span> |<span data-ttu-id="ce70d-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ce70d-106">Type</span></span> |<span data-ttu-id="ce70d-107">Описание</span><span class="sxs-lookup"><span data-stu-id="ce70d-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="ce70d-108">Цертификатионнаме</span><span class="sxs-lookup"><span data-stu-id="ce70d-108">certificationName</span></span> | <span data-ttu-id="ce70d-109">string</span><span class="sxs-lookup"><span data-stu-id="ce70d-109">string</span></span> | <span data-ttu-id="ce70d-110">Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171).</span><span class="sxs-lookup"><span data-stu-id="ce70d-110">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="ce70d-111">Цертификатионконтролс</span><span class="sxs-lookup"><span data-stu-id="ce70d-111">certificationControls</span></span> | <span data-ttu-id="ce70d-112">Коллекция [цертификатионконтрол](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="ce70d-112">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="ce70d-113">Коллекция элементов управления сертификацией, связанных с сертификацией</span><span class="sxs-lookup"><span data-stu-id="ce70d-113">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ce70d-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce70d-114">JSON representation</span></span>

<span data-ttu-id="ce70d-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce70d-115">The following is a JSON representation of the resource.</span></span>

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
