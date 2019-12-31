---
title: Тип ресурса Ресултинфо
description: Содержит сведения о результатах, относящиеся к успехам и сбоям.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 43a7dba5d758f8884285e7238e4e4fab0763409f
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913725"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="f9042-103">Тип ресурса Ресултинфо</span><span class="sxs-lookup"><span data-stu-id="f9042-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9042-104">Содержит сведения о результатах, относящиеся к успехам и сбоям.</span><span class="sxs-lookup"><span data-stu-id="f9042-104">Contains success and failure-specific result information.</span></span> 

<span data-ttu-id="f9042-105">Код указывает, является ли результат универсальным успехом или ошибкой.</span><span class="sxs-lookup"><span data-stu-id="f9042-105">The code specifies whether the result is a generic success or failure.</span></span> 

<span data-ttu-id="f9042-106">Вспомогательные коды предоставляют дополнительные сведения, связанные с типом успешного или неудачного завершения (например, успешная передача вызова).</span><span class="sxs-lookup"><span data-stu-id="f9042-106">The subcodes provide supplementary information related to the type of success or failure (for example, a call transfer was successful).</span></span>


## <a name="properties"></a><span data-ttu-id="f9042-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9042-107">Properties</span></span>

| <span data-ttu-id="f9042-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9042-108">Property</span></span> | <span data-ttu-id="f9042-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f9042-109">Type</span></span>   | <span data-ttu-id="f9042-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f9042-110">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="f9042-111">code</span><span class="sxs-lookup"><span data-stu-id="f9042-111">code</span></span>     | <span data-ttu-id="f9042-112">Int32</span><span class="sxs-lookup"><span data-stu-id="f9042-112">Int32</span></span> | <span data-ttu-id="f9042-113">Код результата.</span><span class="sxs-lookup"><span data-stu-id="f9042-113">The result code.</span></span>     |
| <span data-ttu-id="f9042-114">message</span><span class="sxs-lookup"><span data-stu-id="f9042-114">message</span></span>  | <span data-ttu-id="f9042-115">String</span><span class="sxs-lookup"><span data-stu-id="f9042-115">String</span></span> | <span data-ttu-id="f9042-116">Сообщение.</span><span class="sxs-lookup"><span data-stu-id="f9042-116">The message.</span></span>         |
| <span data-ttu-id="f9042-117">Subcode</span><span class="sxs-lookup"><span data-stu-id="f9042-117">subcode</span></span>  | <span data-ttu-id="f9042-118">Int32</span><span class="sxs-lookup"><span data-stu-id="f9042-118">Int32</span></span> | <span data-ttu-id="f9042-119">Дочерний код результата.</span><span class="sxs-lookup"><span data-stu-id="f9042-119">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f9042-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9042-120">JSON representation</span></span>

<span data-ttu-id="f9042-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9042-121">The following is a JSON representation of the resource.</span></span>

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
