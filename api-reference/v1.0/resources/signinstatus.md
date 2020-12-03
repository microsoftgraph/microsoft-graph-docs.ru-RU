---
title: Тип ресурса Сигнинстатус
description: Предоставляет состояние входа (успешный или неудачный) входа
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3633968869c0cf61e16afa4ba056a530c86b3c93
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563655"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="ef9a0-103">Тип ресурса Сигнинстатус</span><span class="sxs-lookup"><span data-stu-id="ef9a0-103">signInStatus resource type</span></span>

<span data-ttu-id="ef9a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef9a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ef9a0-105">Предоставляет состояние входа (успешный или неудачный) входа.</span><span class="sxs-lookup"><span data-stu-id="ef9a0-105">Provides the sign-in status (Success or Failure) of the sign-in.</span></span>

## <a name="properties"></a><span data-ttu-id="ef9a0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef9a0-106">Properties</span></span>

| <span data-ttu-id="ef9a0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef9a0-107">Property</span></span>     | <span data-ttu-id="ef9a0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ef9a0-108">Type</span></span>   |<span data-ttu-id="ef9a0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ef9a0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef9a0-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="ef9a0-110">additionalDetails</span></span>|<span data-ttu-id="ef9a0-111">String</span><span class="sxs-lookup"><span data-stu-id="ef9a0-111">String</span></span>|<span data-ttu-id="ef9a0-112">Предоставляет дополнительные сведения об активности входа</span><span class="sxs-lookup"><span data-stu-id="ef9a0-112">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="ef9a0-113">errorCode</span><span class="sxs-lookup"><span data-stu-id="ef9a0-113">errorCode</span></span>|<span data-ttu-id="ef9a0-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ef9a0-114">Int32</span></span>|<span data-ttu-id="ef9a0-115">Предоставляет код ошибки 5-6, который создается при сбое входа.</span><span class="sxs-lookup"><span data-stu-id="ef9a0-115">Provides the 5-6 digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="ef9a0-116">Ознакомьтесь со [списком кодов и сообщений об ошибках](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="ef9a0-116">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="ef9a0-117">failureReason</span><span class="sxs-lookup"><span data-stu-id="ef9a0-117">failureReason</span></span>|<span data-ttu-id="ef9a0-118">String</span><span class="sxs-lookup"><span data-stu-id="ef9a0-118">String</span></span>|<span data-ttu-id="ef9a0-119">Содержит сообщение об ошибке или причину сбоя для соответствующего действия при входе.</span><span class="sxs-lookup"><span data-stu-id="ef9a0-119">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="ef9a0-120">Ознакомьтесь со [списком кодов и сообщений об ошибках](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span><span class="sxs-lookup"><span data-stu-id="ef9a0-120">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef9a0-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef9a0-121">JSON representation</span></span>

<span data-ttu-id="ef9a0-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef9a0-122">Here is a JSON representation of the resource.</span></span>

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

