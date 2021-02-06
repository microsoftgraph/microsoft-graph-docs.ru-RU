---
title: Тип ресурса passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, которые могут использовать политику проверки подлинности на телефоне без пароля Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d3dd874b96a54dc7e764200800e85b445abd50ee
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137657"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodtarget-resource-type-deprecated"></a><span data-ttu-id="95023-103">Тип ресурса passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget (неподготовлен)</span><span class="sxs-lookup"><span data-stu-id="95023-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget resource type (deprecated)</span></span>

<span data-ttu-id="95023-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95023-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95023-105">Коллекция пользователей или групп, которые могут использовать политику проверки подлинности на телефоне без пароля Microsoft Authenticator](.. /resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="95023-105">A collection of users or groups enabled to use Microsoft Authenticator Passwordless Phone Sign-in authentication methods policy](../resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

> [!CAUTION]
> <span data-ttu-id="95023-106">API политики проверки подлинности для телефона без пароля Microsoft Authenticator является неподготовленным и больше не возвращает результаты 31 декабря 2020 г.</span><span class="sxs-lookup"><span data-stu-id="95023-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="95023-107">Используйте новую политику метода [проверки подлинности Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95023-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="95023-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="95023-108">Properties</span></span>
|<span data-ttu-id="95023-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="95023-109">Property</span></span>|<span data-ttu-id="95023-110">Тип</span><span class="sxs-lookup"><span data-stu-id="95023-110">Type</span></span>|<span data-ttu-id="95023-111">Описание</span><span class="sxs-lookup"><span data-stu-id="95023-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95023-112">id</span><span class="sxs-lookup"><span data-stu-id="95023-112">id</span></span>|<span data-ttu-id="95023-113">Строка</span><span class="sxs-lookup"><span data-stu-id="95023-113">String</span></span>|<span data-ttu-id="95023-114">ИД объекта пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="95023-114">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="95023-115">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="95023-115">isRegistrationRequired</span></span>|<span data-ttu-id="95023-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="95023-116">Boolean</span></span>|<span data-ttu-id="95023-117">Определяет, должен ли пользователь принудительно регистрировать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="95023-117">Determines whether the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="95023-118">shownContext</span><span class="sxs-lookup"><span data-stu-id="95023-118">shownContext</span></span>|<span data-ttu-id="95023-119">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="95023-119">authenticatorAppContextType</span></span>|<span data-ttu-id="95023-120">Возможные значения: `location`, `app`.</span><span class="sxs-lookup"><span data-stu-id="95023-120">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="95023-121">targetType</span><span class="sxs-lookup"><span data-stu-id="95023-121">targetType</span></span>|<span data-ttu-id="95023-122">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="95023-122">authenticationMethodTargetType</span></span>|<span data-ttu-id="95023-123">Возможные значения: `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="95023-123">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="95023-124">useForSignIn</span><span class="sxs-lookup"><span data-stu-id="95023-124">useForSignIn</span></span>|<span data-ttu-id="95023-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="95023-125">Boolean</span></span>|<span data-ttu-id="95023-126">Определяет, можно ли использовать метод проверки подлинности для входов в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="95023-126">Determines whether the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95023-127">Связи</span><span class="sxs-lookup"><span data-stu-id="95023-127">Relationships</span></span>
<span data-ttu-id="95023-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="95023-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="95023-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="95023-129">JSON representation</span></span>
<span data-ttu-id="95023-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95023-130">The following is a JSON representation of the resource.</span></span>
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
