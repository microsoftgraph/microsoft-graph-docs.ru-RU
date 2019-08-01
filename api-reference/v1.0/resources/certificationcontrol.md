---
title: Тип ресурса Цертификатионконтрол
description: Этот ресурс содержит данные сертификации соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ad7c07d269f9dc627de41db621e4d73f0d2c10b0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029906"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="c4ffb-103">Тип ресурса Цертификатионконтрол</span><span class="sxs-lookup"><span data-stu-id="c4ffb-103">certificationControl resource type</span></span>

<span data-ttu-id="c4ffb-104">Содержит данные сертификации соответствия требованиям, связанные с контролем безопасного индекса.</span><span class="sxs-lookup"><span data-stu-id="c4ffb-104">Contains compliance certification data associated with secure score control.</span></span>

## <a name="properties"></a><span data-ttu-id="c4ffb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4ffb-105">Properties</span></span>

|<span data-ttu-id="c4ffb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4ffb-106">Property</span></span> |<span data-ttu-id="c4ffb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c4ffb-107">Type</span></span> |<span data-ttu-id="c4ffb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c4ffb-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="c4ffb-109">name</span><span class="sxs-lookup"><span data-stu-id="c4ffb-109">name</span></span>|<span data-ttu-id="c4ffb-110">String</span><span class="sxs-lookup"><span data-stu-id="c4ffb-110">String</span></span>|<span data-ttu-id="c4ffb-111">Имя элемента управления сертификацией</span><span class="sxs-lookup"><span data-stu-id="c4ffb-111">Certification control name</span></span> |
|<span data-ttu-id="c4ffb-112">url</span><span class="sxs-lookup"><span data-stu-id="c4ffb-112">url</span></span>|<span data-ttu-id="c4ffb-113">String</span><span class="sxs-lookup"><span data-stu-id="c4ffb-113">String</span></span>|<span data-ttu-id="c4ffb-114">URL-адрес портала доверия службы Майкрософт</span><span class="sxs-lookup"><span data-stu-id="c4ffb-114">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c4ffb-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4ffb-115">JSON representation</span></span>

<span data-ttu-id="c4ffb-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4ffb-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificationControl"
}-->

```json
{
  "name": "String",
  "url": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
