---
title: Тип ресурса Кредентиалусеррегистратиондетаилс
description: Представляет сведения об использовании функции автоматического сброса пароля и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: e5bb982df85ac977a21808b28eec569fbb0d1f36
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383526"
---
# <a name="credentialuserregistrationdetails-resource-type"></a><span data-ttu-id="37c90-103">Тип ресурса Кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="37c90-103">credentialUserRegistrationDetails resource type</span></span>

<span data-ttu-id="37c90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37c90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37c90-105">Представляет сведения об использовании функции автоматического сброса пароля и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.</span><span class="sxs-lookup"><span data-stu-id="37c90-105">Represents the details of the usage of self-service password reset and multi-factor authentication (MFA) for all registered users.</span></span> <span data-ttu-id="37c90-106">Сведения включают сведения о пользователе, состояние регистрации и используемый способ проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="37c90-106">Details include user information, status of registration, and the authentication method used.</span></span>

## <a name="methods"></a><span data-ttu-id="37c90-107">Методы</span><span class="sxs-lookup"><span data-stu-id="37c90-107">Methods</span></span>

| <span data-ttu-id="37c90-108">Метод</span><span class="sxs-lookup"><span data-stu-id="37c90-108">Method</span></span>       | <span data-ttu-id="37c90-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="37c90-109">Return Type</span></span> | <span data-ttu-id="37c90-110">Описание</span><span class="sxs-lookup"><span data-stu-id="37c90-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="37c90-111">Список Кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="37c90-111">List credentialUserRegistrationDetails</span></span>](../api/reportroot-list-credentialuserregistrationdetails.md) | <span data-ttu-id="37c90-112">Коллекция Кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="37c90-112">credentialUserRegistrationDetails collection</span></span> | <span data-ttu-id="37c90-113">Получение списка объектов [кредентиалусеррегистратиондетаилс](../resources/credentialuserregistrationdetails.md) для определенного клиента.</span><span class="sxs-lookup"><span data-stu-id="37c90-113">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="37c90-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="37c90-114">Properties</span></span>

| <span data-ttu-id="37c90-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="37c90-115">Property</span></span>     | <span data-ttu-id="37c90-116">Тип</span><span class="sxs-lookup"><span data-stu-id="37c90-116">Type</span></span>        | <span data-ttu-id="37c90-117">Описание</span><span class="sxs-lookup"><span data-stu-id="37c90-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="37c90-118">аусмесодс</span><span class="sxs-lookup"><span data-stu-id="37c90-118">authMethods</span></span> | <span data-ttu-id="37c90-119">Коллекция Регистратионаусмесод</span><span class="sxs-lookup"><span data-stu-id="37c90-119">registrationAuthMethod collection</span></span> | <span data-ttu-id="37c90-120">Представляет способ проверки подлинности, используемый пользователем.</span><span class="sxs-lookup"><span data-stu-id="37c90-120">Represents the authentication method that the user used.</span></span> <span data-ttu-id="37c90-121">`email`Возможные значения:, `mobilePhone`, `officePhone`, `securityQuestion` (только для самостоятельного сброса пароля), `appNotification` `appCode`и `alternateMobilePhone` (поддерживается только при регистрации).</span><span class="sxs-lookup"><span data-stu-id="37c90-121">Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobilePhone` (supported only in registration).</span></span> |
| <span data-ttu-id="37c90-122">id</span><span class="sxs-lookup"><span data-stu-id="37c90-122">id</span></span> | <span data-ttu-id="37c90-123">Строка</span><span class="sxs-lookup"><span data-stu-id="37c90-123">String</span></span> | <span data-ttu-id="37c90-124">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="37c90-124">The unique identifier for the activity.</span></span> <span data-ttu-id="37c90-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37c90-125">Read-only.</span></span>|
| <span data-ttu-id="37c90-126">Поддержка</span><span class="sxs-lookup"><span data-stu-id="37c90-126">isCapable</span></span> | <span data-ttu-id="37c90-127">Логическое</span><span class="sxs-lookup"><span data-stu-id="37c90-127">Boolean</span></span> | <span data-ttu-id="37c90-128">Указывает, готов ли пользователь к выполнению самостоятельного сброса пароля или MFA.</span><span class="sxs-lookup"><span data-stu-id="37c90-128">Indicates whether the user is ready to perform self-service password reset or MFA.</span></span> |
| <span data-ttu-id="37c90-129">isEnabled</span><span class="sxs-lookup"><span data-stu-id="37c90-129">isEnabled</span></span> | <span data-ttu-id="37c90-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="37c90-130">Boolean</span></span> | <span data-ttu-id="37c90-131">ИндиЦиатес, разрешено ли пользователю выполнять сброс пароля самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="37c90-131">Indiciates whether the user enabled to perform self-service password reset.</span></span> |
| <span data-ttu-id="37c90-132">исмфарегистеред</span><span class="sxs-lookup"><span data-stu-id="37c90-132">isMfaRegistered</span></span> | <span data-ttu-id="37c90-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="37c90-133">Boolean</span></span> | <span data-ttu-id="37c90-134">ИндиЦиатес, зарегистрирован ли пользователь для MFA.</span><span class="sxs-lookup"><span data-stu-id="37c90-134">Indiciates whether the user is registered for MFA.</span></span> |
| <span data-ttu-id="37c90-135">Регистрация</span><span class="sxs-lookup"><span data-stu-id="37c90-135">isRegistered</span></span> | <span data-ttu-id="37c90-136">Логическое</span><span class="sxs-lookup"><span data-stu-id="37c90-136">Boolean</span></span> | <span data-ttu-id="37c90-137">Указывает, зарегистрировал ли пользователь какие бы то ни было методы проверки подлинности для самостоятельного сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="37c90-137">Indicates whether the user has registered any authentication methods for self-service password reset.</span></span> |
| <span data-ttu-id="37c90-138">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="37c90-138">userDisplayName</span></span> | <span data-ttu-id="37c90-139">String</span><span class="sxs-lookup"><span data-stu-id="37c90-139">String</span></span> | <span data-ttu-id="37c90-140">Предоставляет имя пользователя для соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="37c90-140">Provides the user name of the corresponding user.</span></span> |
| <span data-ttu-id="37c90-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="37c90-141">userPrincipalName</span></span> | <span data-ttu-id="37c90-142">String</span><span class="sxs-lookup"><span data-stu-id="37c90-142">String</span></span> | <span data-ttu-id="37c90-143">Предоставляет имя участника пользователя для соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="37c90-143">Provides the user principal name of the corresponding user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="37c90-144">Связи</span><span class="sxs-lookup"><span data-stu-id="37c90-144">Relationships</span></span>

<span data-ttu-id="37c90-145">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="37c90-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="37c90-146">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="37c90-146">JSON representation</span></span>

<span data-ttu-id="37c90-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37c90-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "baseType": "",
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