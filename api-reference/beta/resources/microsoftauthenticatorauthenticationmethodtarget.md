---
title: тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, включенная для использования политики методов проверки подлинности Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: db612bd2ac7aec387574fe1e45c967e2525c2b12
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960392"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="09ce9-103">тип ресурса microsoftAuthenticatorAuthenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="09ce9-103">microsoftAuthenticatorAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="09ce9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09ce9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09ce9-105">Коллекция пользователей или групп, включенная для использования политики методов проверки подлинности [Microsoft Authenticator](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="09ce9-105">A collection of users or groups enabled to use [Microsoft Authenticator authentication methods policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="09ce9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="09ce9-106">Properties</span></span>
|<span data-ttu-id="09ce9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="09ce9-107">Property</span></span>|<span data-ttu-id="09ce9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="09ce9-108">Type</span></span>|<span data-ttu-id="09ce9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="09ce9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09ce9-110">id</span><span class="sxs-lookup"><span data-stu-id="09ce9-110">id</span></span>|<span data-ttu-id="09ce9-111">Строка</span><span class="sxs-lookup"><span data-stu-id="09ce9-111">String</span></span>|<span data-ttu-id="09ce9-112">Объектный ID пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="09ce9-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="09ce9-113">authenticationMode</span><span class="sxs-lookup"><span data-stu-id="09ce9-113">authenticationMode</span></span>|<span data-ttu-id="09ce9-114">MicrosoftAuthenticatorAuthenticationMode</span><span class="sxs-lookup"><span data-stu-id="09ce9-114">microsoftAuthenticatorAuthenticationMode</span></span>|<span data-ttu-id="09ce9-115">Определяет, какие типы уведомлений можно использовать для регистрации.</span><span class="sxs-lookup"><span data-stu-id="09ce9-115">Determines which types of notifications can be used for sign-in.</span></span> <span data-ttu-id="09ce9-116">Возможные значения: `any` , `deviceBasedPush` (только без паролей), `push` .</span><span class="sxs-lookup"><span data-stu-id="09ce9-116">Possible values are: `any`, `deviceBasedPush` (passwordless only), `push`.</span></span>|
|<span data-ttu-id="09ce9-117">featureSettings</span><span class="sxs-lookup"><span data-stu-id="09ce9-117">featureSettings</span></span>|<span data-ttu-id="09ce9-118">authenticatorAppFeatureSettings</span><span class="sxs-lookup"><span data-stu-id="09ce9-118">authenticatorAppFeatureSettings</span></span>|<span data-ttu-id="09ce9-119">Определяет, какие дополнительные параметры следует применить к Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="09ce9-119">Determines what additional settings should be applied to Microsoft Authenticator.</span></span> <span data-ttu-id="09ce9-120">Возможные значения: `null` , `requireNumberMatching` (Требуется совпадение номеров для уведомлений MFA.</span><span class="sxs-lookup"><span data-stu-id="09ce9-120">Possible values are: `null`, `requireNumberMatching` (Requires number matching for MFA notifications.</span></span> <span data-ttu-id="09ce9-121">Значение игнорируется для уведомлений о входе в телефон).</span><span class="sxs-lookup"><span data-stu-id="09ce9-121">Value is ignored for phone sign-in notifications).</span></span>|
|<span data-ttu-id="09ce9-122">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="09ce9-122">isRegistrationRequired</span></span>|<span data-ttu-id="09ce9-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="09ce9-123">Boolean</span></span>|<span data-ttu-id="09ce9-124">Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="09ce9-124">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="09ce9-125">*Не поддерживается.*</span><span class="sxs-lookup"><span data-stu-id="09ce9-125">*Not supported*.</span></span> |
|<span data-ttu-id="09ce9-126">shownContext (Private Preview)</span><span class="sxs-lookup"><span data-stu-id="09ce9-126">shownContext (Private Preview)</span></span>|<span data-ttu-id="09ce9-127">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="09ce9-127">authenticatorAppContextType</span></span>|<span data-ttu-id="09ce9-128">Определяет, какие типы контекста о входе должны быть показаны пользователю в теле уведомления.</span><span class="sxs-lookup"><span data-stu-id="09ce9-128">Determines what types of context about the sign-in should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="09ce9-129">Возможные значения: `location`, `app`.</span><span class="sxs-lookup"><span data-stu-id="09ce9-129">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="09ce9-130">targetType</span><span class="sxs-lookup"><span data-stu-id="09ce9-130">targetType</span></span>|<span data-ttu-id="09ce9-131">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="09ce9-131">authenticationMethodTargetType</span></span>| <span data-ttu-id="09ce9-132">Возможные значения: `null`, `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="09ce9-132">Possible values are: `null`, `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09ce9-133">Связи</span><span class="sxs-lookup"><span data-stu-id="09ce9-133">Relationships</span></span>
<span data-ttu-id="09ce9-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="09ce9-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="09ce9-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="09ce9-135">JSON representation</span></span>
<span data-ttu-id="09ce9-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09ce9-136">The following is a JSON representation of the resource.</span></span>
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
  "shownContext": "String",
  "featureSettings": "String"
}

```
