---
title: тип ресурса credentialUserRegistrationDetails
description: Представляет сведения об использовании сброса пароля самообслуживления и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: ac5712bf3c0d396f7ddc84c4812b4e1ed7090355
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941815"
---
# <a name="credentialuserregistrationdetails-resource-type"></a><span data-ttu-id="859a5-103">тип ресурса credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="859a5-103">credentialUserRegistrationDetails resource type</span></span>

<span data-ttu-id="859a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="859a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="859a5-105">Представляет сведения об использовании сброса пароля самообслуживления и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.</span><span class="sxs-lookup"><span data-stu-id="859a5-105">Represents the details of the usage of self-service password reset and multi-factor authentication (MFA) for all registered users.</span></span> <span data-ttu-id="859a5-106">Сведения включают сведения о пользователях, состояние регистрации и используемый метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="859a5-106">Details include user information, status of registration, and the authentication method used.</span></span>

## <a name="methods"></a><span data-ttu-id="859a5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="859a5-107">Methods</span></span>

| <span data-ttu-id="859a5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="859a5-108">Method</span></span>       | <span data-ttu-id="859a5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="859a5-109">Return Type</span></span> | <span data-ttu-id="859a5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="859a5-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="859a5-111">Список credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="859a5-111">List credentialUserRegistrationDetails</span></span>](../api/reportroot-list-credentialuserregistrationdetails.md) | <span data-ttu-id="859a5-112">коллекция credentialUserRegistrationDetails</span><span class="sxs-lookup"><span data-stu-id="859a5-112">credentialUserRegistrationDetails collection</span></span> | <span data-ttu-id="859a5-113">Получите список объектов [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) для данного клиента.</span><span class="sxs-lookup"><span data-stu-id="859a5-113">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="859a5-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="859a5-114">Properties</span></span>

| <span data-ttu-id="859a5-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="859a5-115">Property</span></span>     | <span data-ttu-id="859a5-116">Тип</span><span class="sxs-lookup"><span data-stu-id="859a5-116">Type</span></span>        | <span data-ttu-id="859a5-117">Описание</span><span class="sxs-lookup"><span data-stu-id="859a5-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="859a5-118">authMethods</span><span class="sxs-lookup"><span data-stu-id="859a5-118">authMethods</span></span> | <span data-ttu-id="859a5-119">registrationAuthMethod collection</span><span class="sxs-lookup"><span data-stu-id="859a5-119">registrationAuthMethod collection</span></span> | <span data-ttu-id="859a5-120">Представляет метод проверки подлинности, зарегистрированный пользователем.</span><span class="sxs-lookup"><span data-stu-id="859a5-120">Represents the authentication method that the user has registered.</span></span> <span data-ttu-id="859a5-121">Возможные значения: , , , (только используется для самообслуживки сброс `email` `mobilePhone` `officePhone`  `securityQuestion` пароля), , , ( `appNotification`  `appCode` `alternateMobilePhone` поддерживается  `fido`  `appPassword`  `unknownFutureValue` только в регистрации), , , .</span><span class="sxs-lookup"><span data-stu-id="859a5-121">Possible values are: `email`, `mobilePhone`, `officePhone`,  `securityQuestion` (only used for self-service password reset), `appNotification`,  `appCode`, `alternateMobilePhone` (supported only in registration),  `fido`,  `appPassword`,  `unknownFutureValue`.</span></span> |
| <span data-ttu-id="859a5-122">id</span><span class="sxs-lookup"><span data-stu-id="859a5-122">id</span></span> | <span data-ttu-id="859a5-123">Строка</span><span class="sxs-lookup"><span data-stu-id="859a5-123">String</span></span> | <span data-ttu-id="859a5-124">Уникальный идентификатор для этого действия.</span><span class="sxs-lookup"><span data-stu-id="859a5-124">The unique identifier for the activity.</span></span> <span data-ttu-id="859a5-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="859a5-125">Read-only.</span></span>|
| <span data-ttu-id="859a5-126">isCapable</span><span class="sxs-lookup"><span data-stu-id="859a5-126">isCapable</span></span> | <span data-ttu-id="859a5-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="859a5-127">Boolean</span></span> | <span data-ttu-id="859a5-128">Указывает, готов ли пользователь выполнять сброс пароля самообслуживки или MFA.</span><span class="sxs-lookup"><span data-stu-id="859a5-128">Indicates whether the user is ready to perform self-service password reset or MFA.</span></span> |
| <span data-ttu-id="859a5-129">isEnabled</span><span class="sxs-lookup"><span data-stu-id="859a5-129">isEnabled</span></span> | <span data-ttu-id="859a5-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="859a5-130">Boolean</span></span> | <span data-ttu-id="859a5-131">Указывает, включен ли пользователь для выполнения сброса пароля самообслуживки.</span><span class="sxs-lookup"><span data-stu-id="859a5-131">Indicates whether the user enabled to perform self-service password reset.</span></span> |
| <span data-ttu-id="859a5-132">isMfaRegistered</span><span class="sxs-lookup"><span data-stu-id="859a5-132">isMfaRegistered</span></span> | <span data-ttu-id="859a5-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="859a5-133">Boolean</span></span> | <span data-ttu-id="859a5-134">Указывает, зарегистрирован ли пользователь для MFA.</span><span class="sxs-lookup"><span data-stu-id="859a5-134">Indicates whether the user is registered for MFA.</span></span> |
| <span data-ttu-id="859a5-135">isRegistered</span><span class="sxs-lookup"><span data-stu-id="859a5-135">isRegistered</span></span> | <span data-ttu-id="859a5-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="859a5-136">Boolean</span></span> | <span data-ttu-id="859a5-137">Указывает, зарегистрировал ли пользователь какие-либо методы проверки подлинности для сброса пароля самообслуживления.</span><span class="sxs-lookup"><span data-stu-id="859a5-137">Indicates whether the user has registered any authentication methods for self-service password reset.</span></span> |
| <span data-ttu-id="859a5-138">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="859a5-138">userDisplayName</span></span> | <span data-ttu-id="859a5-139">String</span><span class="sxs-lookup"><span data-stu-id="859a5-139">String</span></span> | <span data-ttu-id="859a5-140">Предоставляет имя пользователя соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="859a5-140">Provides the user name of the corresponding user.</span></span> |
| <span data-ttu-id="859a5-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="859a5-141">userPrincipalName</span></span> | <span data-ttu-id="859a5-142">String</span><span class="sxs-lookup"><span data-stu-id="859a5-142">String</span></span> | <span data-ttu-id="859a5-143">Предоставляет основное имя пользователя соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="859a5-143">Provides the user principal name of the corresponding user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="859a5-144">Связи</span><span class="sxs-lookup"><span data-stu-id="859a5-144">Relationships</span></span>

<span data-ttu-id="859a5-145">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="859a5-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="859a5-146">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="859a5-146">JSON representation</span></span>

<span data-ttu-id="859a5-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="859a5-147">The following is a JSON representation of the resource.</span></span>

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


