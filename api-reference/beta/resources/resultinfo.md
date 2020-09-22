---
title: Тип ресурса Ресултинфо
description: Содержит сведения о результатах, относящиеся к успехам и сбоям.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7202cd0bfa7dee3db3e37d2cab4333da49a41856
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026245"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="2b591-103">Тип ресурса Ресултинфо</span><span class="sxs-lookup"><span data-stu-id="2b591-103">resultInfo resource type</span></span>

<span data-ttu-id="2b591-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b591-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b591-105">Содержит сведения о результатах, относящиеся к успехам и сбоям.</span><span class="sxs-lookup"><span data-stu-id="2b591-105">Contains success and failure-specific result information.</span></span> 

<span data-ttu-id="2b591-106">Код указывает, является ли результат универсальным успехом или ошибкой.</span><span class="sxs-lookup"><span data-stu-id="2b591-106">The code specifies whether the result is a generic success or failure.</span></span> 

<span data-ttu-id="2b591-107">Вспомогательные коды предоставляют дополнительные сведения, связанные с типом успешного или неудачного завершения (например, успешная передача вызова).</span><span class="sxs-lookup"><span data-stu-id="2b591-107">The subcodes provide supplementary information related to the type of success or failure (for example, a call transfer was successful).</span></span>


## <a name="properties"></a><span data-ttu-id="2b591-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b591-108">Properties</span></span>

| <span data-ttu-id="2b591-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b591-109">Property</span></span> | <span data-ttu-id="2b591-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2b591-110">Type</span></span>   | <span data-ttu-id="2b591-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2b591-111">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="2b591-112">code</span><span class="sxs-lookup"><span data-stu-id="2b591-112">code</span></span>     | <span data-ttu-id="2b591-113">Int32</span><span class="sxs-lookup"><span data-stu-id="2b591-113">Int32</span></span> | <span data-ttu-id="2b591-114">Код результата.</span><span class="sxs-lookup"><span data-stu-id="2b591-114">The result code.</span></span>     |
| <span data-ttu-id="2b591-115">message</span><span class="sxs-lookup"><span data-stu-id="2b591-115">message</span></span>  | <span data-ttu-id="2b591-116">String</span><span class="sxs-lookup"><span data-stu-id="2b591-116">String</span></span> | <span data-ttu-id="2b591-117">Сообщение.</span><span class="sxs-lookup"><span data-stu-id="2b591-117">The message.</span></span>         |
| <span data-ttu-id="2b591-118">Subcode</span><span class="sxs-lookup"><span data-stu-id="2b591-118">subcode</span></span>  | <span data-ttu-id="2b591-119">Int32</span><span class="sxs-lookup"><span data-stu-id="2b591-119">Int32</span></span> | <span data-ttu-id="2b591-120">Дочерний код результата.</span><span class="sxs-lookup"><span data-stu-id="2b591-120">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2b591-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b591-121">JSON representation</span></span>

<span data-ttu-id="2b591-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b591-122">The following is a JSON representation of the resource.</span></span>

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


