---
title: Тип ресурса Сигнинстатус
description: Предоставляет состояние входа (успешный или неудачный) входа
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c534ae4c6d881add405e0cd29d39197ce5e79f1e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086419"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="2a82b-103">Тип ресурса Сигнинстатус</span><span class="sxs-lookup"><span data-stu-id="2a82b-103">signInStatus resource type</span></span>

<span data-ttu-id="2a82b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a82b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a82b-105">Предоставляет состояние входа (успешный или неудачный) входа.</span><span class="sxs-lookup"><span data-stu-id="2a82b-105">Provides the sign-in status (Success or Failure) of the sign-in.</span></span>

## <a name="properties"></a><span data-ttu-id="2a82b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a82b-106">Properties</span></span>

| <span data-ttu-id="2a82b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a82b-107">Property</span></span>     | <span data-ttu-id="2a82b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2a82b-108">Type</span></span>   |<span data-ttu-id="2a82b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2a82b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a82b-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="2a82b-110">additionalDetails</span></span>|<span data-ttu-id="2a82b-111">Строка</span><span class="sxs-lookup"><span data-stu-id="2a82b-111">String</span></span>|<span data-ttu-id="2a82b-112">Предоставляет дополнительные сведения об активности входа</span><span class="sxs-lookup"><span data-stu-id="2a82b-112">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="2a82b-113">errorCode</span><span class="sxs-lookup"><span data-stu-id="2a82b-113">errorCode</span></span>|<span data-ttu-id="2a82b-114">Int32</span><span class="sxs-lookup"><span data-stu-id="2a82b-114">Int32</span></span>|<span data-ttu-id="2a82b-115">Предоставляет код ошибки 5 6digit, который создается при сбое входа.</span><span class="sxs-lookup"><span data-stu-id="2a82b-115">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="2a82b-116">Ознакомьтесь со [списком кодов и сообщений об ошибках](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="2a82b-116">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="2a82b-117">failureReason</span><span class="sxs-lookup"><span data-stu-id="2a82b-117">failureReason</span></span>|<span data-ttu-id="2a82b-118">String</span><span class="sxs-lookup"><span data-stu-id="2a82b-118">String</span></span>|<span data-ttu-id="2a82b-119">Содержит сообщение об ошибке или причину сбоя для соответствующего действия при входе.</span><span class="sxs-lookup"><span data-stu-id="2a82b-119">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="2a82b-120">Ознакомьтесь со [списком кодов и сообщений об ошибках](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="2a82b-120">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a82b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a82b-121">JSON representation</span></span>

<span data-ttu-id="2a82b-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a82b-122">Here is a JSON representation of the resource.</span></span>

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

