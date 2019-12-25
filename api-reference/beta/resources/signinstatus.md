---
title: Тип ресурса Сигнинстатус
description: Предоставляет состояние входа (успешный или неудачный) входа
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0f86c7026fc487e48388bd3d20e973e7a0cf7e41
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866611"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="f6bd1-103">Тип ресурса Сигнинстатус</span><span class="sxs-lookup"><span data-stu-id="f6bd1-103">signInStatus resource type</span></span>
<span data-ttu-id="f6bd1-104">Предоставляет состояние входа (успешный или неудачный) входа</span><span class="sxs-lookup"><span data-stu-id="f6bd1-104">Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="f6bd1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6bd1-105">Properties</span></span>
| <span data-ttu-id="f6bd1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6bd1-106">Property</span></span>     | <span data-ttu-id="f6bd1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f6bd1-107">Type</span></span>   |<span data-ttu-id="f6bd1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f6bd1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6bd1-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="f6bd1-109">additionalDetails</span></span>|<span data-ttu-id="f6bd1-110">String</span><span class="sxs-lookup"><span data-stu-id="f6bd1-110">String</span></span>|<span data-ttu-id="f6bd1-111">Предоставляет дополнительные сведения об активности входа</span><span class="sxs-lookup"><span data-stu-id="f6bd1-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="f6bd1-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="f6bd1-112">errorCode</span></span>|<span data-ttu-id="f6bd1-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f6bd1-113">Int32</span></span>|<span data-ttu-id="f6bd1-114">Предоставляет код ошибки 5 6digit, который создается при сбое входа.</span><span class="sxs-lookup"><span data-stu-id="f6bd1-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="f6bd1-115">Ознакомьтесь со [списком кодов и сообщений об ошибках](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="f6bd1-115">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="f6bd1-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="f6bd1-116">failureReason</span></span>|<span data-ttu-id="f6bd1-117">String</span><span class="sxs-lookup"><span data-stu-id="f6bd1-117">String</span></span>|<span data-ttu-id="f6bd1-118">Содержит сообщение об ошибке или причину сбоя для соответствующего действия при входе.</span><span class="sxs-lookup"><span data-stu-id="f6bd1-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="f6bd1-119">Ознакомьтесь со [списком кодов и сообщений об ошибках](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="f6bd1-119">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6bd1-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6bd1-120">JSON representation</span></span>

<span data-ttu-id="f6bd1-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6bd1-121">Here is a JSON representation of the resource.</span></span>

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
