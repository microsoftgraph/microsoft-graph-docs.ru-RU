---
title: Тип ресурса Комплианцеинформатион
description: Этот ресурс содержит данные соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 85fef478a8dcc0f3196355d89f0a20ef0cd7a5b4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629308"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="f972b-103">Тип ресурса Комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="f972b-103">complianceInformation resource type</span></span>

<span data-ttu-id="f972b-104">Содержит данные соответствия требованиям, связанные с контролем безопасного рейтинга.</span><span class="sxs-lookup"><span data-stu-id="f972b-104">Contains compliance data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="f972b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f972b-105">Properties</span></span>

|<span data-ttu-id="f972b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f972b-106">Property</span></span> |<span data-ttu-id="f972b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f972b-107">Type</span></span> |<span data-ttu-id="f972b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f972b-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="f972b-109">Цертификатионнаме</span><span class="sxs-lookup"><span data-stu-id="f972b-109">certificationName</span></span>|<span data-ttu-id="f972b-110">String</span><span class="sxs-lookup"><span data-stu-id="f972b-110">String</span></span>| <span data-ttu-id="f972b-111">Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171).</span><span class="sxs-lookup"><span data-stu-id="f972b-111">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="f972b-112">Цертификатионконтролс</span><span class="sxs-lookup"><span data-stu-id="f972b-112">certificationControls</span></span>|<span data-ttu-id="f972b-113">Коллекция [цертификатионконтрол](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="f972b-113">[certificationControl](certificationcontrol.md) collection</span></span>|<span data-ttu-id="f972b-114">Коллекция элементов управления сертификацией, связанных с сертификацией</span><span class="sxs-lookup"><span data-stu-id="f972b-114">Collection of the certification controls associated with certification</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f972b-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f972b-115">JSON representation</span></span>

<span data-ttu-id="f972b-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f972b-116">The following is a JSON representation of the resource.</span></span>

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
