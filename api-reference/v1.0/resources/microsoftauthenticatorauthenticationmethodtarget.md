---
title: тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, включенная для использования политики методов проверки подлинности Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 43c8e5a4ba92e838a64ec5f345ae82c744b53dee
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469250"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="8f1b1-103">тип ресурса microsoftAuthenticatorAuthenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="8f1b1-103">microsoftAuthenticatorAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="8f1b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f1b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f1b1-105">Коллекция пользователей или групп, включенная для использования политики методов проверки подлинности [Microsoft Authenticator](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8f1b1-105">A collection of users or groups enabled to use [Microsoft Authenticator authentication methods policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="8f1b1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f1b1-106">Properties</span></span>
|<span data-ttu-id="8f1b1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f1b1-107">Property</span></span>|<span data-ttu-id="8f1b1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8f1b1-108">Type</span></span>|<span data-ttu-id="8f1b1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8f1b1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f1b1-110">id</span><span class="sxs-lookup"><span data-stu-id="8f1b1-110">id</span></span>|<span data-ttu-id="8f1b1-111">String</span><span class="sxs-lookup"><span data-stu-id="8f1b1-111">String</span></span>|<span data-ttu-id="8f1b1-112">Объектный ID пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8f1b1-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="8f1b1-113">authenticationMode</span><span class="sxs-lookup"><span data-stu-id="8f1b1-113">authenticationMode</span></span>|<span data-ttu-id="8f1b1-114">MicrosoftAuthenticatorAuthenticationMode</span><span class="sxs-lookup"><span data-stu-id="8f1b1-114">microsoftAuthenticatorAuthenticationMode</span></span>|<span data-ttu-id="8f1b1-115">Определяет, какие типы уведомлений можно использовать для регистрации.</span><span class="sxs-lookup"><span data-stu-id="8f1b1-115">Determines which types of notifications can be used for sign-in.</span></span> <span data-ttu-id="8f1b1-116">Возможные значения: `any` , `deviceBasedPush` (только без паролей), `push` .</span><span class="sxs-lookup"><span data-stu-id="8f1b1-116">Possible values are: `any`, `deviceBasedPush` (passwordless only), `push`.</span></span>|
|<span data-ttu-id="8f1b1-117">featureSettings</span><span class="sxs-lookup"><span data-stu-id="8f1b1-117">featureSettings</span></span>|<span data-ttu-id="8f1b1-118">authenticatorAppFeatureSettings</span><span class="sxs-lookup"><span data-stu-id="8f1b1-118">authenticatorAppFeatureSettings</span></span>|<span data-ttu-id="8f1b1-119">Определяет, какие дополнительные параметры следует применить к Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="8f1b1-119">Determines what additional settings should be applied to Microsoft Authenticator.</span></span> <span data-ttu-id="8f1b1-120">Возможные значения: `null` , `requireNumberMatching` (Требуется совпадение номеров для уведомлений MFA.</span><span class="sxs-lookup"><span data-stu-id="8f1b1-120">Possible values are: `null`, `requireNumberMatching` (Requires number matching for MFA notifications.</span></span> <span data-ttu-id="8f1b1-121">Значение игнорируется для уведомлений о входе в телефон).</span><span class="sxs-lookup"><span data-stu-id="8f1b1-121">Value is ignored for phone sign-in notifications).</span></span>|
|<span data-ttu-id="8f1b1-122">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="8f1b1-122">isRegistrationRequired</span></span>|<span data-ttu-id="8f1b1-123">Логический</span><span class="sxs-lookup"><span data-stu-id="8f1b1-123">Boolean</span></span>|<span data-ttu-id="8f1b1-124">Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="8f1b1-124">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="8f1b1-125">*Не поддерживается.*</span><span class="sxs-lookup"><span data-stu-id="8f1b1-125">*Not supported*.</span></span> |
|<span data-ttu-id="8f1b1-126">shownContext</span><span class="sxs-lookup"><span data-stu-id="8f1b1-126">shownContext</span></span>|<span data-ttu-id="8f1b1-127">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="8f1b1-127">authenticatorAppContextType</span></span>|<span data-ttu-id="8f1b1-128">(Частный предварительный просмотр) Определяет, какие типы контекста о входе должны быть показаны пользователю в теле уведомления.</span><span class="sxs-lookup"><span data-stu-id="8f1b1-128">(Private Preview) Determines what types of context about the sign-in should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="8f1b1-129">Возможные значения: `location`, `app`.</span><span class="sxs-lookup"><span data-stu-id="8f1b1-129">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="8f1b1-130">targetType</span><span class="sxs-lookup"><span data-stu-id="8f1b1-130">targetType</span></span>|<span data-ttu-id="8f1b1-131">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="8f1b1-131">authenticationMethodTargetType</span></span>| <span data-ttu-id="8f1b1-132">Возможные значения: `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="8f1b1-132">Possible values are: `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f1b1-133">Связи</span><span class="sxs-lookup"><span data-stu-id="8f1b1-133">Relationships</span></span>
<span data-ttu-id="8f1b1-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8f1b1-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f1b1-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8f1b1-135">JSON representation</span></span>
<span data-ttu-id="8f1b1-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f1b1-136">The following is a JSON representation of the resource.</span></span>
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
