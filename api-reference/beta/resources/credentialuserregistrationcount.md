---
title: Тип ресурса credentialUserRegistrationCount
description: Представляет текущее состояние регистрации пользователей в организации для самостоятельного сброса паролей и многофакторной проверки подлинности.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: cb83bbfe4c738fd8c5c6460a27aafbbc73cad437
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136278"
---
# <a name="credentialuserregistrationcount-resource-type"></a><span data-ttu-id="8a4ec-103">Тип ресурса credentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="8a4ec-103">credentialUserRegistrationCount resource type</span></span>

<span data-ttu-id="8a4ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a4ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a4ec-105">Представляет текущее состояние регистрации пользователей в организации для самостоятельного сброса паролей и многофакторной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="8a4ec-105">Represents the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication capabilities.</span></span>

## <a name="methods"></a><span data-ttu-id="8a4ec-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8a4ec-106">Methods</span></span>

| <span data-ttu-id="8a4ec-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8a4ec-107">Method</span></span>       | <span data-ttu-id="8a4ec-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8a4ec-108">Return Type</span></span> | <span data-ttu-id="8a4ec-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8a4ec-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8a4ec-110">getCredentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="8a4ec-110">getCredentialUserRegistrationCount</span></span>](../api/reportroot-getcredentialuserregistrationcount.md) | <span data-ttu-id="8a4ec-111">Коллекция credentialUserRegistrationCount</span><span class="sxs-lookup"><span data-stu-id="8a4ec-111">credentialUserRegistrationCount collection</span></span> | <span data-ttu-id="8a4ec-112">Фиксируйте текущее состояние регистрации пользователей в организации для самостоятельного сброса паролей и многофакторной проверки подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="8a4ec-112">Report the current state of how many users in your organization are registered for self-service password reset and multi-factor authentication (MFA) capabilities.</span></span> |

## <a name="properties"></a><span data-ttu-id="8a4ec-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a4ec-113">Properties</span></span>

| <span data-ttu-id="8a4ec-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a4ec-114">Property</span></span>     | <span data-ttu-id="8a4ec-115">Тип</span><span class="sxs-lookup"><span data-stu-id="8a4ec-115">Type</span></span>        | <span data-ttu-id="8a4ec-116">Описание</span><span class="sxs-lookup"><span data-stu-id="8a4ec-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8a4ec-117">id</span><span class="sxs-lookup"><span data-stu-id="8a4ec-117">id</span></span> | <span data-ttu-id="8a4ec-118">Строка</span><span class="sxs-lookup"><span data-stu-id="8a4ec-118">String</span></span> | <span data-ttu-id="8a4ec-119">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="8a4ec-119">The unique identifier for the activity.</span></span> <span data-ttu-id="8a4ec-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a4ec-120">Read-only.</span></span> |
| <span data-ttu-id="8a4ec-121">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="8a4ec-121">totalUserCount</span></span> | <span data-ttu-id="8a4ec-122">Int64</span><span class="sxs-lookup"><span data-stu-id="8a4ec-122">Int64</span></span> | <span data-ttu-id="8a4ec-123">Предоставляет общее количество пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="8a4ec-123">Provides the total user count in the tenant.</span></span> |
| <span data-ttu-id="8a4ec-124">userRegistrationCounts</span><span class="sxs-lookup"><span data-stu-id="8a4ec-124">userRegistrationCounts</span></span> | <span data-ttu-id="8a4ec-125">[Коллекция userRegistrationCount](userregistrationcount.md)</span><span class="sxs-lookup"><span data-stu-id="8a4ec-125">[userRegistrationCount](userregistrationcount.md) collection</span></span> | <span data-ttu-id="8a4ec-126">Коллекция сведений о регистрации и состоянии для пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="8a4ec-126">A collection of registration count and status information for users in your tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8a4ec-127">Связи</span><span class="sxs-lookup"><span data-stu-id="8a4ec-127">Relationships</span></span>

<span data-ttu-id="8a4ec-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8a4ec-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a4ec-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8a4ec-129">JSON representation</span></span>

<span data-ttu-id="8a4ec-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a4ec-130">The following is a JSON representation of the resource.</span></span>

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

