---
title: Тип ресурса signInStatus
description: Предоставляет входа в состояние (успешное или неудачное) входа в программу
ms.openlocfilehash: cafa0dffe1b1d798d87225ac82901cf041d5e4fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081655"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="9d8f1-103">Тип ресурса signInStatus</span><span class="sxs-lookup"><span data-stu-id="9d8f1-103">signInStatus resource type</span></span>
<span data-ttu-id="9d8f1-104">Предоставляет входа в состояние (успешное или неудачное) входа в программу</span><span class="sxs-lookup"><span data-stu-id="9d8f1-104">Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="9d8f1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d8f1-105">Properties</span></span>
| <span data-ttu-id="9d8f1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d8f1-106">Property</span></span>     | <span data-ttu-id="9d8f1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9d8f1-107">Type</span></span>   |<span data-ttu-id="9d8f1-108">Description</span><span class="sxs-lookup"><span data-stu-id="9d8f1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d8f1-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="9d8f1-109">additionalDetails</span></span>|<span data-ttu-id="9d8f1-110">String</span><span class="sxs-lookup"><span data-stu-id="9d8f1-110">String</span></span>|<span data-ttu-id="9d8f1-111">Дополнительные сведения для входа в действия</span><span class="sxs-lookup"><span data-stu-id="9d8f1-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="9d8f1-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="9d8f1-112">errorCode</span></span>|<span data-ttu-id="9d8f1-113">Int32</span><span class="sxs-lookup"><span data-stu-id="9d8f1-113">Int32</span></span>|<span data-ttu-id="9d8f1-114">Содержит код ошибки 5 6digit, созданного во время сбоя входа.</span><span class="sxs-lookup"><span data-stu-id="9d8f1-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="9d8f1-115">Извлечение [списка кодов ошибок и сообщений](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="9d8f1-115">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="9d8f1-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="9d8f1-116">failureReason</span></span>|<span data-ttu-id="9d8f1-117">String</span><span class="sxs-lookup"><span data-stu-id="9d8f1-117">String</span></span>|<span data-ttu-id="9d8f1-118">Содержит сообщение об ошибке или причину сбоя для соответствующей операции регистрации.</span><span class="sxs-lookup"><span data-stu-id="9d8f1-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="9d8f1-119">Извлечение [списка кодов ошибок и сообщений](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="9d8f1-119">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d8f1-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d8f1-120">JSON representation</span></span>

<span data-ttu-id="9d8f1-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d8f1-121">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInStatus"
}-->

```json
{
  "additionalDetails": "String",
  "errorCode": 1024,
  "failureReason": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->