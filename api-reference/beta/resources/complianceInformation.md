---
title: " Тип ресурса Комплианцеинформатион"
description: Этот ресурс содержит данные соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 69114795468a3cb23908a0ca476de5a34032aa86
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033918"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="e961a-103">Тип ресурса Комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="e961a-103">complianceInformation resource type</span></span>

<span data-ttu-id="e961a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e961a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e961a-105">Содержит данные соответствия требованиям, связанные с контролем безопасного рейтинга.</span><span class="sxs-lookup"><span data-stu-id="e961a-105">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="e961a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e961a-106">Property</span></span> |<span data-ttu-id="e961a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e961a-107">Type</span></span> |<span data-ttu-id="e961a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e961a-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="e961a-109">цертификатионнаме</span><span class="sxs-lookup"><span data-stu-id="e961a-109">certificationName</span></span> | <span data-ttu-id="e961a-110">string</span><span class="sxs-lookup"><span data-stu-id="e961a-110">string</span></span> | <span data-ttu-id="e961a-111">Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171).</span><span class="sxs-lookup"><span data-stu-id="e961a-111">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="e961a-112">цертификатионконтролс</span><span class="sxs-lookup"><span data-stu-id="e961a-112">certificationControls</span></span> | <span data-ttu-id="e961a-113">Коллекция [цертификатионконтрол](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="e961a-113">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="e961a-114">Коллекция элементов управления сертификацией, связанных с сертификацией</span><span class="sxs-lookup"><span data-stu-id="e961a-114">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e961a-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e961a-115">JSON representation</span></span>

<span data-ttu-id="e961a-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e961a-116">The following is a JSON representation of the resource.</span></span>

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


