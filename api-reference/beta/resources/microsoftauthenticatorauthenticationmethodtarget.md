---
title: тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, включенная для Microsoft Authenticator методов проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: db534dfb13e288b82b49005b2b1a923b8bfd5112
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896643"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="36af7-103">тип ресурса microsoftAuthenticatorAuthenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="36af7-103">microsoftAuthenticatorAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="36af7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36af7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36af7-105">Коллекция пользователей или групп, с помощью [Microsoft Authenticator методов](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) проверки подлинности в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="36af7-105">A collection of users or groups enabled to use [Microsoft Authenticator authentication methods policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="36af7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="36af7-106">Properties</span></span>
|<span data-ttu-id="36af7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="36af7-107">Property</span></span>|<span data-ttu-id="36af7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="36af7-108">Type</span></span>|<span data-ttu-id="36af7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="36af7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36af7-110">id</span><span class="sxs-lookup"><span data-stu-id="36af7-110">id</span></span>|<span data-ttu-id="36af7-111">String</span><span class="sxs-lookup"><span data-stu-id="36af7-111">String</span></span>|<span data-ttu-id="36af7-112">Объектный ID пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="36af7-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="36af7-113">authenticationMode</span><span class="sxs-lookup"><span data-stu-id="36af7-113">authenticationMode</span></span>|<span data-ttu-id="36af7-114">MicrosoftAuthenticatorAuthenticationMode</span><span class="sxs-lookup"><span data-stu-id="36af7-114">microsoftAuthenticatorAuthenticationMode</span></span>|<span data-ttu-id="36af7-115">Определяет, какие типы уведомлений можно использовать для регистрации.</span><span class="sxs-lookup"><span data-stu-id="36af7-115">Determines which types of notifications can be used for sign-in.</span></span> <span data-ttu-id="36af7-116">Возможные значения: `any` , `deviceBasedPush` (только без паролей), `push` .</span><span class="sxs-lookup"><span data-stu-id="36af7-116">Possible values are: `any`, `deviceBasedPush` (passwordless only), `push`.</span></span>|
|<span data-ttu-id="36af7-117">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="36af7-117">isRegistrationRequired</span></span>|<span data-ttu-id="36af7-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="36af7-118">Boolean</span></span>|<span data-ttu-id="36af7-119">Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="36af7-119">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="36af7-120">*Не поддерживается.*</span><span class="sxs-lookup"><span data-stu-id="36af7-120">*Not supported*.</span></span> |
|<span data-ttu-id="36af7-121">numberMatchingRequiredState</span><span class="sxs-lookup"><span data-stu-id="36af7-121">numberMatchingRequiredState</span></span>|<span data-ttu-id="36af7-122">advancedConfigState</span><span class="sxs-lookup"><span data-stu-id="36af7-122">advancedConfigState</span></span>|<span data-ttu-id="36af7-123">Требуется совпадение номеров для уведомлений MFA.</span><span class="sxs-lookup"><span data-stu-id="36af7-123">Requires number matching for MFA notifications.</span></span> <span data-ttu-id="36af7-124">Значение игнорируется для уведомлений о входе в телефон.</span><span class="sxs-lookup"><span data-stu-id="36af7-124">Value is ignored for phone sign-in notifications.</span></span> <span data-ttu-id="36af7-125">Возможные значения: `enabled`, `disabled`, `default`.</span><span class="sxs-lookup"><span data-stu-id="36af7-125">Possible values are: `enabled`, `disabled`, `default`.</span></span>|
|<span data-ttu-id="36af7-126">displayLocationInformationRequiredState</span><span class="sxs-lookup"><span data-stu-id="36af7-126">displayLocationInformationRequiredState</span></span>|<span data-ttu-id="36af7-127">advancedConfigState</span><span class="sxs-lookup"><span data-stu-id="36af7-127">advancedConfigState</span></span>|<span data-ttu-id="36af7-128">Определяет, следует ли показывать пользователю расположение входной записи в теле уведомления.</span><span class="sxs-lookup"><span data-stu-id="36af7-128">Determines whether the location of the sign-in should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="36af7-129">Возможные значения: `enabled`, `disabled`, `default`.</span><span class="sxs-lookup"><span data-stu-id="36af7-129">Possible values are: `enabled`, `disabled`, `default`.</span></span>|
|<span data-ttu-id="36af7-130">displayAppInformationRequiredState</span><span class="sxs-lookup"><span data-stu-id="36af7-130">displayAppInformationRequiredState</span></span>|<span data-ttu-id="36af7-131">advancedConfigState</span><span class="sxs-lookup"><span data-stu-id="36af7-131">advancedConfigState</span></span>|<span data-ttu-id="36af7-132">Определяет, следует ли показывать пользователю приложение, в которое подписывает пользователь, в теле уведомления.</span><span class="sxs-lookup"><span data-stu-id="36af7-132">Determines whether the app the user is signing into should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="36af7-133">Возможные значения: `enabled`, `disabled`, `default`.</span><span class="sxs-lookup"><span data-stu-id="36af7-133">Possible values are: `enabled`, `disabled`, `default`.</span></span>|
|<span data-ttu-id="36af7-134">targetType</span><span class="sxs-lookup"><span data-stu-id="36af7-134">targetType</span></span>|<span data-ttu-id="36af7-135">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="36af7-135">authenticationMethodTargetType</span></span>| <span data-ttu-id="36af7-136">Возможные значения: `null`, `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="36af7-136">Possible values are: `null`, `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36af7-137">Связи</span><span class="sxs-lookup"><span data-stu-id="36af7-137">Relationships</span></span>
<span data-ttu-id="36af7-138">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="36af7-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="36af7-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="36af7-139">JSON representation</span></span>
<span data-ttu-id="36af7-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36af7-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "targetType": "String",
  "id": "String (identifier)",
  "isRegistrationRequired": "Boolean",
  "authenticationMode": "String",
  "numberMatchingRequiredState": "String",
  "displayLocationInformationRequiredState": "String",
  "displayAppInformationRequiredState": "String"
}

```
