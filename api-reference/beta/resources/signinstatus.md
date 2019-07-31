---
title: Тип ресурса Сигнинстатус
description: Предоставляет состояние входа (успешный или неудачный) входа
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d336e226b2855687da0aae889afd9d92141c895c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008308"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="6d79c-103">Тип ресурса Сигнинстатус</span><span class="sxs-lookup"><span data-stu-id="6d79c-103">signInStatus resource type</span></span>
<span data-ttu-id="6d79c-104">Предоставляет состояние входа (успешный или неудачный) входа</span><span class="sxs-lookup"><span data-stu-id="6d79c-104">Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="6d79c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d79c-105">Properties</span></span>
| <span data-ttu-id="6d79c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d79c-106">Property</span></span>     | <span data-ttu-id="6d79c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6d79c-107">Type</span></span>   |<span data-ttu-id="6d79c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6d79c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d79c-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="6d79c-109">additionalDetails</span></span>|<span data-ttu-id="6d79c-110">String</span><span class="sxs-lookup"><span data-stu-id="6d79c-110">String</span></span>|<span data-ttu-id="6d79c-111">Предоставляет дополнительные сведения об активности входа</span><span class="sxs-lookup"><span data-stu-id="6d79c-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="6d79c-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="6d79c-112">errorCode</span></span>|<span data-ttu-id="6d79c-113">Int32</span><span class="sxs-lookup"><span data-stu-id="6d79c-113">Int32</span></span>|<span data-ttu-id="6d79c-114">Предоставляет код ошибки 5 6digit, который создается при сбое входа.</span><span class="sxs-lookup"><span data-stu-id="6d79c-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="6d79c-115">Ознакомьтесь со [списком кодов и сообщений об ошибках](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="6d79c-115">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="6d79c-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="6d79c-116">failureReason</span></span>|<span data-ttu-id="6d79c-117">String</span><span class="sxs-lookup"><span data-stu-id="6d79c-117">String</span></span>|<span data-ttu-id="6d79c-118">Содержит сообщение об ошибке или причину сбоя для соответствующего действия при входе.</span><span class="sxs-lookup"><span data-stu-id="6d79c-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="6d79c-119">Ознакомьтесь со [списком кодов и сообщений об ошибках](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="6d79c-119">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d79c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d79c-120">JSON representation</span></span>

<span data-ttu-id="6d79c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d79c-121">Here is a JSON representation of the resource.</span></span>

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
