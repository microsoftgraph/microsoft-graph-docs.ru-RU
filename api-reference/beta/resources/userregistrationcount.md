---
title: Тип ресурса Усеррегистратионкаунт
description: Представляет счетчик регистраций и состояние для пользователей в клиенте.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 5aa86a0b490ddb2cd68a504f5a4879f922fa0cf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057829"
---
# <a name="userregistrationcount-resource-type"></a><span data-ttu-id="cc30f-103">Тип ресурса Усеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="cc30f-103">userRegistrationCount resource type</span></span>

<span data-ttu-id="cc30f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc30f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc30f-105">Представляет счетчик регистраций и состояние для пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="cc30f-105">Represents the registration count and status for users in your tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="cc30f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc30f-106">Properties</span></span>

| <span data-ttu-id="cc30f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc30f-107">Property</span></span>     | <span data-ttu-id="cc30f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cc30f-108">Type</span></span>        | <span data-ttu-id="cc30f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cc30f-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cc30f-110">регистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="cc30f-110">registrationCount</span></span> | <span data-ttu-id="cc30f-111">Int64</span><span class="sxs-lookup"><span data-stu-id="cc30f-111">Int64</span></span> | <span data-ttu-id="cc30f-112">Предоставляет счетчик регистраций для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc30f-112">Provides the registration count for your tenant.</span></span> |
| <span data-ttu-id="cc30f-113">регистратионстатус</span><span class="sxs-lookup"><span data-stu-id="cc30f-113">registrationStatus</span></span> | <span data-ttu-id="cc30f-114">String</span><span class="sxs-lookup"><span data-stu-id="cc30f-114">String</span></span> | <span data-ttu-id="cc30f-115">Представляет состояние регистрации пользователя.</span><span class="sxs-lookup"><span data-stu-id="cc30f-115">Represents the status of user registration.</span></span> <span data-ttu-id="cc30f-116">Возможные значения: `registered` , `enabled` , `capable` и `mfaRegistered` .</span><span class="sxs-lookup"><span data-stu-id="cc30f-116">Possible values are: `registered`, `enabled`, `capable`, and `mfaRegistered`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cc30f-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cc30f-117">JSON representation</span></span>

<span data-ttu-id="cc30f-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc30f-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userRegistrationCount",
  "baseType": null
}-->

```json
{ 
  "registrationStatus":"String", 
  "registrationCount": 23423
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

