---
title: Тип ресурса Сигнинстатус
description: Предоставляет состояние входа (успешный или неудачный) входа
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: SarahBar
ms.openlocfilehash: 339041f4fa332efdf949ed5d3c4cad1ad6fdcf2c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067116"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="e89a6-103">Тип ресурса Сигнинстатус</span><span class="sxs-lookup"><span data-stu-id="e89a6-103">signInStatus resource type</span></span>

<span data-ttu-id="e89a6-104">Пространство имен: Microsoft. Graph предоставляет состояние входа (успешную или неудачную) входа</span><span class="sxs-lookup"><span data-stu-id="e89a6-104">Namespace: microsoft.graph Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="e89a6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e89a6-105">Properties</span></span>
| <span data-ttu-id="e89a6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e89a6-106">Property</span></span>     | <span data-ttu-id="e89a6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e89a6-107">Type</span></span>   |<span data-ttu-id="e89a6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e89a6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e89a6-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="e89a6-109">additionalDetails</span></span>|<span data-ttu-id="e89a6-110">String</span><span class="sxs-lookup"><span data-stu-id="e89a6-110">String</span></span>|<span data-ttu-id="e89a6-111">Предоставляет дополнительные сведения об активности входа</span><span class="sxs-lookup"><span data-stu-id="e89a6-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="e89a6-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="e89a6-112">errorCode</span></span>|<span data-ttu-id="e89a6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e89a6-113">Int32</span></span>|<span data-ttu-id="e89a6-114">Предоставляет код ошибки 5 6digit, который создается при сбое входа.</span><span class="sxs-lookup"><span data-stu-id="e89a6-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="e89a6-115">Ознакомьтесь со [списком кодов и сообщений об ошибках](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="e89a6-115">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="e89a6-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="e89a6-116">failureReason</span></span>|<span data-ttu-id="e89a6-117">String</span><span class="sxs-lookup"><span data-stu-id="e89a6-117">String</span></span>|<span data-ttu-id="e89a6-118">Содержит сообщение об ошибке или причину сбоя для соответствующего действия при входе.</span><span class="sxs-lookup"><span data-stu-id="e89a6-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="e89a6-119">Ознакомьтесь со [списком кодов и сообщений об ошибках](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="e89a6-119">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e89a6-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e89a6-120">JSON representation</span></span>

<span data-ttu-id="e89a6-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e89a6-121">Here is a JSON representation of the resource.</span></span>

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


