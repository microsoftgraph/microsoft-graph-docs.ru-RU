---
title: Тип ресурса Пассвордлессмикрософтаусентикатораусентикатионмесодтаржет
description: Коллекция пользователей или групп, для которых используется политика методов проверки подлинности при входе в систему без пароля.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a26a8fe76da954d3dc44a238665954539df0fa72
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418482"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="4086b-103">Тип ресурса Пассвордлессмикрософтаусентикатораусентикатионмесодтаржет</span><span class="sxs-lookup"><span data-stu-id="4086b-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget resource type</span></span>

<span data-ttu-id="4086b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4086b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4086b-105">Набор пользователей или групп, для которых используется политика проверки подлинности входа на телефон, не поддерживающий пароль для проверки подлинности (Майкрософт). /Ресаурцес/пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион.МД) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4086b-105">A collection of users or groups enabled to use Microsoft Authenticator Passwordless Phone Sign-in authentication methods policy](../resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

> [!NOTE]
> <span data-ttu-id="4086b-106">Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии.</span><span class="sxs-lookup"><span data-stu-id="4086b-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="4086b-107">Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.</span><span class="sxs-lookup"><span data-stu-id="4086b-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="properties"></a><span data-ttu-id="4086b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4086b-108">Properties</span></span>
|<span data-ttu-id="4086b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4086b-109">Property</span></span>|<span data-ttu-id="4086b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4086b-110">Type</span></span>|<span data-ttu-id="4086b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4086b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4086b-112">id</span><span class="sxs-lookup"><span data-stu-id="4086b-112">id</span></span>|<span data-ttu-id="4086b-113">String</span><span class="sxs-lookup"><span data-stu-id="4086b-113">String</span></span>|<span data-ttu-id="4086b-114">Идентификатор объекта пользователя или группы Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4086b-114">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="4086b-115">исрегистратионрекуиред</span><span class="sxs-lookup"><span data-stu-id="4086b-115">isRegistrationRequired</span></span>|<span data-ttu-id="4086b-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="4086b-116">Boolean</span></span>|<span data-ttu-id="4086b-117">Определяет, применяется ли пользователь для регистрации метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="4086b-117">Determines whether the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="4086b-118">шовнконтекст</span><span class="sxs-lookup"><span data-stu-id="4086b-118">shownContext</span></span>|<span data-ttu-id="4086b-119">аусентикатораппконтексттипе</span><span class="sxs-lookup"><span data-stu-id="4086b-119">authenticatorAppContextType</span></span>|<span data-ttu-id="4086b-120">Возможные значения: `location`, `app`.</span><span class="sxs-lookup"><span data-stu-id="4086b-120">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="4086b-121">targetType</span><span class="sxs-lookup"><span data-stu-id="4086b-121">targetType</span></span>|<span data-ttu-id="4086b-122">аусентикатионмесодтаржеттипе</span><span class="sxs-lookup"><span data-stu-id="4086b-122">authenticationMethodTargetType</span></span>|<span data-ttu-id="4086b-123">Возможные значения: `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="4086b-123">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="4086b-124">усефорсигнин</span><span class="sxs-lookup"><span data-stu-id="4086b-124">useForSignIn</span></span>|<span data-ttu-id="4086b-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="4086b-125">Boolean</span></span>|<span data-ttu-id="4086b-126">Определяет, можно ли использовать метод проверки подлинности для входа в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4086b-126">Determines whether the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4086b-127">Связи</span><span class="sxs-lookup"><span data-stu-id="4086b-127">Relationships</span></span>
<span data-ttu-id="4086b-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4086b-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4086b-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4086b-129">JSON representation</span></span>
<span data-ttu-id="4086b-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4086b-130">The following is a JSON representation of the resource.</span></span>
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
