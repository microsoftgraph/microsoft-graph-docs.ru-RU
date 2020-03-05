---
title: " Тип ресурса Комплианцеинформатион"
description: Этот ресурс содержит данные соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 65eda1c24fee112ef18fc6682b537f92f924dcf8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507578"
---
#  <a name="complianceinformation-resource-type"></a><span data-ttu-id="a1cd9-103">Тип ресурса Комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="a1cd9-103">complianceInformation resource type</span></span>

<span data-ttu-id="a1cd9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a1cd9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1cd9-105">Содержит данные соответствия требованиям, связанные с контролем безопасного рейтинга.</span><span class="sxs-lookup"><span data-stu-id="a1cd9-105">Contains compliance data associated with secure score control.</span></span>

|<span data-ttu-id="a1cd9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1cd9-106">Property</span></span> |<span data-ttu-id="a1cd9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a1cd9-107">Type</span></span> |<span data-ttu-id="a1cd9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a1cd9-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="a1cd9-109">цертификатионнаме</span><span class="sxs-lookup"><span data-stu-id="a1cd9-109">certificationName</span></span> | <span data-ttu-id="a1cd9-110">строка</span><span class="sxs-lookup"><span data-stu-id="a1cd9-110">string</span></span> | <span data-ttu-id="a1cd9-111">Имя сертификации соответствия (например, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171).</span><span class="sxs-lookup"><span data-stu-id="a1cd9-111">Compliance certification name (for example, ISO 27018:2014, GDPR, FedRAMP, NIST 800-171)</span></span> |
|<span data-ttu-id="a1cd9-112">цертификатионконтролс</span><span class="sxs-lookup"><span data-stu-id="a1cd9-112">certificationControls</span></span> | <span data-ttu-id="a1cd9-113">Коллекция [цертификатионконтрол](certificationcontrol.md)</span><span class="sxs-lookup"><span data-stu-id="a1cd9-113">[certificationControl](certificationcontrol.md) collection</span></span> | <span data-ttu-id="a1cd9-114">Коллекция элементов управления сертификацией, связанных с сертификацией</span><span class="sxs-lookup"><span data-stu-id="a1cd9-114">Collection of the certification controls associated with certification</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a1cd9-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a1cd9-115">JSON representation</span></span>

<span data-ttu-id="a1cd9-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1cd9-116">The following is a JSON representation of the resource.</span></span>

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
