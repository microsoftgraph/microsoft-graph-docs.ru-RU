---
title: Тип ресурса signInStatus
description: Предоставляет состояние (успешное или неудачное) для этого.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: SarahBar
ms.openlocfilehash: d7428c2a73d0b4a114599dad8ac1740d91ba5865
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132638"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="04466-103">Тип ресурса signInStatus</span><span class="sxs-lookup"><span data-stu-id="04466-103">signInStatus resource type</span></span>

<span data-ttu-id="04466-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04466-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04466-105">Предоставляет состояние (успешное или неудачное) для этого.</span><span class="sxs-lookup"><span data-stu-id="04466-105">Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="04466-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="04466-106">Properties</span></span>
| <span data-ttu-id="04466-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="04466-107">Property</span></span>     | <span data-ttu-id="04466-108">Тип</span><span class="sxs-lookup"><span data-stu-id="04466-108">Type</span></span>   |<span data-ttu-id="04466-109">Описание</span><span class="sxs-lookup"><span data-stu-id="04466-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04466-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="04466-110">additionalDetails</span></span>|<span data-ttu-id="04466-111">Строка</span><span class="sxs-lookup"><span data-stu-id="04466-111">String</span></span>|<span data-ttu-id="04466-112">Предоставляет дополнительные сведения об активности при входе</span><span class="sxs-lookup"><span data-stu-id="04466-112">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="04466-113">errorCode</span><span class="sxs-lookup"><span data-stu-id="04466-113">errorCode</span></span>|<span data-ttu-id="04466-114">Int32</span><span class="sxs-lookup"><span data-stu-id="04466-114">Int32</span></span>|<span data-ttu-id="04466-115">Предоставляет код ошибки из 5–6 цифр, который создается при сбое при входе.</span><span class="sxs-lookup"><span data-stu-id="04466-115">Provides the 5-6 digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="04466-116">Ознакомьтесь [со списком кодов ошибок и сообщений.](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)</span><span class="sxs-lookup"><span data-stu-id="04466-116">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="04466-117">failureReason</span><span class="sxs-lookup"><span data-stu-id="04466-117">failureReason</span></span>|<span data-ttu-id="04466-118">String</span><span class="sxs-lookup"><span data-stu-id="04466-118">String</span></span>|<span data-ttu-id="04466-119">Предоставляет сообщение об ошибке или причину сбоя для соответствующего действия при входе.</span><span class="sxs-lookup"><span data-stu-id="04466-119">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="04466-120">Ознакомьтесь [со списком кодов ошибок и сообщений.](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)</span><span class="sxs-lookup"><span data-stu-id="04466-120">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04466-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="04466-121">JSON representation</span></span>

<span data-ttu-id="04466-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04466-122">Here is a JSON representation of the resource.</span></span>

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


