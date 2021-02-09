---
title: Тип ресурса credentialUserRegistrationCount
description: Представляет текущее состояние регистрации пользователей в организации для самостоятельного сброса паролей и многофакторной проверки подлинности.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 521c8eca7c3233000bf04f2324e8990fd25c55f6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159922"
---
# <a name="credentialuserregistrationcount-resource-type"></a><span data-ttu-id="32db3-103">Тип ресурса credentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="32db3-103">credentialUserRegistrationCount resource type</span></span>

<span data-ttu-id="32db3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32db3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32db3-105">Представляет текущее состояние регистрации пользователей в организации для самостоятельного сброса паролей и многофакторной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="32db3-105">Represents the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="32db3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="32db3-106">Methods</span></span>

| <span data-ttu-id="32db3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="32db3-107">Method</span></span>       | <span data-ttu-id="32db3-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="32db3-108">Return Type</span></span> | <span data-ttu-id="32db3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="32db3-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="32db3-110">getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="32db3-110">getCredentialUserRegistrationCount</span></span>](../api/reportroot-getcredentialuserregistrationcount.md) | <span data-ttu-id="32db3-111">Коллекция credentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="32db3-111">credentialUserRegistrationCount collection</span></span> | <span data-ttu-id="32db3-112">Фиксируйте текущее состояние регистрации пользователей в организации для самостоятельного сброса паролей и многофакторной проверки подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="32db3-112">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span> |

## <a name="properties"></a><span data-ttu-id="32db3-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="32db3-113">Properties</span></span>

| <span data-ttu-id="32db3-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="32db3-114">Property</span></span>     | <span data-ttu-id="32db3-115">Тип</span><span class="sxs-lookup"><span data-stu-id="32db3-115">Type</span></span>        | <span data-ttu-id="32db3-116">Описание</span><span class="sxs-lookup"><span data-stu-id="32db3-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="32db3-117">id</span><span class="sxs-lookup"><span data-stu-id="32db3-117">id</span></span> | <span data-ttu-id="32db3-118">String</span><span class="sxs-lookup"><span data-stu-id="32db3-118">String</span></span> | <span data-ttu-id="32db3-119">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="32db3-119">The unique identifier for the activity.</span></span> <span data-ttu-id="32db3-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="32db3-120">Read-only.</span></span> |
| <span data-ttu-id="32db3-121">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="32db3-121">totalUserCount</span></span> | <span data-ttu-id="32db3-122">Int64</span><span class="sxs-lookup"><span data-stu-id="32db3-122">Int64</span></span> | <span data-ttu-id="32db3-123">Предоставляет общее количество пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="32db3-123">Provides the total user count in the tenant.</span></span> |
| <span data-ttu-id="32db3-124">userRegistrationCounts</span><span class="sxs-lookup"><span data-stu-id="32db3-124">userRegistrationCounts</span></span> | <span data-ttu-id="32db3-125">[Коллекция userRegistrationCount](userregistrationcount.md)</span><span class="sxs-lookup"><span data-stu-id="32db3-125">[userRegistrationCount](userregistrationcount.md) collection</span></span> | <span data-ttu-id="32db3-126">Коллекция сведений о регистрации и состоянии для пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="32db3-126">A collection of registration count and status information for users in your tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="32db3-127">Связи</span><span class="sxs-lookup"><span data-stu-id="32db3-127">Relationships</span></span>

<span data-ttu-id="32db3-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="32db3-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="32db3-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="32db3-129">JSON representation</span></span>

<span data-ttu-id="32db3-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32db3-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationCount",
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

