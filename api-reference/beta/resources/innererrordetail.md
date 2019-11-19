---
title: Тип ресурса Иннереррордетаил
description: Внутренняя ошибка, которая находится в объекте Еррордетаил
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6b3dfb2ec4caf8ae2b8ec9a279a6d001ad3aaae7
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703779"
---
# <a name="innererrordetail-resource-type"></a><span data-ttu-id="cb476-103">Тип ресурса Иннереррордетаил</span><span class="sxs-lookup"><span data-stu-id="cb476-103">innerErrorDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb476-104">Внутренняя ошибка, которая находится в объекте [еррордетаил](errordetail.md)</span><span class="sxs-lookup"><span data-stu-id="cb476-104">An inner error contained in an [errorDetail](errordetail.md) object.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="cb476-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb476-105">Properties</span></span>

| <span data-ttu-id="cb476-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb476-106">Property</span></span> | <span data-ttu-id="cb476-107">Тип</span><span class="sxs-lookup"><span data-stu-id="cb476-107">Type</span></span>   | <span data-ttu-id="cb476-108">Описание</span><span class="sxs-lookup"><span data-stu-id="cb476-108">Description</span></span>                                  |
|:---------|:-------|:---------------------------------------------|
| <span data-ttu-id="cb476-109">message</span><span class="sxs-lookup"><span data-stu-id="cb476-109">message</span></span>  | <span data-ttu-id="cb476-110">String</span><span class="sxs-lookup"><span data-stu-id="cb476-110">String</span></span> | <span data-ttu-id="cb476-111">Сообщение об ошибке, читаемое человеком.</span><span class="sxs-lookup"><span data-stu-id="cb476-111">The human-readable error message.</span></span> <span data-ttu-id="cb476-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb476-112">Read-only.</span></span> |
| <span data-ttu-id="cb476-113">source</span><span class="sxs-lookup"><span data-stu-id="cb476-113">source</span></span>   | <span data-ttu-id="cb476-114">String</span><span class="sxs-lookup"><span data-stu-id="cb476-114">String</span></span> | <span data-ttu-id="cb476-115">Источник ошибки.</span><span class="sxs-lookup"><span data-stu-id="cb476-115">The source of the error.</span></span> <span data-ttu-id="cb476-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb476-116">Read-only.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="cb476-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb476-117">JSON representation</span></span>

<span data-ttu-id="cb476-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb476-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.innerErrorDetail",
  "baseType": null
}-->

```json
{
  "message": "String",
  "source": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "innerErrorDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
