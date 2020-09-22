---
title: Тип ресурса Комплианцеинформатион
description: Этот ресурс содержит данные соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 00447f134b2c54bdda92857c6c84c05e8c52b3cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018937"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="641d1-103">Тип ресурса Комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="641d1-103">complianceInformation resource type</span></span>

<span data-ttu-id="641d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="641d1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="641d1-105">Содержит данные соответствия требованиям, связанные с контролем безопасного рейтинга.</span><span class="sxs-lookup"><span data-stu-id="641d1-105">Contains compliance data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="641d1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="641d1-106">Properties</span></span>

|<span data-ttu-id="641d1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="641d1-107">Property</span></span> |<span data-ttu-id="641d1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="641d1-108">Type</span></span> |<span data-ttu-id="641d1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="641d1-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="641d1-110">цертификатионнаме</span><span class="sxs-lookup"><span data-stu-id="641d1-110">certificationName</span></span>|<span data-ttu-id="641d1-111">String</span><span class="sxs-lookup"><span data-stu-id="641d1-111">String</span></span>| <span data-ttu-id="641d1-112">Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171).</span><span class="sxs-lookup"><span data-stu-id="641d1-112">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="641d1-113">цертификатионконтролс</span><span class="sxs-lookup"><span data-stu-id="641d1-113">certificationControls</span></span>|<span data-ttu-id="641d1-114">Коллекция [цертификатионконтрол](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="641d1-114">[certificationControl](certificationcontrol.md) collection</span></span>|<span data-ttu-id="641d1-115">Коллекция элементов управления сертификацией, связанных с сертификацией</span><span class="sxs-lookup"><span data-stu-id="641d1-115">Collection of the certification controls associated with certification</span></span>|

## <a name="json-representation"></a><span data-ttu-id="641d1-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="641d1-116">JSON representation</span></span>

<span data-ttu-id="641d1-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="641d1-117">The following is a JSON representation of the resource.</span></span>

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

