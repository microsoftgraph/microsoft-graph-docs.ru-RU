---
title: Тип ресурса Ресултинфо
description: Тип Ресултинфо.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 0c924798715448e87c30cf2b65cc923c6ddc20bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562995"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="7ef88-103">Тип ресурса Ресултинфо</span><span class="sxs-lookup"><span data-stu-id="7ef88-103">resultInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ef88-104">Тип Ресултинфо.</span><span class="sxs-lookup"><span data-stu-id="7ef88-104">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="7ef88-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ef88-105">Properties</span></span>

| <span data-ttu-id="7ef88-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ef88-106">Property</span></span> | <span data-ttu-id="7ef88-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7ef88-107">Type</span></span>   | <span data-ttu-id="7ef88-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7ef88-108">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="7ef88-109">code</span><span class="sxs-lookup"><span data-stu-id="7ef88-109">code</span></span>     | <span data-ttu-id="7ef88-110">String</span><span class="sxs-lookup"><span data-stu-id="7ef88-110">String</span></span> | <span data-ttu-id="7ef88-111">Код результата.</span><span class="sxs-lookup"><span data-stu-id="7ef88-111">The result code.</span></span>     |
| <span data-ttu-id="7ef88-112">message</span><span class="sxs-lookup"><span data-stu-id="7ef88-112">message</span></span>  | <span data-ttu-id="7ef88-113">String</span><span class="sxs-lookup"><span data-stu-id="7ef88-113">String</span></span> | <span data-ttu-id="7ef88-114">Сообщение.</span><span class="sxs-lookup"><span data-stu-id="7ef88-114">The message.</span></span>         |
| <span data-ttu-id="7ef88-115">subCode</span><span class="sxs-lookup"><span data-stu-id="7ef88-115">subCode</span></span>  | <span data-ttu-id="7ef88-116">String</span><span class="sxs-lookup"><span data-stu-id="7ef88-116">String</span></span> | <span data-ttu-id="7ef88-117">Дочерний код результата.</span><span class="sxs-lookup"><span data-stu-id="7ef88-117">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7ef88-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ef88-118">JSON representation</span></span>

<span data-ttu-id="7ef88-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ef88-119">The following is a JSON representation of the resource.</span></span>

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

## <a name="example-error-result"></a><span data-ttu-id="7ef88-120">Пример результата ошибки</span><span class="sxs-lookup"><span data-stu-id="7ef88-120">Example Error result</span></span>

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

## <a name="example-generic-success-result"></a><span data-ttu-id="7ef88-121">Пример общего результата успеха</span><span class="sxs-lookup"><span data-stu-id="7ef88-121">Example Generic success result</span></span>

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

## <a name="example-record-success-result"></a><span data-ttu-id="7ef88-122">Пример результатов записи</span><span class="sxs-lookup"><span data-stu-id="7ef88-122">Example Record Success result</span></span>

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
