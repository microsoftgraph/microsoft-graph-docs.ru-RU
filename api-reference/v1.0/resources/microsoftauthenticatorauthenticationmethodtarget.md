---
title: тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, включенная для использования политики методов проверки подлинности Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 233eed9e49ca25fafbdebc0097b513122bdb9a4b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964935"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="1e200-103">тип ресурса microsoftAuthenticatorAuthenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="1e200-103">microsoftAuthenticatorAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="1e200-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e200-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1e200-105">Коллекция пользователей или групп, включенная для использования политики методов проверки подлинности [Microsoft Authenticator](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1e200-105">A collection of users or groups enabled to use [Microsoft Authenticator authentication methods policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="1e200-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e200-106">Properties</span></span>
|<span data-ttu-id="1e200-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e200-107">Property</span></span>|<span data-ttu-id="1e200-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1e200-108">Type</span></span>|<span data-ttu-id="1e200-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1e200-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e200-110">id</span><span class="sxs-lookup"><span data-stu-id="1e200-110">id</span></span>|<span data-ttu-id="1e200-111">String</span><span class="sxs-lookup"><span data-stu-id="1e200-111">String</span></span>|<span data-ttu-id="1e200-112">Объектный ID пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1e200-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="1e200-113">authenticationMode</span><span class="sxs-lookup"><span data-stu-id="1e200-113">authenticationMode</span></span>|<span data-ttu-id="1e200-114">MicrosoftAuthenticatorAuthenticationMode</span><span class="sxs-lookup"><span data-stu-id="1e200-114">microsoftAuthenticatorAuthenticationMode</span></span>|<span data-ttu-id="1e200-115">Определяет, какие типы уведомлений можно использовать для регистрации.</span><span class="sxs-lookup"><span data-stu-id="1e200-115">Determines which types of notifications can be used for sign-in.</span></span> <span data-ttu-id="1e200-116">Возможные значения: `any` , `deviceBasedPush` (только без паролей), `push` .</span><span class="sxs-lookup"><span data-stu-id="1e200-116">Possible values are: `any`, `deviceBasedPush` (passwordless only), `push`.</span></span>|
|<span data-ttu-id="1e200-117">featureSettings</span><span class="sxs-lookup"><span data-stu-id="1e200-117">featureSettings</span></span>|<span data-ttu-id="1e200-118">authenticatorAppFeatureSettings</span><span class="sxs-lookup"><span data-stu-id="1e200-118">authenticatorAppFeatureSettings</span></span>|<span data-ttu-id="1e200-119">Определяет, какие дополнительные параметры следует применить к Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="1e200-119">Determines what additional settings should be applied to Microsoft Authenticator.</span></span> <span data-ttu-id="1e200-120">Возможные значения: `null` , `requireNumberMatching` (Требуется совпадение номеров для уведомлений MFA.</span><span class="sxs-lookup"><span data-stu-id="1e200-120">Possible values are: `null`, `requireNumberMatching` (Requires number matching for MFA notifications.</span></span> <span data-ttu-id="1e200-121">Значение игнорируется для уведомлений о входе в телефон).</span><span class="sxs-lookup"><span data-stu-id="1e200-121">Value is ignored for phone sign-in notifications).</span></span>|
|<span data-ttu-id="1e200-122">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="1e200-122">isRegistrationRequired</span></span>|<span data-ttu-id="1e200-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e200-123">Boolean</span></span>|<span data-ttu-id="1e200-124">Определяет, принудит ли пользователь зарегистрировать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="1e200-124">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="1e200-125">*Не поддерживается.*</span><span class="sxs-lookup"><span data-stu-id="1e200-125">*Not supported*.</span></span> |
|<span data-ttu-id="1e200-126">shownContext</span><span class="sxs-lookup"><span data-stu-id="1e200-126">shownContext</span></span>|<span data-ttu-id="1e200-127">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="1e200-127">authenticatorAppContextType</span></span>|<span data-ttu-id="1e200-128">(Частный предварительный просмотр) Определяет, какие типы контекста о входе должны быть показаны пользователю в теле уведомления.</span><span class="sxs-lookup"><span data-stu-id="1e200-128">(Private Preview) Determines what types of context about the sign-in should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="1e200-129">Возможные значения: `location`, `app`.</span><span class="sxs-lookup"><span data-stu-id="1e200-129">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="1e200-130">targetType</span><span class="sxs-lookup"><span data-stu-id="1e200-130">targetType</span></span>|<span data-ttu-id="1e200-131">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="1e200-131">authenticationMethodTargetType</span></span>| <span data-ttu-id="1e200-132">Возможные значения: `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="1e200-132">Possible values are: `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e200-133">Связи</span><span class="sxs-lookup"><span data-stu-id="1e200-133">Relationships</span></span>
<span data-ttu-id="1e200-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1e200-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e200-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1e200-135">JSON representation</span></span>
<span data-ttu-id="1e200-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e200-136">The following is a JSON representation of the resource.</span></span>
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
