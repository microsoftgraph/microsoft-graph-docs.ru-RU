---
title: " Тип ресурса certificationControl"
description: Этот ресурс содержит соответствия требованиям сертификации данные, связанные с безопасного элемента управления показателя.
ms.openlocfilehash: 62b6627a9bb1a012d6d7e542d87abbaddb0e279a
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380947"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="db3d2-103">Тип ресурса certificationControl</span><span class="sxs-lookup"><span data-stu-id="db3d2-103">certificationControl resource type</span></span>

<span data-ttu-id="db3d2-104">Содержит соответствия требованиям сертификации данные, связанные с безопасного элемента управления показателя.</span><span class="sxs-lookup"><span data-stu-id="db3d2-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="db3d2-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="db3d2-105">Property</span></span> |<span data-ttu-id="db3d2-106">Тип</span><span class="sxs-lookup"><span data-stu-id="db3d2-106">Type</span></span> |<span data-ttu-id="db3d2-107">Описание</span><span class="sxs-lookup"><span data-stu-id="db3d2-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="db3d2-108">name</span><span class="sxs-lookup"><span data-stu-id="db3d2-108">name</span></span> | <span data-ttu-id="db3d2-109">строка</span><span class="sxs-lookup"><span data-stu-id="db3d2-109">string</span></span> | <span data-ttu-id="db3d2-110">Имя элемента управления сертификации</span><span class="sxs-lookup"><span data-stu-id="db3d2-110">Certification control name</span></span> |
|<span data-ttu-id="db3d2-111">url</span><span class="sxs-lookup"><span data-stu-id="db3d2-111">url</span></span> | <span data-ttu-id="db3d2-112">строка</span><span class="sxs-lookup"><span data-stu-id="db3d2-112">string</span></span> | <span data-ttu-id="db3d2-113">URL-адрес для службы Microsoft доверять портала</span><span class="sxs-lookup"><span data-stu-id="db3d2-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="db3d2-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db3d2-114">JSON representation</span></span>

<span data-ttu-id="db3d2-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db3d2-115">The following is a JSON representation of the resource.</span></span>

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
