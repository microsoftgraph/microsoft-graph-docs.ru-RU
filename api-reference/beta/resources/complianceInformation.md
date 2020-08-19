---
title: " Тип ресурса Комплианцеинформатион"
description: Этот ресурс содержит данные соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 2c8bb3b2a016ec58da1ad58b01843a2691ad13b7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811142"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="abd05-103">Тип ресурса Комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="abd05-103">complianceInformation resource type</span></span>

<span data-ttu-id="abd05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abd05-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="abd05-105">Содержит данные соответствия требованиям, связанные с контролем безопасного рейтинга.</span><span class="sxs-lookup"><span data-stu-id="abd05-105">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="abd05-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="abd05-106">Property</span></span> |<span data-ttu-id="abd05-107">Тип</span><span class="sxs-lookup"><span data-stu-id="abd05-107">Type</span></span> |<span data-ttu-id="abd05-108">Описание</span><span class="sxs-lookup"><span data-stu-id="abd05-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="abd05-109">цертификатионнаме</span><span class="sxs-lookup"><span data-stu-id="abd05-109">certificationName</span></span> | <span data-ttu-id="abd05-110">string</span><span class="sxs-lookup"><span data-stu-id="abd05-110">string</span></span> | <span data-ttu-id="abd05-111">Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171).</span><span class="sxs-lookup"><span data-stu-id="abd05-111">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="abd05-112">цертификатионконтролс</span><span class="sxs-lookup"><span data-stu-id="abd05-112">certificationControls</span></span> | <span data-ttu-id="abd05-113">Коллекция [цертификатионконтрол](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="abd05-113">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="abd05-114">Коллекция элементов управления сертификацией, связанных с сертификацией</span><span class="sxs-lookup"><span data-stu-id="abd05-114">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="abd05-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="abd05-115">JSON representation</span></span>

<span data-ttu-id="abd05-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="abd05-116">The following is a JSON representation of the resource.</span></span>

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
