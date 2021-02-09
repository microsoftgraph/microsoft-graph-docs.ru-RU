---
title: Тип ресурса credentialUserRegistrationDetails
description: Представляет сведения об использовании самостоятельного сброса паролей и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c7e45b186e1ef7a3a96115f408cb5a0992e538fe
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159908"
---
# <a name="credentialuserregistrationdetails-resource-type"></a><span data-ttu-id="19f84-103">Тип ресурса credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="19f84-103">credentialUserRegistrationDetails resource type</span></span>

<span data-ttu-id="19f84-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19f84-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19f84-105">Представляет сведения об использовании самостоятельного сброса пароля и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.</span><span class="sxs-lookup"><span data-stu-id="19f84-105">Represents the details of the usage of self-service password reset and multi-factor authentication (MFA) for all registered users.</span></span> <span data-ttu-id="19f84-106">Сведения включают сведения о пользователе, состояние регистрации и используемый метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="19f84-106">Details include user information, status of registration, and the authentication method used.</span></span>

## <a name="methods"></a><span data-ttu-id="19f84-107">Методы</span><span class="sxs-lookup"><span data-stu-id="19f84-107">Methods</span></span>

| <span data-ttu-id="19f84-108">Метод</span><span class="sxs-lookup"><span data-stu-id="19f84-108">Method</span></span>       | <span data-ttu-id="19f84-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="19f84-109">Return Type</span></span> | <span data-ttu-id="19f84-110">Описание</span><span class="sxs-lookup"><span data-stu-id="19f84-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="19f84-111">Список credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="19f84-111">List credentialUserRegistrationDetails</span></span>](../api/reportroot-list-credentialuserregistrationdetails.md) | <span data-ttu-id="19f84-112">Коллекция credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="19f84-112">credentialUserRegistrationDetails collection</span></span> | <span data-ttu-id="19f84-113">Получите список объектов [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="19f84-113">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="19f84-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="19f84-114">Properties</span></span>

| <span data-ttu-id="19f84-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="19f84-115">Property</span></span>     | <span data-ttu-id="19f84-116">Тип</span><span class="sxs-lookup"><span data-stu-id="19f84-116">Type</span></span>        | <span data-ttu-id="19f84-117">Описание</span><span class="sxs-lookup"><span data-stu-id="19f84-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="19f84-118">authMethods</span><span class="sxs-lookup"><span data-stu-id="19f84-118">authMethods</span></span> | <span data-ttu-id="19f84-119">коллекция registrationAuthMethod</span><span class="sxs-lookup"><span data-stu-id="19f84-119">registrationAuthMethod collection</span></span> | <span data-ttu-id="19f84-120">Представляет метод проверки подлинности, зарегистрированный пользователем.</span><span class="sxs-lookup"><span data-stu-id="19f84-120">Represents the authentication method that the user has registered.</span></span> <span data-ttu-id="19f84-121">Возможные значения: , , , (используется только для самостоятельного сброса `email` `mobilePhone` `officePhone` `securityQuestion` пароля), `appNotification` , и `appCode` `alternateMobilePhone` (поддерживается только при регистрации).</span><span class="sxs-lookup"><span data-stu-id="19f84-121">Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobilePhone` (supported only in registration).</span></span> |
| <span data-ttu-id="19f84-122">id</span><span class="sxs-lookup"><span data-stu-id="19f84-122">id</span></span> | <span data-ttu-id="19f84-123">String</span><span class="sxs-lookup"><span data-stu-id="19f84-123">String</span></span> | <span data-ttu-id="19f84-124">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="19f84-124">The unique identifier for the activity.</span></span> <span data-ttu-id="19f84-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19f84-125">Read-only.</span></span>|
| <span data-ttu-id="19f84-126">isCapable</span><span class="sxs-lookup"><span data-stu-id="19f84-126">isCapable</span></span> | <span data-ttu-id="19f84-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="19f84-127">Boolean</span></span> | <span data-ttu-id="19f84-128">Указывает, готов ли пользователь к самостоятельному сбросу пароля или MFA.</span><span class="sxs-lookup"><span data-stu-id="19f84-128">Indicates whether the user is ready to perform self-service password reset or MFA.</span></span> |
| <span data-ttu-id="19f84-129">isEnabled</span><span class="sxs-lookup"><span data-stu-id="19f84-129">isEnabled</span></span> | <span data-ttu-id="19f84-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="19f84-130">Boolean</span></span> | <span data-ttu-id="19f84-131">Не сообщает, включен ли для пользователя самостоятельный сброс пароля.</span><span class="sxs-lookup"><span data-stu-id="19f84-131">Indiciates whether the user enabled to perform self-service password reset.</span></span> |
| <span data-ttu-id="19f84-132">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="19f84-132">isMfaRegistered</span></span> | <span data-ttu-id="19f84-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="19f84-133">Boolean</span></span> | <span data-ttu-id="19f84-134">Не сообщает, зарегистрирован ли пользователь для MFA.</span><span class="sxs-lookup"><span data-stu-id="19f84-134">Indiciates whether the user is registered for MFA.</span></span> |
| <span data-ttu-id="19f84-135">isRegistered</span><span class="sxs-lookup"><span data-stu-id="19f84-135">isRegistered</span></span> | <span data-ttu-id="19f84-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="19f84-136">Boolean</span></span> | <span data-ttu-id="19f84-137">Указывает, зарегистрирован ли пользователь какие-либо методы проверки подлинности для самостоятельного сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="19f84-137">Indicates whether the user has registered any authentication methods for self-service password reset.</span></span> |
| <span data-ttu-id="19f84-138">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="19f84-138">userDisplayName</span></span> | <span data-ttu-id="19f84-139">String</span><span class="sxs-lookup"><span data-stu-id="19f84-139">String</span></span> | <span data-ttu-id="19f84-140">Предоставляет имя соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="19f84-140">Provides the user name of the corresponding user.</span></span> |
| <span data-ttu-id="19f84-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="19f84-141">userPrincipalName</span></span> | <span data-ttu-id="19f84-142">String</span><span class="sxs-lookup"><span data-stu-id="19f84-142">String</span></span> | <span data-ttu-id="19f84-143">Предоставляет имя основного пользователя соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="19f84-143">Provides the user principal name of the corresponding user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="19f84-144">Связи</span><span class="sxs-lookup"><span data-stu-id="19f84-144">Relationships</span></span>

<span data-ttu-id="19f84-145">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="19f84-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="19f84-146">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="19f84-146">JSON representation</span></span>

<span data-ttu-id="19f84-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19f84-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "authMethods": ["string"],
  "isRegistered" : false,
  "isEnabled" : true,
  "isCapable" : false,
  "isMfaRegistered" : true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credentialUserRegistrationDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


