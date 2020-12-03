---
title: Тип ресурса Кредентиалусеррегистратионкаунт
description: Представляет текущее состояние количества пользователей в вашей организации, зарегистрированных для самостоятельного сброса паролей и возможности многофакторной проверки подлинности.
localization_priority: Normal
author: besiler
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 59c7849a5145064eafbce63804b5d3415fb92b97
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523135"
---
# <a name="credentialuserregistrationcount-resource-type"></a><span data-ttu-id="27020-103">Тип ресурса Кредентиалусеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="27020-103">credentialUserRegistrationCount resource type</span></span>

<span data-ttu-id="27020-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27020-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27020-105">Представляет текущее состояние количества пользователей в вашей организации, зарегистрированных для самостоятельного сброса паролей и возможности многофакторной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="27020-105">Represents the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="27020-106">Методы</span><span class="sxs-lookup"><span data-stu-id="27020-106">Methods</span></span>

| <span data-ttu-id="27020-107">Метод</span><span class="sxs-lookup"><span data-stu-id="27020-107">Method</span></span>       | <span data-ttu-id="27020-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="27020-108">Return Type</span></span> | <span data-ttu-id="27020-109">Описание</span><span class="sxs-lookup"><span data-stu-id="27020-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="27020-110">жеткредентиалусеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="27020-110">getCredentialUserRegistrationCount</span></span>](../api/reportroot-getcredentialuserregistrationcount.md) | <span data-ttu-id="27020-111">Коллекция Кредентиалусеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="27020-111">credentialUserRegistrationCount collection</span></span> | <span data-ttu-id="27020-112">Сообщите о текущем состоянии того, сколько пользователей в вашей организации зарегистрировано для самостоятельного сброса паролей и возможностей многофакторной проверки подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="27020-112">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span> |

## <a name="properties"></a><span data-ttu-id="27020-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="27020-113">Properties</span></span>

| <span data-ttu-id="27020-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="27020-114">Property</span></span>     | <span data-ttu-id="27020-115">Тип</span><span class="sxs-lookup"><span data-stu-id="27020-115">Type</span></span>        | <span data-ttu-id="27020-116">Описание</span><span class="sxs-lookup"><span data-stu-id="27020-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="27020-117">id</span><span class="sxs-lookup"><span data-stu-id="27020-117">id</span></span> | <span data-ttu-id="27020-118">String</span><span class="sxs-lookup"><span data-stu-id="27020-118">String</span></span> | <span data-ttu-id="27020-119">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="27020-119">The unique identifier for the activity.</span></span> <span data-ttu-id="27020-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27020-120">Read-only.</span></span> |
| <span data-ttu-id="27020-121">тоталусеркаунт</span><span class="sxs-lookup"><span data-stu-id="27020-121">totalUserCount</span></span> | <span data-ttu-id="27020-122">Int64</span><span class="sxs-lookup"><span data-stu-id="27020-122">Int64</span></span> | <span data-ttu-id="27020-123">Предоставляет общее число пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="27020-123">Provides the total user count in the tenant.</span></span> |
| <span data-ttu-id="27020-124">усеррегистратионкаунтс</span><span class="sxs-lookup"><span data-stu-id="27020-124">userRegistrationCounts</span></span> | <span data-ttu-id="27020-125">Коллекция [усеррегистратионкаунт](userregistrationcount.md)</span><span class="sxs-lookup"><span data-stu-id="27020-125">[userRegistrationCount](userregistrationcount.md) collection</span></span> | <span data-ttu-id="27020-126">Коллекция счетчиков регистрации и сведений о состоянии для пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="27020-126">A collection of registration count and status information for users in your tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="27020-127">Связи</span><span class="sxs-lookup"><span data-stu-id="27020-127">Relationships</span></span>

<span data-ttu-id="27020-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="27020-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="27020-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="27020-129">JSON representation</span></span>

<span data-ttu-id="27020-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27020-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "totalUserCount" : 23123,
  "userRegistrationCounts" :
  [
    { "registrationStatus":"registered", "registrationCount": 23423 },
    { "registrationStatus":"enabled", "registrationCount": 4234 },
    { "registrationStatus":"capable", "registrationCount": 323 },
    { "registrationStatus":"mfaRegistered", "registrationCount": 33 }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationCount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

