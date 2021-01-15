---
title: Тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, которые могут использовать политику методов проверки подлинности Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 395a1a10d9d99ce8ea5475e09a2e082b3bc5ddf3
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874496"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="821e4-103">Тип ресурса microsoftAuthenticatorAuthenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="821e4-103">microsoftAuthenticatorAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="821e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="821e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="821e4-105">Коллекция пользователей или групп, которые могут использовать политику методов проверки подлинности [Microsoft Authenticator](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="821e4-105">A collection of users or groups enabled to use [Microsoft Authenticator authentication methods policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="821e4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="821e4-106">Properties</span></span>
|<span data-ttu-id="821e4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="821e4-107">Property</span></span>|<span data-ttu-id="821e4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="821e4-108">Type</span></span>|<span data-ttu-id="821e4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="821e4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="821e4-110">id</span><span class="sxs-lookup"><span data-stu-id="821e4-110">id</span></span>|<span data-ttu-id="821e4-111">String</span><span class="sxs-lookup"><span data-stu-id="821e4-111">String</span></span>|<span data-ttu-id="821e4-112">ИД объекта пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="821e4-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="821e4-113">isNumberMatchingRequired (Private Preview)</span><span class="sxs-lookup"><span data-stu-id="821e4-113">isNumberMatchingRequired (Private Preview)</span></span>|<span data-ttu-id="821e4-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="821e4-114">Boolean</span></span>|<span data-ttu-id="821e4-115">Требовать от пользователя совпадения номера, отображаемого на странице для регистрации, чтобы утвердить уведомление MFA.</span><span class="sxs-lookup"><span data-stu-id="821e4-115">Require the user to match the number displayed on the sign-in page to approve the MFA notification.</span></span>|
|<span data-ttu-id="821e4-116">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="821e4-116">isRegistrationRequired</span></span>|<span data-ttu-id="821e4-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="821e4-117">Boolean</span></span>|<span data-ttu-id="821e4-118">Определяет, должен ли пользователь принудительно регистрировать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="821e4-118">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="821e4-119">*Не поддерживается.*</span><span class="sxs-lookup"><span data-stu-id="821e4-119">*Not supported*.</span></span> |
|<span data-ttu-id="821e4-120">shownContext (Private Preview)</span><span class="sxs-lookup"><span data-stu-id="821e4-120">shownContext (Private Preview)</span></span>|<span data-ttu-id="821e4-121">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="821e4-121">authenticatorAppContextType</span></span>|<span data-ttu-id="821e4-122">Определяет, какие типы контекста о входе должны быть показаны пользователю в теле уведомления.</span><span class="sxs-lookup"><span data-stu-id="821e4-122">Determines what types of context about the sign-in should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="821e4-123">Возможные значения: `location`, `app`.</span><span class="sxs-lookup"><span data-stu-id="821e4-123">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="821e4-124">targetType</span><span class="sxs-lookup"><span data-stu-id="821e4-124">targetType</span></span>|<span data-ttu-id="821e4-125">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="821e4-125">authenticationMethodTargetType</span></span>| <span data-ttu-id="821e4-126">Возможные значения: `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="821e4-126">Possible values are: `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="821e4-127">Связи</span><span class="sxs-lookup"><span data-stu-id="821e4-127">Relationships</span></span>
<span data-ttu-id="821e4-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="821e4-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="821e4-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="821e4-129">JSON representation</span></span>
<span data-ttu-id="821e4-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="821e4-130">The following is a JSON representation of the resource.</span></span>
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

