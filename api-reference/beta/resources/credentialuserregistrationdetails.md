---
title: Тип ресурса Кредентиалусеррегистратиондетаилс
description: Представляет сведения об использовании функции автоматического сброса пароля и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.
localization_priority: Normal
author: khotz
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: fb852bb20fa8564f81e3dbcb027fced3d630f36b
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598460"
---
# <a name="credentialuserregistrationdetails-resource-type"></a><span data-ttu-id="84d14-103">Тип ресурса Кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="84d14-103">credentialUserRegistrationDetails resource type</span></span>

<span data-ttu-id="84d14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84d14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84d14-105">Представляет сведения об использовании функции автоматического сброса пароля и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.</span><span class="sxs-lookup"><span data-stu-id="84d14-105">Represents the details of the usage of self-service password reset and multi-factor authentication (MFA) for all registered users.</span></span> <span data-ttu-id="84d14-106">Сведения включают сведения о пользователе, состояние регистрации и используемый способ проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="84d14-106">Details include user information, status of registration, and the authentication method used.</span></span>

## <a name="methods"></a><span data-ttu-id="84d14-107">Методы</span><span class="sxs-lookup"><span data-stu-id="84d14-107">Methods</span></span>

| <span data-ttu-id="84d14-108">Метод</span><span class="sxs-lookup"><span data-stu-id="84d14-108">Method</span></span>       | <span data-ttu-id="84d14-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="84d14-109">Return Type</span></span> | <span data-ttu-id="84d14-110">Описание</span><span class="sxs-lookup"><span data-stu-id="84d14-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="84d14-111">Список Кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="84d14-111">List credentialUserRegistrationDetails</span></span>](../api/reportroot-list-credentialuserregistrationdetails.md) | <span data-ttu-id="84d14-112">Коллекция Кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="84d14-112">credentialUserRegistrationDetails collection</span></span> | <span data-ttu-id="84d14-113">Получение списка объектов [кредентиалусеррегистратиондетаилс](../resources/credentialuserregistrationdetails.md) для определенного клиента.</span><span class="sxs-lookup"><span data-stu-id="84d14-113">Get a list of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects for a given tenant.</span></span>
 |

## <a name="properties"></a><span data-ttu-id="84d14-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="84d14-114">Properties</span></span>

| <span data-ttu-id="84d14-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="84d14-115">Property</span></span>     | <span data-ttu-id="84d14-116">Тип</span><span class="sxs-lookup"><span data-stu-id="84d14-116">Type</span></span>        | <span data-ttu-id="84d14-117">Описание</span><span class="sxs-lookup"><span data-stu-id="84d14-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="84d14-118">аусмесодс</span><span class="sxs-lookup"><span data-stu-id="84d14-118">authMethods</span></span> | <span data-ttu-id="84d14-119">Коллекция Регистратионаусмесод</span><span class="sxs-lookup"><span data-stu-id="84d14-119">registrationAuthMethod collection</span></span> | <span data-ttu-id="84d14-120">Представляет способ проверки подлинности, зарегистрированный пользователем.</span><span class="sxs-lookup"><span data-stu-id="84d14-120">Represents the authentication method that the user has registered.</span></span> <span data-ttu-id="84d14-121">Возможные значения: `email` , `mobilePhone` ,, `officePhone` `securityQuestion` (только для самостоятельного сброса пароля), `appNotification` `appCode` и `alternateMobilePhone` (поддерживается только при регистрации).</span><span class="sxs-lookup"><span data-stu-id="84d14-121">Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobilePhone` (supported only in registration).</span></span> |
| <span data-ttu-id="84d14-122">id</span><span class="sxs-lookup"><span data-stu-id="84d14-122">id</span></span> | <span data-ttu-id="84d14-123">String</span><span class="sxs-lookup"><span data-stu-id="84d14-123">String</span></span> | <span data-ttu-id="84d14-124">Уникальный идентификатор действия.</span><span class="sxs-lookup"><span data-stu-id="84d14-124">The unique identifier for the activity.</span></span> <span data-ttu-id="84d14-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84d14-125">Read-only.</span></span>|
| <span data-ttu-id="84d14-126">Поддержка</span><span class="sxs-lookup"><span data-stu-id="84d14-126">isCapable</span></span> | <span data-ttu-id="84d14-127">Логический</span><span class="sxs-lookup"><span data-stu-id="84d14-127">Boolean</span></span> | <span data-ttu-id="84d14-128">Указывает, готов ли пользователь к выполнению самостоятельного сброса пароля или MFA.</span><span class="sxs-lookup"><span data-stu-id="84d14-128">Indicates whether the user is ready to perform self-service password reset or MFA.</span></span> |
| <span data-ttu-id="84d14-129">isEnabled</span><span class="sxs-lookup"><span data-stu-id="84d14-129">isEnabled</span></span> | <span data-ttu-id="84d14-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="84d14-130">Boolean</span></span> | <span data-ttu-id="84d14-131">ИндиЦиатес, разрешено ли пользователю выполнять сброс пароля самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="84d14-131">Indiciates whether the user enabled to perform self-service password reset.</span></span> |
| <span data-ttu-id="84d14-132">исмфарегистеред</span><span class="sxs-lookup"><span data-stu-id="84d14-132">isMfaRegistered</span></span> | <span data-ttu-id="84d14-133">Логический</span><span class="sxs-lookup"><span data-stu-id="84d14-133">Boolean</span></span> | <span data-ttu-id="84d14-134">ИндиЦиатес, зарегистрирован ли пользователь для MFA.</span><span class="sxs-lookup"><span data-stu-id="84d14-134">Indiciates whether the user is registered for MFA.</span></span> |
| <span data-ttu-id="84d14-135">Регистрация</span><span class="sxs-lookup"><span data-stu-id="84d14-135">isRegistered</span></span> | <span data-ttu-id="84d14-136">Логический</span><span class="sxs-lookup"><span data-stu-id="84d14-136">Boolean</span></span> | <span data-ttu-id="84d14-137">Указывает, зарегистрировал ли пользователь какие бы то ни было методы проверки подлинности для самостоятельного сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="84d14-137">Indicates whether the user has registered any authentication methods for self-service password reset.</span></span> |
| <span data-ttu-id="84d14-138">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="84d14-138">userDisplayName</span></span> | <span data-ttu-id="84d14-139">String</span><span class="sxs-lookup"><span data-stu-id="84d14-139">String</span></span> | <span data-ttu-id="84d14-140">Предоставляет имя пользователя для соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="84d14-140">Provides the user name of the corresponding user.</span></span> |
| <span data-ttu-id="84d14-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="84d14-141">userPrincipalName</span></span> | <span data-ttu-id="84d14-142">String</span><span class="sxs-lookup"><span data-stu-id="84d14-142">String</span></span> | <span data-ttu-id="84d14-143">Предоставляет имя участника пользователя для соответствующего пользователя.</span><span class="sxs-lookup"><span data-stu-id="84d14-143">Provides the user principal name of the corresponding user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="84d14-144">Связи</span><span class="sxs-lookup"><span data-stu-id="84d14-144">Relationships</span></span>

<span data-ttu-id="84d14-145">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="84d14-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="84d14-146">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="84d14-146">JSON representation</span></span>

<span data-ttu-id="84d14-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84d14-147">The following is a JSON representation of the resource.</span></span>

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
