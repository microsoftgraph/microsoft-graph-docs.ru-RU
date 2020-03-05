---
title: " Тип ресурса Цертификатионконтрол"
description: Этот ресурс содержит данные сертификации соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bafd2c9d66c0d696649944f88e4fcfbdea4bcca6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507763"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="062c4-103">Тип ресурса Цертификатионконтрол</span><span class="sxs-lookup"><span data-stu-id="062c4-103">certificationControl resource type</span></span>

<span data-ttu-id="062c4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="062c4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="062c4-105">Содержит данные сертификации соответствия требованиям, связанные с контролем безопасного индекса.</span><span class="sxs-lookup"><span data-stu-id="062c4-105">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="062c4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="062c4-106">Property</span></span> |<span data-ttu-id="062c4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="062c4-107">Type</span></span> |<span data-ttu-id="062c4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="062c4-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="062c4-109">name</span><span class="sxs-lookup"><span data-stu-id="062c4-109">name</span></span> | <span data-ttu-id="062c4-110">string</span><span class="sxs-lookup"><span data-stu-id="062c4-110">string</span></span> | <span data-ttu-id="062c4-111">Имя элемента управления сертификацией</span><span class="sxs-lookup"><span data-stu-id="062c4-111">Certification control name</span></span> |
|<span data-ttu-id="062c4-112">url</span><span class="sxs-lookup"><span data-stu-id="062c4-112">url</span></span> | <span data-ttu-id="062c4-113">string</span><span class="sxs-lookup"><span data-stu-id="062c4-113">string</span></span> | <span data-ttu-id="062c4-114">URL-адрес портала доверия службы Майкрософт</span><span class="sxs-lookup"><span data-stu-id="062c4-114">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="062c4-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="062c4-115">JSON representation</span></span>

<span data-ttu-id="062c4-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="062c4-116">The following is a JSON representation of the resource.</span></span>

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
