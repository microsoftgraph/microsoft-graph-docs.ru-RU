---
title: Тип ресурса microsoftAuthenticatorAuthenticationMethodTarget
description: Коллекция пользователей или групп, которые могут использовать политику методов проверки подлинности Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f2107ff1bde5fb34b541565e828ca91247803598
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131341"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="d47be-103">Тип ресурса microsoftAuthenticatorAuthenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="d47be-103">microsoftAuthenticatorAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="d47be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d47be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d47be-105">Коллекция пользователей или групп, которые могут использовать политику методов проверки подлинности [Microsoft Authenticator](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d47be-105">A collection of users or groups enabled to use [Microsoft Authenticator authentication methods policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="d47be-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d47be-106">Properties</span></span>
|<span data-ttu-id="d47be-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d47be-107">Property</span></span>|<span data-ttu-id="d47be-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d47be-108">Type</span></span>|<span data-ttu-id="d47be-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d47be-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d47be-110">id</span><span class="sxs-lookup"><span data-stu-id="d47be-110">id</span></span>|<span data-ttu-id="d47be-111">Строка</span><span class="sxs-lookup"><span data-stu-id="d47be-111">String</span></span>|<span data-ttu-id="d47be-112">ИД объекта пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d47be-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="d47be-113">isNumberMatchingRequired (Private Preview)</span><span class="sxs-lookup"><span data-stu-id="d47be-113">isNumberMatchingRequired (Private Preview)</span></span>|<span data-ttu-id="d47be-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="d47be-114">Boolean</span></span>|<span data-ttu-id="d47be-115">Требовать от пользователя совпадения номера, отображаемого на странице для регистрации, чтобы утвердить уведомление MFA.</span><span class="sxs-lookup"><span data-stu-id="d47be-115">Require the user to match the number displayed on the sign-in page to approve the MFA notification.</span></span>|
|<span data-ttu-id="d47be-116">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="d47be-116">isRegistrationRequired</span></span>|<span data-ttu-id="d47be-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="d47be-117">Boolean</span></span>|<span data-ttu-id="d47be-118">Определяет, должен ли пользователь принудительно регистрировать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d47be-118">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="d47be-119">*Не поддерживается.*</span><span class="sxs-lookup"><span data-stu-id="d47be-119">*Not supported*.</span></span> |
|<span data-ttu-id="d47be-120">shownContext (Private Preview)</span><span class="sxs-lookup"><span data-stu-id="d47be-120">shownContext (Private Preview)</span></span>|<span data-ttu-id="d47be-121">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="d47be-121">authenticatorAppContextType</span></span>|<span data-ttu-id="d47be-122">Определяет, какие типы контекста о входе должны быть показаны пользователю в теле уведомления.</span><span class="sxs-lookup"><span data-stu-id="d47be-122">Determines what types of context about the sign-in should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="d47be-123">Возможные значения: `location`, `app`.</span><span class="sxs-lookup"><span data-stu-id="d47be-123">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="d47be-124">targetType</span><span class="sxs-lookup"><span data-stu-id="d47be-124">targetType</span></span>|<span data-ttu-id="d47be-125">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="d47be-125">authenticationMethodTargetType</span></span>| <span data-ttu-id="d47be-126">Возможные значения: `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="d47be-126">Possible values are: `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d47be-127">Связи</span><span class="sxs-lookup"><span data-stu-id="d47be-127">Relationships</span></span>
<span data-ttu-id="d47be-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d47be-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d47be-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d47be-129">JSON representation</span></span>
<span data-ttu-id="d47be-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d47be-130">The following is a JSON representation of the resource.</span></span>
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

