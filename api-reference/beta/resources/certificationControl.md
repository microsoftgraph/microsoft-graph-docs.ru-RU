---
title: " Тип ресурса Цертификатионконтрол"
description: Этот ресурс содержит данные сертификации соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 22dc12070a801988d814ba73c6bffe1414bb5218
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012998"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="8d778-103">Тип ресурса Цертификатионконтрол</span><span class="sxs-lookup"><span data-stu-id="8d778-103">certificationControl resource type</span></span>

<span data-ttu-id="8d778-104">Содержит данные сертификации соответствия требованиям, связанные с контролем безопасного индекса.</span><span class="sxs-lookup"><span data-stu-id="8d778-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="8d778-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d778-105">Property</span></span> |<span data-ttu-id="8d778-106">Тип</span><span class="sxs-lookup"><span data-stu-id="8d778-106">Type</span></span> |<span data-ttu-id="8d778-107">Описание</span><span class="sxs-lookup"><span data-stu-id="8d778-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="8d778-108">name</span><span class="sxs-lookup"><span data-stu-id="8d778-108">name</span></span> | <span data-ttu-id="8d778-109">string</span><span class="sxs-lookup"><span data-stu-id="8d778-109">string</span></span> | <span data-ttu-id="8d778-110">Имя элемента управления сертификацией</span><span class="sxs-lookup"><span data-stu-id="8d778-110">Certification control name</span></span> |
|<span data-ttu-id="8d778-111">url</span><span class="sxs-lookup"><span data-stu-id="8d778-111">url</span></span> | <span data-ttu-id="8d778-112">string</span><span class="sxs-lookup"><span data-stu-id="8d778-112">string</span></span> | <span data-ttu-id="8d778-113">URL-адрес портала доверия службы Майкрософт</span><span class="sxs-lookup"><span data-stu-id="8d778-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8d778-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d778-114">JSON representation</span></span>

<span data-ttu-id="8d778-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d778-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificationControl"
}-->

```json
{
  "name": "String",
  "url": "Collection(microsoft.graph.certificationControl)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
