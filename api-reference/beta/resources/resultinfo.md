---
title: Тип ресурса Ресултинфо
description: Содержит сведения о результатах, относящиеся к успехам и сбоям.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5cb59cb63ff7c50ba14b972991d54806eabc4f54
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866632"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="54550-103">Тип ресурса Ресултинфо</span><span class="sxs-lookup"><span data-stu-id="54550-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54550-104">Содержит сведения о результатах, относящиеся к успехам и сбоям.</span><span class="sxs-lookup"><span data-stu-id="54550-104">Contains success and failure-specific result information.</span></span> 

<span data-ttu-id="54550-105">Код указывает, является ли результат универсальным успехом или ошибкой.</span><span class="sxs-lookup"><span data-stu-id="54550-105">The code specifies whether the result is a generic success or failure.</span></span> 

<span data-ttu-id="54550-106">Вспомогательные коды предоставляют дополнительные сведения, связанные с типом успешного или неудачного завершения (например, успешная передача вызова).</span><span class="sxs-lookup"><span data-stu-id="54550-106">The subcodes provide supplementary information related to the type of success or failure (for example, a call transfer was successful).</span></span>


## <a name="properties"></a><span data-ttu-id="54550-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="54550-107">Properties</span></span>

| <span data-ttu-id="54550-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="54550-108">Property</span></span> | <span data-ttu-id="54550-109">Тип</span><span class="sxs-lookup"><span data-stu-id="54550-109">Type</span></span>   | <span data-ttu-id="54550-110">Описание</span><span class="sxs-lookup"><span data-stu-id="54550-110">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="54550-111">code</span><span class="sxs-lookup"><span data-stu-id="54550-111">code</span></span>     | <span data-ttu-id="54550-112">Int32</span><span class="sxs-lookup"><span data-stu-id="54550-112">Int32</span></span> | <span data-ttu-id="54550-113">Код результата.</span><span class="sxs-lookup"><span data-stu-id="54550-113">The result code.</span></span>     |
| <span data-ttu-id="54550-114">message</span><span class="sxs-lookup"><span data-stu-id="54550-114">message</span></span>  | <span data-ttu-id="54550-115">String</span><span class="sxs-lookup"><span data-stu-id="54550-115">String</span></span> | <span data-ttu-id="54550-116">Сообщение.</span><span class="sxs-lookup"><span data-stu-id="54550-116">The message.</span></span>         |
| <span data-ttu-id="54550-117">Subcode</span><span class="sxs-lookup"><span data-stu-id="54550-117">subcode</span></span>  | <span data-ttu-id="54550-118">Int32</span><span class="sxs-lookup"><span data-stu-id="54550-118">Int32</span></span> | <span data-ttu-id="54550-119">Дочерний код результата.</span><span class="sxs-lookup"><span data-stu-id="54550-119">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="54550-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54550-120">JSON representation</span></span>

<span data-ttu-id="54550-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54550-121">The following is a JSON representation of the resource.</span></span>

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
