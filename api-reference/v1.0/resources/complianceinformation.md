---
title: Тип ресурса Комплианцеинформатион
description: Этот ресурс содержит данные соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9fc47940b8a9f249e66092ee016453a9eb5152ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032860"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="0d3e2-103">Тип ресурса Комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="0d3e2-103">complianceInformation resource type</span></span>

<span data-ttu-id="0d3e2-104">Содержит данные соответствия требованиям, связанные с контролем безопасного рейтинга.</span><span class="sxs-lookup"><span data-stu-id="0d3e2-104">Contains compliance data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="0d3e2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d3e2-105">Properties</span></span>

|<span data-ttu-id="0d3e2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d3e2-106">Property</span></span> |<span data-ttu-id="0d3e2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0d3e2-107">Type</span></span> |<span data-ttu-id="0d3e2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0d3e2-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="0d3e2-109">Цертификатионнаме</span><span class="sxs-lookup"><span data-stu-id="0d3e2-109">certificationName</span></span>|<span data-ttu-id="0d3e2-110">String</span><span class="sxs-lookup"><span data-stu-id="0d3e2-110">String</span></span>| <span data-ttu-id="0d3e2-111">Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171).</span><span class="sxs-lookup"><span data-stu-id="0d3e2-111">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="0d3e2-112">Цертификатионконтролс</span><span class="sxs-lookup"><span data-stu-id="0d3e2-112">certificationControls</span></span>|<span data-ttu-id="0d3e2-113">Коллекция [цертификатионконтрол](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="0d3e2-113">[certificationControl](certificationcontrol.md) collection</span></span>|<span data-ttu-id="0d3e2-114">Коллекция элементов управления сертификацией, связанных с сертификацией</span><span class="sxs-lookup"><span data-stu-id="0d3e2-114">Collection of the certification controls associated with certification</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d3e2-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d3e2-115">JSON representation</span></span>

<span data-ttu-id="0d3e2-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d3e2-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.complianceInformation"
}-->

```json
{
  "certificationName": "String",
  "certificationControls": [{"@odata.type": "microsoft.graph.certificationControl"}]
}

```


<!-- {
  "type": "#page.annotation",
  "description": "complianceInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
