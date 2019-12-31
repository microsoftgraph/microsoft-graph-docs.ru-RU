---
title: Тип ресурса Ресултинфо
description: Содержит сведения о результатах успешного выполнения и сбоя.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 230783192e936d3fb3c2799e6cb98d39492589a3
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913410"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="e9bc5-103">Тип ресурса Ресултинфо</span><span class="sxs-lookup"><span data-stu-id="e9bc5-103">resultInfo resource type</span></span>

<span data-ttu-id="e9bc5-104">Содержит сведения о результатах успешного выполнения и сбоя.</span><span class="sxs-lookup"><span data-stu-id="e9bc5-104">This contains success and failure specific result information.</span></span> 

<span data-ttu-id="e9bc5-105">Код указывает, является ли результат универсальным успехом или ошибкой.</span><span class="sxs-lookup"><span data-stu-id="e9bc5-105">The code specifies if the result is a generic success or failure.</span></span> <span data-ttu-id="e9bc5-106">Если код 2xx это успех, то в случае, если это 4xx ошибка клиента, и если это значение 5xx, то это может быть ошибка сервера.</span><span class="sxs-lookup"><span data-stu-id="e9bc5-106">If the code is 2xx it's a success, if it's a 4xx it's a client error, and if it's 5xx, it's a server error.</span></span>

<span data-ttu-id="e9bc5-107">Дочерние коды предоставляют дополнительные сведения, связанные с типом успеха или сбоем (например, успешная передача вызова).</span><span class="sxs-lookup"><span data-stu-id="e9bc5-107">The sub-codes provide supplementary information related to the type of success or failure (e.g. a call transfer was successful)</span></span>


## <a name="properties"></a><span data-ttu-id="e9bc5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9bc5-108">Properties</span></span>

| <span data-ttu-id="e9bc5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9bc5-109">Property</span></span> | <span data-ttu-id="e9bc5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e9bc5-110">Type</span></span>   | <span data-ttu-id="e9bc5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e9bc5-111">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="e9bc5-112">code</span><span class="sxs-lookup"><span data-stu-id="e9bc5-112">code</span></span>     | <span data-ttu-id="e9bc5-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e9bc5-113">Int32</span></span> | <span data-ttu-id="e9bc5-114">Код результата.</span><span class="sxs-lookup"><span data-stu-id="e9bc5-114">The result code.</span></span>     |
| <span data-ttu-id="e9bc5-115">message</span><span class="sxs-lookup"><span data-stu-id="e9bc5-115">message</span></span>  | <span data-ttu-id="e9bc5-116">String</span><span class="sxs-lookup"><span data-stu-id="e9bc5-116">String</span></span> | <span data-ttu-id="e9bc5-117">Сообщение.</span><span class="sxs-lookup"><span data-stu-id="e9bc5-117">The message.</span></span>         |
| <span data-ttu-id="e9bc5-118">Subcode</span><span class="sxs-lookup"><span data-stu-id="e9bc5-118">subcode</span></span>  | <span data-ttu-id="e9bc5-119">Int32</span><span class="sxs-lookup"><span data-stu-id="e9bc5-119">Int32</span></span> | <span data-ttu-id="e9bc5-120">Дочерний код результата.</span><span class="sxs-lookup"><span data-stu-id="e9bc5-120">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e9bc5-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9bc5-121">JSON representation</span></span>

<span data-ttu-id="e9bc5-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9bc5-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": 0,
  "message": "String",
  "subcode": 0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
