---
title: " Тип ресурса Цертификатионконтрол"
description: Этот ресурс содержит данные сертификации соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 4f2be439f1b286a8d916fe80a7b4fcb4f6d60071
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016823"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="5fe81-103">Тип ресурса Цертификатионконтрол</span><span class="sxs-lookup"><span data-stu-id="5fe81-103">certificationControl resource type</span></span>

<span data-ttu-id="5fe81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fe81-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5fe81-105">Содержит данные сертификации соответствия требованиям, связанные с контролем безопасного индекса.</span><span class="sxs-lookup"><span data-stu-id="5fe81-105">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="5fe81-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fe81-106">Property</span></span> |<span data-ttu-id="5fe81-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5fe81-107">Type</span></span> |<span data-ttu-id="5fe81-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5fe81-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="5fe81-109">name</span><span class="sxs-lookup"><span data-stu-id="5fe81-109">name</span></span> | <span data-ttu-id="5fe81-110">string</span><span class="sxs-lookup"><span data-stu-id="5fe81-110">string</span></span> | <span data-ttu-id="5fe81-111">Имя элемента управления сертификацией</span><span class="sxs-lookup"><span data-stu-id="5fe81-111">Certification control name</span></span> |
|<span data-ttu-id="5fe81-112">url</span><span class="sxs-lookup"><span data-stu-id="5fe81-112">url</span></span> | <span data-ttu-id="5fe81-113">string</span><span class="sxs-lookup"><span data-stu-id="5fe81-113">string</span></span> | <span data-ttu-id="5fe81-114">URL-адрес портала доверия службы Майкрософт</span><span class="sxs-lookup"><span data-stu-id="5fe81-114">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5fe81-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5fe81-115">JSON representation</span></span>

<span data-ttu-id="5fe81-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fe81-116">The following is a JSON representation of the resource.</span></span>

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


