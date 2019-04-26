---
title: Тип ресурса Ресултинфо
description: Тип Ресултинфо.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 2406c29c12af81ee6981b8ffa59e630a5451c2fc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343552"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="a9659-103">Тип ресурса Ресултинфо</span><span class="sxs-lookup"><span data-stu-id="a9659-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9659-104">Тип Ресултинфо.</span><span class="sxs-lookup"><span data-stu-id="a9659-104">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="a9659-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9659-105">Properties</span></span>

| <span data-ttu-id="a9659-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9659-106">Property</span></span> | <span data-ttu-id="a9659-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a9659-107">Type</span></span>   | <span data-ttu-id="a9659-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a9659-108">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="a9659-109">code</span><span class="sxs-lookup"><span data-stu-id="a9659-109">code</span></span>     | <span data-ttu-id="a9659-110">String</span><span class="sxs-lookup"><span data-stu-id="a9659-110">String</span></span> | <span data-ttu-id="a9659-111">Код результата.</span><span class="sxs-lookup"><span data-stu-id="a9659-111">The result code.</span></span>     |
| <span data-ttu-id="a9659-112">message</span><span class="sxs-lookup"><span data-stu-id="a9659-112">message</span></span>  | <span data-ttu-id="a9659-113">String</span><span class="sxs-lookup"><span data-stu-id="a9659-113">String</span></span> | <span data-ttu-id="a9659-114">Сообщение.</span><span class="sxs-lookup"><span data-stu-id="a9659-114">The message.</span></span>         |
| <span data-ttu-id="a9659-115">subCode</span><span class="sxs-lookup"><span data-stu-id="a9659-115">subCode</span></span>  | <span data-ttu-id="a9659-116">String</span><span class="sxs-lookup"><span data-stu-id="a9659-116">String</span></span> | <span data-ttu-id="a9659-117">Дочерний код результата.</span><span class="sxs-lookup"><span data-stu-id="a9659-117">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a9659-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9659-118">JSON representation</span></span>

<span data-ttu-id="a9659-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9659-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "String",
  "message": "String",
  "subCode": "String"
}
```

## <a name="example-error-result"></a><span data-ttu-id="a9659-120">Пример результата ошибки</span><span class="sxs-lookup"><span data-stu-id="a9659-120">Example Error result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "100",
  "message": "Internal Server Error.",
  "subCode": "20"
}
```

## <a name="example-generic-success-result"></a><span data-ttu-id="a9659-121">Пример общего результата успеха</span><span class="sxs-lookup"><span data-stu-id="a9659-121">Example Generic success result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "0"
}
```

## <a name="example-record-success-result"></a><span data-ttu-id="a9659-122">Пример результатов записи</span><span class="sxs-lookup"><span data-stu-id="a9659-122">Example Record Success result</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.resultInfo"
}-->
```json
{
  "code": "200",
  "message": "",
  "subCode": "completedSilenceDetected"
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
