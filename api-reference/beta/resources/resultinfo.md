---
title: Тип ресурса resultInfo
description: Тип resultInfo.
author: VinodRavichandran
ms.openlocfilehash: db208ed214213ec906dac18b65140f010014fc6c
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380410"
---
# <a name="resultinfo-resource-type"></a><span data-ttu-id="86013-103">Тип ресурса resultInfo</span><span class="sxs-lookup"><span data-stu-id="86013-103">resultInfo resource type</span></span>

> <span data-ttu-id="86013-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="86013-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86013-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86013-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="86013-106">Тип resultInfo.</span><span class="sxs-lookup"><span data-stu-id="86013-106">The resultInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="86013-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="86013-107">Properties</span></span>

| <span data-ttu-id="86013-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="86013-108">Property</span></span> | <span data-ttu-id="86013-109">Тип</span><span class="sxs-lookup"><span data-stu-id="86013-109">Type</span></span>   | <span data-ttu-id="86013-110">Описание</span><span class="sxs-lookup"><span data-stu-id="86013-110">Description</span></span>          |
| :------- | :----- | :------------------  |
| <span data-ttu-id="86013-111">code</span><span class="sxs-lookup"><span data-stu-id="86013-111">code</span></span>     | <span data-ttu-id="86013-112">String</span><span class="sxs-lookup"><span data-stu-id="86013-112">String</span></span> | <span data-ttu-id="86013-113">Код результата.</span><span class="sxs-lookup"><span data-stu-id="86013-113">The result code.</span></span>     |
| <span data-ttu-id="86013-114">message</span><span class="sxs-lookup"><span data-stu-id="86013-114">message</span></span>  | <span data-ttu-id="86013-115">String</span><span class="sxs-lookup"><span data-stu-id="86013-115">String</span></span> | <span data-ttu-id="86013-116">Сообщение.</span><span class="sxs-lookup"><span data-stu-id="86013-116">The message.</span></span>         |
| <span data-ttu-id="86013-117">дополнительный код</span><span class="sxs-lookup"><span data-stu-id="86013-117">subCode</span></span>  | <span data-ttu-id="86013-118">String</span><span class="sxs-lookup"><span data-stu-id="86013-118">String</span></span> | <span data-ttu-id="86013-119">Вложенный код результата.</span><span class="sxs-lookup"><span data-stu-id="86013-119">The result sub-code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="86013-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86013-120">JSON representation</span></span>

<span data-ttu-id="86013-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86013-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example-error-result"></a><span data-ttu-id="86013-122">Пример результат ошибки</span><span class="sxs-lookup"><span data-stu-id="86013-122">Example Error result</span></span>

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

## <a name="example-generic-success-result"></a><span data-ttu-id="86013-123">Пример универсального успеха результатов</span><span class="sxs-lookup"><span data-stu-id="86013-123">Example Generic success result</span></span>

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

## <a name="example-record-success-result"></a><span data-ttu-id="86013-124">Пример записи успеха результатов</span><span class="sxs-lookup"><span data-stu-id="86013-124">Example Record Success result</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "resultInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
