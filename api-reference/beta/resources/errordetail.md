---
title: Тип ресурса Еррордетаил
description: Описание ошибки неудачного запроса на асинхронное создание схемы подключения Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7f77ccacd6e1f5339706549873ea4c75d9144e39
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704187"
---
# <a name="errordetail-resource-type"></a><span data-ttu-id="dcf90-103">Тип ресурса Еррордетаил</span><span class="sxs-lookup"><span data-stu-id="dcf90-103">errorDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcf90-104">Описание ошибки неудачного запроса на асинхронное создание [схемы](schema.md) подключения Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="dcf90-104">Describes an error for a failed request to create a Microsoft Search connection [schema](schema.md) asynchronously.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="dcf90-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="dcf90-105">Properties</span></span>

| <span data-ttu-id="dcf90-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="dcf90-106">Property</span></span>  | <span data-ttu-id="dcf90-107">Тип</span><span class="sxs-lookup"><span data-stu-id="dcf90-107">Type</span></span>                                               | <span data-ttu-id="dcf90-108">Описание</span><span class="sxs-lookup"><span data-stu-id="dcf90-108">Description</span></span> |
|:----------|:---------------------------------------------------|:------------|
| <span data-ttu-id="dcf90-109">подробности</span><span class="sxs-lookup"><span data-stu-id="dcf90-109">details</span></span>   | <span data-ttu-id="dcf90-110">Коллекция [иннереррордетаил](innererrordetail.md)</span><span class="sxs-lookup"><span data-stu-id="dcf90-110">[innerErrorDetail](innererrordetail.md) collection</span></span> | <span data-ttu-id="dcf90-111">Коллекция внутренних ошибок (при наличии).</span><span class="sxs-lookup"><span data-stu-id="dcf90-111">A collection of inner errors, if any.</span></span> <span data-ttu-id="dcf90-112">Только для чтения, допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="dcf90-112">Read-only, nullable.</span></span> |
| <span data-ttu-id="dcf90-113">errorCode</span><span class="sxs-lookup"><span data-stu-id="dcf90-113">errorCode</span></span> | <span data-ttu-id="dcf90-114">String</span><span class="sxs-lookup"><span data-stu-id="dcf90-114">String</span></span>                                             | <span data-ttu-id="dcf90-115">Код ошибки, связанный с ошибкой (при наличии).</span><span class="sxs-lookup"><span data-stu-id="dcf90-115">The error code associated with the error, if any.</span></span> <span data-ttu-id="dcf90-116">Только для чтения, допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="dcf90-116">Read-only, nullable.</span></span> |
| <span data-ttu-id="dcf90-117">message</span><span class="sxs-lookup"><span data-stu-id="dcf90-117">message</span></span>   | <span data-ttu-id="dcf90-118">String</span><span class="sxs-lookup"><span data-stu-id="dcf90-118">String</span></span>                                             | <span data-ttu-id="dcf90-119">Сообщение об ошибке, читаемое человеком.</span><span class="sxs-lookup"><span data-stu-id="dcf90-119">The human-readable error message.</span></span> <span data-ttu-id="dcf90-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dcf90-120">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dcf90-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dcf90-121">JSON representation</span></span>

<span data-ttu-id="dcf90-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dcf90-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "details",
    "errorCode"
  ],
  "@odata.type": "microsoft.graph.errorDetail",
  "baseType": null
}-->

```json
{
  "details": [{"@odata.type": "microsoft.graph.innerErrorDetail"}],
  "errorCode": "String",
  "message": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "errorDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
