---
title: " Тип ресурса certificationControl"
description: Этот ресурс содержит соответствия требованиям сертификации данные, связанные с безопасного элемента управления показателя.
localization_priority: Normal
ms.openlocfilehash: 6f8269a85a8d3cb032f3e58457df95f4dd432c11
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810390"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="ab088-103">Тип ресурса certificationControl</span><span class="sxs-lookup"><span data-stu-id="ab088-103">certificationControl resource type</span></span>

<span data-ttu-id="ab088-104">Содержит соответствия требованиям сертификации данные, связанные с безопасного элемента управления показателя.</span><span class="sxs-lookup"><span data-stu-id="ab088-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="ab088-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab088-105">Property</span></span> |<span data-ttu-id="ab088-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ab088-106">Type</span></span> |<span data-ttu-id="ab088-107">Описание</span><span class="sxs-lookup"><span data-stu-id="ab088-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="ab088-108">name</span><span class="sxs-lookup"><span data-stu-id="ab088-108">name</span></span> | <span data-ttu-id="ab088-109">строка</span><span class="sxs-lookup"><span data-stu-id="ab088-109">string</span></span> | <span data-ttu-id="ab088-110">Имя элемента управления сертификации</span><span class="sxs-lookup"><span data-stu-id="ab088-110">Certification control name</span></span> |
|<span data-ttu-id="ab088-111">url</span><span class="sxs-lookup"><span data-stu-id="ab088-111">url</span></span> | <span data-ttu-id="ab088-112">строка</span><span class="sxs-lookup"><span data-stu-id="ab088-112">string</span></span> | <span data-ttu-id="ab088-113">URL-адрес для службы Microsoft доверять портала</span><span class="sxs-lookup"><span data-stu-id="ab088-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ab088-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab088-114">JSON representation</span></span>

<span data-ttu-id="ab088-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab088-115">The following is a JSON representation of the resource.</span></span>

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
