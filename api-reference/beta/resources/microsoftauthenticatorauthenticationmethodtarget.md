---
title: Тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, которые могут использовать политику методов проверки подлинности Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a8eb9959faaf5f4a6bcaecceb165384be737623d
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292275"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="30978-103">Тип ресурса microsoftAuthenticatorAuthenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="30978-103">microsoftAuthenticatorAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="30978-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30978-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30978-105">Коллекция пользователей или групп, которые могут использовать политику методов проверки подлинности [Microsoft Authenticator](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="30978-105">A collection of users or groups enabled to use [Microsoft Authenticator authentication methods policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="30978-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="30978-106">Properties</span></span>
|<span data-ttu-id="30978-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="30978-107">Property</span></span>|<span data-ttu-id="30978-108">Тип</span><span class="sxs-lookup"><span data-stu-id="30978-108">Type</span></span>|<span data-ttu-id="30978-109">Описание</span><span class="sxs-lookup"><span data-stu-id="30978-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30978-110">id</span><span class="sxs-lookup"><span data-stu-id="30978-110">id</span></span>|<span data-ttu-id="30978-111">String</span><span class="sxs-lookup"><span data-stu-id="30978-111">String</span></span>|<span data-ttu-id="30978-112">ИД объекта пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="30978-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="30978-113">isNumberMatchingRequired (private Preview)</span><span class="sxs-lookup"><span data-stu-id="30978-113">isNumberMatchingRequired (Private Preview)</span></span>|<span data-ttu-id="30978-114">Логический</span><span class="sxs-lookup"><span data-stu-id="30978-114">Boolean</span></span>|<span data-ttu-id="30978-115">Требовать от пользователя совпадения номера, отображаемого на странице для регистрации, чтобы утвердить уведомление MFA.</span><span class="sxs-lookup"><span data-stu-id="30978-115">Require the user to match the number displayed on the sign-in page to approve the MFA notification.</span></span>|
|<span data-ttu-id="30978-116">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="30978-116">isRegistrationRequired</span></span>|<span data-ttu-id="30978-117">Логический</span><span class="sxs-lookup"><span data-stu-id="30978-117">Boolean</span></span>|<span data-ttu-id="30978-118">Определяет, должен ли пользователь принудительно регистрировать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="30978-118">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="30978-119">*Не поддерживается.*</span><span class="sxs-lookup"><span data-stu-id="30978-119">*Not supported*.</span></span> |
|<span data-ttu-id="30978-120">shownContext (Private Preview)</span><span class="sxs-lookup"><span data-stu-id="30978-120">shownContext (Private Preview)</span></span>|<span data-ttu-id="30978-121">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="30978-121">authenticatorAppContextType</span></span>|<span data-ttu-id="30978-122">Определяет, какие типы контекста о входе должны показываться пользователю в теле уведомления.</span><span class="sxs-lookup"><span data-stu-id="30978-122">Determines what types of context about the sign-in should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="30978-123">Возможные значения: `location`, `app`.</span><span class="sxs-lookup"><span data-stu-id="30978-123">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="30978-124">targetType</span><span class="sxs-lookup"><span data-stu-id="30978-124">targetType</span></span>|<span data-ttu-id="30978-125">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="30978-125">authenticationMethodTargetType</span></span>| <span data-ttu-id="30978-126">Возможные значения: `null`, `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="30978-126">Possible values are: `null`, `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30978-127">Связи</span><span class="sxs-lookup"><span data-stu-id="30978-127">Relationships</span></span>
<span data-ttu-id="30978-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="30978-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="30978-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="30978-129">JSON representation</span></span>
<span data-ttu-id="30978-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30978-130">The following is a JSON representation of the resource.</span></span>
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
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean",
  "shownContext": "String",
  "isNumberMatchingRequired": "Boolean"
}
```

