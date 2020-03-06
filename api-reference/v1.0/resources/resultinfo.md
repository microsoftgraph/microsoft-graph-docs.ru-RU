---
title: Тип ресурса Ресултинфо
description: Содержит сведения о результатах успешного выполнения и сбоя.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 42b636b09e8cfeb2ed41578e06fc57b5aa976fd5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533820"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="b731c-103">Тип ресурса Ресултинфо</span><span class="sxs-lookup"><span data-stu-id="b731c-103">resultInfo resource type</span></span>

<span data-ttu-id="b731c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b731c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b731c-105">Содержит сведения о результатах успешного выполнения и сбоя.</span><span class="sxs-lookup"><span data-stu-id="b731c-105">This contains success and failure specific result information.</span></span> 

<span data-ttu-id="b731c-106">Код указывает, является ли результат универсальным успехом или ошибкой.</span><span class="sxs-lookup"><span data-stu-id="b731c-106">The code specifies if the result is a generic success or failure.</span></span> <span data-ttu-id="b731c-107">Если код 2xx это успех, то в случае, если это 4xx ошибка клиента, и если это значение 5xx, то это может быть ошибка сервера.</span><span class="sxs-lookup"><span data-stu-id="b731c-107">If the code is 2xx it's a success, if it's a 4xx it's a client error, and if it's 5xx, it's a server error.</span></span>

<span data-ttu-id="b731c-108">Дочерние коды предоставляют дополнительные сведения, связанные с типом успеха или сбоем (например, успешная передача вызова).</span><span class="sxs-lookup"><span data-stu-id="b731c-108">The sub-codes provide supplementary information related to the type of success or failure (e.g. a call transfer was successful)</span></span>


## <a name="properties"></a><span data-ttu-id="b731c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b731c-109">Properties</span></span>

| <span data-ttu-id="b731c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b731c-110">Property</span></span> | <span data-ttu-id="b731c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b731c-111">Type</span></span>   | <span data-ttu-id="b731c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b731c-112">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="b731c-113">code</span><span class="sxs-lookup"><span data-stu-id="b731c-113">code</span></span>     | <span data-ttu-id="b731c-114">Int32</span><span class="sxs-lookup"><span data-stu-id="b731c-114">Int32</span></span> | <span data-ttu-id="b731c-115">Код результата.</span><span class="sxs-lookup"><span data-stu-id="b731c-115">The result code.</span></span>     |
| <span data-ttu-id="b731c-116">message</span><span class="sxs-lookup"><span data-stu-id="b731c-116">message</span></span>  | <span data-ttu-id="b731c-117">String</span><span class="sxs-lookup"><span data-stu-id="b731c-117">String</span></span> | <span data-ttu-id="b731c-118">Сообщение.</span><span class="sxs-lookup"><span data-stu-id="b731c-118">The message.</span></span>         |
| <span data-ttu-id="b731c-119">Subcode</span><span class="sxs-lookup"><span data-stu-id="b731c-119">subcode</span></span>  | <span data-ttu-id="b731c-120">Int32</span><span class="sxs-lookup"><span data-stu-id="b731c-120">Int32</span></span> | <span data-ttu-id="b731c-121">Дочерний код результата.</span><span class="sxs-lookup"><span data-stu-id="b731c-121">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b731c-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b731c-122">JSON representation</span></span>

<span data-ttu-id="b731c-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b731c-123">The following is a JSON representation of the resource.</span></span>

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
