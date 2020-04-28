---
title: Тип ресурса Ресултинфо
description: Содержит сведения о результатах, относящиеся к успехам и сбоям.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: aa55f8cdcb7ca4639aa4975a28ae2bcbcd625588
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521084"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="a5bc9-103">Тип ресурса Ресултинфо</span><span class="sxs-lookup"><span data-stu-id="a5bc9-103">resultInfo resource type</span></span>

<span data-ttu-id="a5bc9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5bc9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5bc9-105">Содержит сведения о результатах, относящиеся к успехам и сбоям.</span><span class="sxs-lookup"><span data-stu-id="a5bc9-105">Contains success and failure-specific result information.</span></span> 

<span data-ttu-id="a5bc9-106">Код указывает, является ли результат универсальным успехом или ошибкой.</span><span class="sxs-lookup"><span data-stu-id="a5bc9-106">The code specifies whether the result is a generic success or failure.</span></span> 

<span data-ttu-id="a5bc9-107">Вспомогательные коды предоставляют дополнительные сведения, связанные с типом успешного или неудачного завершения (например, успешная передача вызова).</span><span class="sxs-lookup"><span data-stu-id="a5bc9-107">The subcodes provide supplementary information related to the type of success or failure (for example, a call transfer was successful).</span></span>


## <a name="properties"></a><span data-ttu-id="a5bc9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5bc9-108">Properties</span></span>

| <span data-ttu-id="a5bc9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5bc9-109">Property</span></span> | <span data-ttu-id="a5bc9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a5bc9-110">Type</span></span>   | <span data-ttu-id="a5bc9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a5bc9-111">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="a5bc9-112">code</span><span class="sxs-lookup"><span data-stu-id="a5bc9-112">code</span></span>     | <span data-ttu-id="a5bc9-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a5bc9-113">Int32</span></span> | <span data-ttu-id="a5bc9-114">Код результата.</span><span class="sxs-lookup"><span data-stu-id="a5bc9-114">The result code.</span></span>     |
| <span data-ttu-id="a5bc9-115">message</span><span class="sxs-lookup"><span data-stu-id="a5bc9-115">message</span></span>  | <span data-ttu-id="a5bc9-116">String</span><span class="sxs-lookup"><span data-stu-id="a5bc9-116">String</span></span> | <span data-ttu-id="a5bc9-117">Сообщение.</span><span class="sxs-lookup"><span data-stu-id="a5bc9-117">The message.</span></span>         |
| <span data-ttu-id="a5bc9-118">Subcode</span><span class="sxs-lookup"><span data-stu-id="a5bc9-118">subcode</span></span>  | <span data-ttu-id="a5bc9-119">Int32</span><span class="sxs-lookup"><span data-stu-id="a5bc9-119">Int32</span></span> | <span data-ttu-id="a5bc9-120">Дочерний код результата.</span><span class="sxs-lookup"><span data-stu-id="a5bc9-120">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a5bc9-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5bc9-121">JSON representation</span></span>

<span data-ttu-id="a5bc9-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5bc9-122">The following is a JSON representation of the resource.</span></span>

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
