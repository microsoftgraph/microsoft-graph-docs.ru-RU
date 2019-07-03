---
title: Тип ресурса Кредентиалусеррегистратиондетаилс
description: Представляет сведения об использовании функции автоматического сброса пароля и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 414cd6977f4e3c15ab7b82bd88329e9e3549f137
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529191"
---
# <a name="credentialuserregistrationdetails-resource-type"></a><span data-ttu-id="425e7-103">Тип ресурса Кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="425e7-103">credentialUserRegistrationDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="425e7-104">Представляет сведения об использовании функции автоматического сброса пароля и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.</span><span class="sxs-lookup"><span data-stu-id="425e7-104">Represents the details of the usage of self-service password reset and multi-factor authentication (MFA) for all registered users.</span></span> <span data-ttu-id="425e7-105">Сведения включают сведения о пользователе, состояние регистрации и используемый способ проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="425e7-105">Details include user information, status of registration, and the authentication method used.</span></span>

## <a name="methods"></a><span data-ttu-id="425e7-106">Методы</span><span class="sxs-lookup"><span data-stu-id="425e7-106">Methods</span></span>

| <span data-ttu-id="425e7-107">Метод</span><span class="sxs-lookup"><span data-stu-id="425e7-107">Method</span></span>       | <span data-ttu-id="425e7-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="425e7-108">Return Type</span></span> | <span data-ttu-id="425e7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="425e7-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="425e7-110">Список Кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="425e7-110">List credentialUserRegistrationDetails</span></span>](../api/reportroot-list-credentialuserregistrationdetails.md) | <span data-ttu-id="425e7-111">Коллекция Кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="425e7-111">credentialUserRegistrationDetails collection</span></span> | <span data-ttu-id="425e7-112">Получение списка объектов [кредентиалусеррегистратиондетаилс](../resources/credentialuserregistrationdetails.md) для определенного клиента.</span><span class="sxs-lookup"><span data-stu-id="425e7-112">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="425e7-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="425e7-113">Properties</span></span>

| <span data-ttu-id="425e7-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="425e7-114">Property</span></span>     | <span data-ttu-id="425e7-115">Тип</span><span class="sxs-lookup"><span data-stu-id="425e7-115">Type</span></span>        | <span data-ttu-id="425e7-116">Описание</span><span class="sxs-lookup"><span data-stu-id="425e7-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="425e7-117">Аусмесодс</span><span class="sxs-lookup"><span data-stu-id="425e7-117">authMethods</span></span> | <span data-ttu-id="425e7-118">Коллекция Регистратионаусмесод</span><span class="sxs-lookup"><span data-stu-id="425e7-118">registrationAuthMethod collection</span></span> | <span data-ttu-id="425e7-119">Представляет способ проверки подлинности, используемый пользователем.</span><span class="sxs-lookup"><span data-stu-id="425e7-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="425e7-120">`email`Возможные значения:, `mobilePhone`, `officePhone`, `securityQuestion` (только для самостоятельного сброса пароля), `appNotification` `appCode`и `alternateMobilePhone` (поддерживается только при регистрации).</span><span class="sxs-lookup"><span data-stu-id="425e7-120">Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobilePhone` (supported only in registration).</span></span> |
| <span data-ttu-id="425e7-121">id</span><span class="sxs-lookup"><span data-stu-id="425e7-121">id</span></span> | <span data-ttu-id="425e7-122">Строка</span><span class="sxs-lookup"><span data-stu-id="425e7-122">String</span></span> | <span data-ttu-id="425e7-123">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="425e7-123">The unique identifier for the activity.</span></span> <span data-ttu-id="425e7-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="425e7-124">Read-only.</span></span>|
| <span data-ttu-id="425e7-125">Поддержка</span><span class="sxs-lookup"><span data-stu-id="425e7-125">isCapable</span></span> | <span data-ttu-id="425e7-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="425e7-126">Boolean</span></span> | <span data-ttu-id="425e7-127">Указывает, готов ли пользователь к выполнению самостоятельного сброса пароля или MFA.</span><span class="sxs-lookup"><span data-stu-id="425e7-127">Indicates whether the user is ready to perform self-service password reset or MFA.</span></span> |
| <span data-ttu-id="425e7-128">isEnabled</span><span class="sxs-lookup"><span data-stu-id="425e7-128">isEnabled</span></span> | <span data-ttu-id="425e7-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="425e7-129">Boolean</span></span> | <span data-ttu-id="425e7-130">ИндиЦиатес, разрешено ли пользователю выполнять сброс пароля самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="425e7-130">Indiciates whether the user enabled to perform self-service password reset.</span></span> |
| <span data-ttu-id="425e7-131">Исмфарегистеред</span><span class="sxs-lookup"><span data-stu-id="425e7-131">isMfaRegistered</span></span> | <span data-ttu-id="425e7-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="425e7-132">Boolean</span></span> | <span data-ttu-id="425e7-133">ИндиЦиатес, зарегистрирован ли пользователь для MFA.</span><span class="sxs-lookup"><span data-stu-id="425e7-133">Indiciates whether the user is registered for MFA.</span></span> |
| <span data-ttu-id="425e7-134">Регистрация</span><span class="sxs-lookup"><span data-stu-id="425e7-134">isRegistered</span></span> | <span data-ttu-id="425e7-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="425e7-135">Boolean</span></span> | <span data-ttu-id="425e7-136">Указывает, зарегистрировал ли пользователь какие бы то ни было методы проверки подлинности для самостоятельного сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="425e7-136">Indicates whether the user has registered any authentication methods for self-service password reset.</span></span> |
| <span data-ttu-id="425e7-137">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="425e7-137">userDisplayName</span></span> | <span data-ttu-id="425e7-138">String</span><span class="sxs-lookup"><span data-stu-id="425e7-138">String</span></span> | <span data-ttu-id="425e7-139">Предоставляет имя пользователя для соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="425e7-139">Provides the user name of the corresponding user.</span></span> |
| <span data-ttu-id="425e7-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="425e7-140">userPrincipalName</span></span> | <span data-ttu-id="425e7-141">String</span><span class="sxs-lookup"><span data-stu-id="425e7-141">String</span></span> | <span data-ttu-id="425e7-142">Предоставляет имя участника пользователя для соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="425e7-142">Provides the user principal name of the corresponding user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="425e7-143">Отношения</span><span class="sxs-lookup"><span data-stu-id="425e7-143">Relationships</span></span>

<span data-ttu-id="425e7-144">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="425e7-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="425e7-145">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="425e7-145">JSON representation</span></span>

<span data-ttu-id="425e7-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="425e7-146">The following is a JSON representation of the resource.</span></span>

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