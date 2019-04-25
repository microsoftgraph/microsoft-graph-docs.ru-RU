---
title: " Тип ресурса Цертификатионконтрол"
description: Этот ресурс содержит данные сертификации соответствия требованиям, связанные с контролем безопасности по показателю.
localization_priority: Normal
ms.openlocfilehash: 6f8269a85a8d3cb032f3e58457df95f4dd432c11
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535415"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="13752-103">Тип ресурса Цертификатионконтрол</span><span class="sxs-lookup"><span data-stu-id="13752-103">certificationControl resource type</span></span>

<span data-ttu-id="13752-104">Содержит данные сертификации соответствия требованиям, связанные с контролем безопасного индекса.</span><span class="sxs-lookup"><span data-stu-id="13752-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="13752-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="13752-105">Property</span></span> |<span data-ttu-id="13752-106">Тип</span><span class="sxs-lookup"><span data-stu-id="13752-106">Type</span></span> |<span data-ttu-id="13752-107">Описание</span><span class="sxs-lookup"><span data-stu-id="13752-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="13752-108">name</span><span class="sxs-lookup"><span data-stu-id="13752-108">name</span></span> | <span data-ttu-id="13752-109">string</span><span class="sxs-lookup"><span data-stu-id="13752-109">string</span></span> | <span data-ttu-id="13752-110">Имя элемента управления сертификацией</span><span class="sxs-lookup"><span data-stu-id="13752-110">Certification control name</span></span> |
|<span data-ttu-id="13752-111">url</span><span class="sxs-lookup"><span data-stu-id="13752-111">url</span></span> | <span data-ttu-id="13752-112">string</span><span class="sxs-lookup"><span data-stu-id="13752-112">string</span></span> | <span data-ttu-id="13752-113">URL-адрес портала доверия службы Майкрософт</span><span class="sxs-lookup"><span data-stu-id="13752-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="13752-114">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="13752-114">JSON representation</span></span>

<span data-ttu-id="13752-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13752-115">The following is a JSON representation of the resource.</span></span>

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
