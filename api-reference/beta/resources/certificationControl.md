---
title: " Тип ресурса Цертификатионконтрол"
description: Этот ресурс содержит данные сертификации соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f6ecfa2ffddd362ba6c166d9dc839aedaf6f4723
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810582"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="e3291-103">Тип ресурса Цертификатионконтрол</span><span class="sxs-lookup"><span data-stu-id="e3291-103">certificationControl resource type</span></span>

<span data-ttu-id="e3291-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3291-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3291-105">Содержит данные сертификации соответствия требованиям, связанные с контролем безопасного индекса.</span><span class="sxs-lookup"><span data-stu-id="e3291-105">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="e3291-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3291-106">Property</span></span> |<span data-ttu-id="e3291-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e3291-107">Type</span></span> |<span data-ttu-id="e3291-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e3291-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="e3291-109">name</span><span class="sxs-lookup"><span data-stu-id="e3291-109">name</span></span> | <span data-ttu-id="e3291-110">string</span><span class="sxs-lookup"><span data-stu-id="e3291-110">string</span></span> | <span data-ttu-id="e3291-111">Имя элемента управления сертификацией</span><span class="sxs-lookup"><span data-stu-id="e3291-111">Certification control name</span></span> |
|<span data-ttu-id="e3291-112">url</span><span class="sxs-lookup"><span data-stu-id="e3291-112">url</span></span> | <span data-ttu-id="e3291-113">string</span><span class="sxs-lookup"><span data-stu-id="e3291-113">string</span></span> | <span data-ttu-id="e3291-114">URL-адрес портала доверия службы Майкрософт</span><span class="sxs-lookup"><span data-stu-id="e3291-114">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e3291-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e3291-115">JSON representation</span></span>

<span data-ttu-id="e3291-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3291-116">The following is a JSON representation of the resource.</span></span>

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
