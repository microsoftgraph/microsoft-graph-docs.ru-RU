---
title: Тип ресурса Комплианцеинформатион
description: Этот ресурс содержит данные соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ef62f6df73c24f9e6b3884921865c28ea152a3dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533038"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="26583-103">Тип ресурса Комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="26583-103">complianceInformation resource type</span></span>

<span data-ttu-id="26583-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26583-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="26583-105">Содержит данные соответствия требованиям, связанные с контролем безопасного рейтинга.</span><span class="sxs-lookup"><span data-stu-id="26583-105">Contains compliance data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="26583-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="26583-106">Properties</span></span>

|<span data-ttu-id="26583-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="26583-107">Property</span></span> |<span data-ttu-id="26583-108">Тип</span><span class="sxs-lookup"><span data-stu-id="26583-108">Type</span></span> |<span data-ttu-id="26583-109">Описание</span><span class="sxs-lookup"><span data-stu-id="26583-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="26583-110">цертификатионнаме</span><span class="sxs-lookup"><span data-stu-id="26583-110">certificationName</span></span>|<span data-ttu-id="26583-111">Строка</span><span class="sxs-lookup"><span data-stu-id="26583-111">String</span></span>| <span data-ttu-id="26583-112">Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171).</span><span class="sxs-lookup"><span data-stu-id="26583-112">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="26583-113">цертификатионконтролс</span><span class="sxs-lookup"><span data-stu-id="26583-113">certificationControls</span></span>|<span data-ttu-id="26583-114">Коллекция [цертификатионконтрол](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="26583-114">[certificationControl](certificationcontrol.md) collection</span></span>|<span data-ttu-id="26583-115">Коллекция элементов управления сертификацией, связанных с сертификацией</span><span class="sxs-lookup"><span data-stu-id="26583-115">Collection of the certification controls associated with certification</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26583-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26583-116">JSON representation</span></span>

<span data-ttu-id="26583-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26583-117">The following is a JSON representation of the resource.</span></span>

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
