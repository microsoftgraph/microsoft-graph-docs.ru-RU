---
title: Тип ресурса Кредентиалусеррегистратионкаунт
description: Представляет текущее состояние количества пользователей в вашей организации, зарегистрированных для самостоятельного сброса паролей и возможности многофакторной проверки подлинности.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 42c722b04493767d3dbcaf713157d931569d8c32
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487607"
---
# <a name="credentialuserregistrationcount-resource-type"></a><span data-ttu-id="85a71-103">Тип ресурса Кредентиалусеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="85a71-103">credentialUserRegistrationCount resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85a71-104">Представляет текущее состояние количества пользователей в вашей организации, зарегистрированных для самостоятельного сброса паролей и возможности многофакторной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="85a71-104">Represents the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="85a71-105">Методы</span><span class="sxs-lookup"><span data-stu-id="85a71-105">Methods</span></span>

| <span data-ttu-id="85a71-106">Метод</span><span class="sxs-lookup"><span data-stu-id="85a71-106">Method</span></span>       | <span data-ttu-id="85a71-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="85a71-107">Return Type</span></span> | <span data-ttu-id="85a71-108">Описание</span><span class="sxs-lookup"><span data-stu-id="85a71-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="85a71-109">Жеткредентиалусеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="85a71-109">getCredentialUserRegistrationCount</span></span>](../api/reportroot-getcredentialuserregistrationcount.md) | <span data-ttu-id="85a71-110">Коллекция Кредентиалусеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="85a71-110">credentialUserRegistrationCount collection</span></span> | <span data-ttu-id="85a71-111">Сообщите о текущем состоянии того, сколько пользователей в вашей организации зарегистрировано для самостоятельного сброса паролей и возможностей многофакторной проверки подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="85a71-111">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span> |

## <a name="properties"></a><span data-ttu-id="85a71-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="85a71-112">Properties</span></span>

| <span data-ttu-id="85a71-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="85a71-113">Property</span></span>     | <span data-ttu-id="85a71-114">Тип</span><span class="sxs-lookup"><span data-stu-id="85a71-114">Type</span></span>        | <span data-ttu-id="85a71-115">Описание</span><span class="sxs-lookup"><span data-stu-id="85a71-115">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="85a71-116">id</span><span class="sxs-lookup"><span data-stu-id="85a71-116">id</span></span> | <span data-ttu-id="85a71-117">String</span><span class="sxs-lookup"><span data-stu-id="85a71-117">String</span></span> | <span data-ttu-id="85a71-118">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="85a71-118">The unique identifier for the activity.</span></span> <span data-ttu-id="85a71-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="85a71-119">Read-only.</span></span> |
| <span data-ttu-id="85a71-120">Тоталусеркаунт</span><span class="sxs-lookup"><span data-stu-id="85a71-120">totalUserCount</span></span> | <span data-ttu-id="85a71-121">Int64</span><span class="sxs-lookup"><span data-stu-id="85a71-121">Int64</span></span> | <span data-ttu-id="85a71-122">Предоставляет общее число пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="85a71-122">Provides the total user count in the tenant.</span></span> |
| <span data-ttu-id="85a71-123">Усеррегистратионкаунтс</span><span class="sxs-lookup"><span data-stu-id="85a71-123">userRegistrationCounts</span></span> | <span data-ttu-id="85a71-124">Коллекция [усеррегистратионкаунт](userregistrationcount.md)</span><span class="sxs-lookup"><span data-stu-id="85a71-124">[userRegistrationCount](userregistrationcount.md) collection</span></span> | <span data-ttu-id="85a71-125">Коллекция счетчиков регистрации и сведений о состоянии для пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="85a71-125">A collection of registration count and status information for users in your tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="85a71-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="85a71-126">Relationships</span></span>

<span data-ttu-id="85a71-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="85a71-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85a71-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="85a71-128">JSON representation</span></span>

<span data-ttu-id="85a71-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85a71-129">The following is a JSON representation of the resource.</span></span>

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