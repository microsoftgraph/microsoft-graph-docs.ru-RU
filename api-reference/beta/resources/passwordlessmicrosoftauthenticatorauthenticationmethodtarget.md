---
title: Тип ресурса passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, которые могут использовать политику проверки подлинности на телефоне без пароля Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef62b251d6c943bd6290a07fa2b018bddca81ab5
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872270"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodtarget-resource-type-deprecated"></a><span data-ttu-id="bb21d-103">Тип ресурса passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget (неподготовлен)</span><span class="sxs-lookup"><span data-stu-id="bb21d-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget resource type (deprecated)</span></span>

<span data-ttu-id="bb21d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb21d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb21d-105">Коллекция пользователей или групп, которые могут использовать политику проверки подлинности на телефоне без пароля Microsoft Authenticator](.. /resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bb21d-105">A collection of users or groups enabled to use Microsoft Authenticator Passwordless Phone Sign-in authentication methods policy](../resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

> [!CAUTION]
> <span data-ttu-id="bb21d-106">API политики проверки подлинности для телефона без пароля Microsoft Authenticator является неподготовленным и больше не возвращает результаты 31 декабря 2020 г.</span><span class="sxs-lookup"><span data-stu-id="bb21d-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="bb21d-107">Используйте новую политику метода [проверки подлинности Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb21d-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bb21d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb21d-108">Properties</span></span>
|<span data-ttu-id="bb21d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb21d-109">Property</span></span>|<span data-ttu-id="bb21d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bb21d-110">Type</span></span>|<span data-ttu-id="bb21d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bb21d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb21d-112">id</span><span class="sxs-lookup"><span data-stu-id="bb21d-112">id</span></span>|<span data-ttu-id="bb21d-113">String</span><span class="sxs-lookup"><span data-stu-id="bb21d-113">String</span></span>|<span data-ttu-id="bb21d-114">ИД объекта пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bb21d-114">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="bb21d-115">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="bb21d-115">isRegistrationRequired</span></span>|<span data-ttu-id="bb21d-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb21d-116">Boolean</span></span>|<span data-ttu-id="bb21d-117">Определяет, должен ли пользователь принудительно регистрировать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="bb21d-117">Determines whether the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="bb21d-118">shownContext</span><span class="sxs-lookup"><span data-stu-id="bb21d-118">shownContext</span></span>|<span data-ttu-id="bb21d-119">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="bb21d-119">authenticatorAppContextType</span></span>|<span data-ttu-id="bb21d-120">Возможные значения: `location`, `app`.</span><span class="sxs-lookup"><span data-stu-id="bb21d-120">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="bb21d-121">targetType</span><span class="sxs-lookup"><span data-stu-id="bb21d-121">targetType</span></span>|<span data-ttu-id="bb21d-122">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="bb21d-122">authenticationMethodTargetType</span></span>|<span data-ttu-id="bb21d-123">Возможные значения: `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="bb21d-123">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="bb21d-124">useForSignIn</span><span class="sxs-lookup"><span data-stu-id="bb21d-124">useForSignIn</span></span>|<span data-ttu-id="bb21d-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb21d-125">Boolean</span></span>|<span data-ttu-id="bb21d-126">Определяет, можно ли использовать метод проверки подлинности для входов в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bb21d-126">Determines whether the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb21d-127">Связи</span><span class="sxs-lookup"><span data-stu-id="bb21d-127">Relationships</span></span>
<span data-ttu-id="bb21d-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bb21d-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb21d-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bb21d-129">JSON representation</span></span>
<span data-ttu-id="bb21d-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb21d-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean",
  "shownContext": "String"
}
```
