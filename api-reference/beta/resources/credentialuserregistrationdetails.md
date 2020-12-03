---
title: Тип ресурса Кредентиалусеррегистратиондетаилс
description: Представляет сведения об использовании функции автоматического сброса пароля и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.
localization_priority: Normal
author: besiler
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 56d3f603fd9a8daf0c19e30c566379390aca7aed
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523740"
---
# <a name="credentialuserregistrationdetails-resource-type"></a><span data-ttu-id="3d20f-103">Тип ресурса Кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="3d20f-103">credentialUserRegistrationDetails resource type</span></span>

<span data-ttu-id="3d20f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d20f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d20f-105">Представляет сведения об использовании функции автоматического сброса пароля и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.</span><span class="sxs-lookup"><span data-stu-id="3d20f-105">Represents the details of the usage of self-service password reset and multi-factor authentication (MFA) for all registered users.</span></span> <span data-ttu-id="3d20f-106">Сведения включают сведения о пользователе, состояние регистрации и используемый способ проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="3d20f-106">Details include user information, status of registration, and the authentication method used.</span></span>

## <a name="methods"></a><span data-ttu-id="3d20f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3d20f-107">Methods</span></span>

| <span data-ttu-id="3d20f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3d20f-108">Method</span></span>       | <span data-ttu-id="3d20f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3d20f-109">Return Type</span></span> | <span data-ttu-id="3d20f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3d20f-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3d20f-111">Список Кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="3d20f-111">List credentialUserRegistrationDetails</span></span>](../api/reportroot-list-credentialuserregistrationdetails.md) | <span data-ttu-id="3d20f-112">Коллекция Кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="3d20f-112">credentialUserRegistrationDetails collection</span></span> | <span data-ttu-id="3d20f-113">Получение списка объектов [кредентиалусеррегистратиондетаилс](../resources/credentialuserregistrationdetails.md) для определенного клиента.</span><span class="sxs-lookup"><span data-stu-id="3d20f-113">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="3d20f-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d20f-114">Properties</span></span>

| <span data-ttu-id="3d20f-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d20f-115">Property</span></span>     | <span data-ttu-id="3d20f-116">Тип</span><span class="sxs-lookup"><span data-stu-id="3d20f-116">Type</span></span>        | <span data-ttu-id="3d20f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="3d20f-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3d20f-118">аусмесодс</span><span class="sxs-lookup"><span data-stu-id="3d20f-118">authMethods</span></span> | <span data-ttu-id="3d20f-119">Коллекция Регистратионаусмесод</span><span class="sxs-lookup"><span data-stu-id="3d20f-119">registrationAuthMethod collection</span></span> | <span data-ttu-id="3d20f-120">Представляет способ проверки подлинности, зарегистрированный пользователем.</span><span class="sxs-lookup"><span data-stu-id="3d20f-120">Represents the authentication method that the user has registered.</span></span> <span data-ttu-id="3d20f-121">Возможные значения: `email` , `mobilePhone` ,, `officePhone` `securityQuestion` (только для самостоятельного сброса пароля), `appNotification` `appCode` и `alternateMobilePhone` (поддерживается только при регистрации).</span><span class="sxs-lookup"><span data-stu-id="3d20f-121">Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobilePhone` (supported only in registration).</span></span> |
| <span data-ttu-id="3d20f-122">id</span><span class="sxs-lookup"><span data-stu-id="3d20f-122">id</span></span> | <span data-ttu-id="3d20f-123">String</span><span class="sxs-lookup"><span data-stu-id="3d20f-123">String</span></span> | <span data-ttu-id="3d20f-124">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="3d20f-124">The unique identifier for the activity.</span></span> <span data-ttu-id="3d20f-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d20f-125">Read-only.</span></span>|
| <span data-ttu-id="3d20f-126">Поддержка</span><span class="sxs-lookup"><span data-stu-id="3d20f-126">isCapable</span></span> | <span data-ttu-id="3d20f-127">Логический</span><span class="sxs-lookup"><span data-stu-id="3d20f-127">Boolean</span></span> | <span data-ttu-id="3d20f-128">Указывает, готов ли пользователь к выполнению самостоятельного сброса пароля или MFA.</span><span class="sxs-lookup"><span data-stu-id="3d20f-128">Indicates whether the user is ready to perform self-service password reset or MFA.</span></span> |
| <span data-ttu-id="3d20f-129">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3d20f-129">isEnabled</span></span> | <span data-ttu-id="3d20f-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d20f-130">Boolean</span></span> | <span data-ttu-id="3d20f-131">ИндиЦиатес, разрешено ли пользователю выполнять сброс пароля самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="3d20f-131">Indiciates whether the user enabled to perform self-service password reset.</span></span> |
| <span data-ttu-id="3d20f-132">исмфарегистеред</span><span class="sxs-lookup"><span data-stu-id="3d20f-132">isMfaRegistered</span></span> | <span data-ttu-id="3d20f-133">Логический</span><span class="sxs-lookup"><span data-stu-id="3d20f-133">Boolean</span></span> | <span data-ttu-id="3d20f-134">ИндиЦиатес, зарегистрирован ли пользователь для MFA.</span><span class="sxs-lookup"><span data-stu-id="3d20f-134">Indiciates whether the user is registered for MFA.</span></span> |
| <span data-ttu-id="3d20f-135">Регистрация</span><span class="sxs-lookup"><span data-stu-id="3d20f-135">isRegistered</span></span> | <span data-ttu-id="3d20f-136">Логический</span><span class="sxs-lookup"><span data-stu-id="3d20f-136">Boolean</span></span> | <span data-ttu-id="3d20f-137">Указывает, зарегистрировал ли пользователь какие бы то ни было методы проверки подлинности для самостоятельного сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="3d20f-137">Indicates whether the user has registered any authentication methods for self-service password reset.</span></span> |
| <span data-ttu-id="3d20f-138">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3d20f-138">userDisplayName</span></span> | <span data-ttu-id="3d20f-139">String</span><span class="sxs-lookup"><span data-stu-id="3d20f-139">String</span></span> | <span data-ttu-id="3d20f-140">Предоставляет имя пользователя для соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="3d20f-140">Provides the user name of the corresponding user.</span></span> |
| <span data-ttu-id="3d20f-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3d20f-141">userPrincipalName</span></span> | <span data-ttu-id="3d20f-142">String</span><span class="sxs-lookup"><span data-stu-id="3d20f-142">String</span></span> | <span data-ttu-id="3d20f-143">Предоставляет имя участника пользователя для соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="3d20f-143">Provides the user principal name of the corresponding user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3d20f-144">Связи</span><span class="sxs-lookup"><span data-stu-id="3d20f-144">Relationships</span></span>

<span data-ttu-id="3d20f-145">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3d20f-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d20f-146">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3d20f-146">JSON representation</span></span>

<span data-ttu-id="3d20f-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d20f-147">The following is a JSON representation of the resource.</span></span>

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


