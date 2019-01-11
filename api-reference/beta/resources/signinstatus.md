---
title: Тип ресурса signInStatus
description: Предоставляет входа в состояние (успешное или неудачное) входа в программу
localization_priority: Normal
ms.openlocfilehash: 96bcee62bac24701254f56bee41422ca91501d9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878640"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="408e7-103">Тип ресурса signInStatus</span><span class="sxs-lookup"><span data-stu-id="408e7-103">signInStatus resource type</span></span>
<span data-ttu-id="408e7-104">Предоставляет входа в состояние (успешное или неудачное) входа в программу</span><span class="sxs-lookup"><span data-stu-id="408e7-104">Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="408e7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="408e7-105">Properties</span></span>
| <span data-ttu-id="408e7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="408e7-106">Property</span></span>     | <span data-ttu-id="408e7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="408e7-107">Type</span></span>   |<span data-ttu-id="408e7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="408e7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="408e7-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="408e7-109">additionalDetails</span></span>|<span data-ttu-id="408e7-110">Строка</span><span class="sxs-lookup"><span data-stu-id="408e7-110">String</span></span>|<span data-ttu-id="408e7-111">Дополнительные сведения для входа в действия</span><span class="sxs-lookup"><span data-stu-id="408e7-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="408e7-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="408e7-112">errorCode</span></span>|<span data-ttu-id="408e7-113">Int32</span><span class="sxs-lookup"><span data-stu-id="408e7-113">Int32</span></span>|<span data-ttu-id="408e7-114">Содержит код ошибки 5 6digit, созданного во время сбоя входа.</span><span class="sxs-lookup"><span data-stu-id="408e7-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="408e7-115">Извлечение [списка кодов ошибок и сообщений](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="408e7-115">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="408e7-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="408e7-116">failureReason</span></span>|<span data-ttu-id="408e7-117">String</span><span class="sxs-lookup"><span data-stu-id="408e7-117">String</span></span>|<span data-ttu-id="408e7-118">Содержит сообщение об ошибке или причину сбоя для соответствующей операции регистрации.</span><span class="sxs-lookup"><span data-stu-id="408e7-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="408e7-119">Извлечение [списка кодов ошибок и сообщений](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="408e7-119">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="408e7-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="408e7-120">JSON representation</span></span>

<span data-ttu-id="408e7-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="408e7-121">Here is a JSON representation of the resource.</span></span>

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
