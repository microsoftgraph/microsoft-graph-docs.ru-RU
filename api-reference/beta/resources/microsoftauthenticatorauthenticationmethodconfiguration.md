---
title: тип ресурса microsoftAuthenticatorAuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5af441d32c02f2c6b8be45ef3f3ab401b10d12da
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444149"
---
# <a name="microsoftauthenticatorauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="85cd5-103">тип ресурса microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="85cd5-103">microsoftAuthenticatorAuthenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="85cd5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85cd5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85cd5-105">Представляет политику методов проверки подлинности Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="85cd5-105">Represents a Microsoft Authenticator authentication methods policy.</span></span> <span data-ttu-id="85cd5-106">Политики методов проверки подлинности определяют параметры конфигурации, а также пользователей или групп, которые могут использовать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="85cd5-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="85cd5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="85cd5-107">Methods</span></span>
|<span data-ttu-id="85cd5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="85cd5-108">Method</span></span>|<span data-ttu-id="85cd5-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="85cd5-109">Return type</span></span>|<span data-ttu-id="85cd5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="85cd5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85cd5-111">[получение](../api/microsoftauthenticatorauthenticationmethodconfiguration-get.md);</span><span class="sxs-lookup"><span data-stu-id="85cd5-111">[Get](../api/microsoftauthenticatorauthenticationmethodconfiguration-get.md)</span></span>|[<span data-ttu-id="85cd5-112">MicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="85cd5-112">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="85cd5-113">Ознакомьтесь с свойствами и отношениями объекта MicrosoftAuthenticatorAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="85cd5-113">Read the properties and relationships of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="85cd5-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="85cd5-114">Update</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="85cd5-115">MicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="85cd5-115">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="85cd5-116">Обновление свойств объекта MicrosoftAuthenticatorAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="85cd5-116">Update the properties of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|<span data-ttu-id="85cd5-117">[удаление](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md);</span><span class="sxs-lookup"><span data-stu-id="85cd5-117">[Delete](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md)</span></span>|<span data-ttu-id="85cd5-118">Нет</span><span class="sxs-lookup"><span data-stu-id="85cd5-118">None</span></span>|<span data-ttu-id="85cd5-119">Возвращает объект MicrosoftAuthenticatorAuthenticationMethodConfiguration к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="85cd5-119">Reverts the microsoftAuthenticatorAuthenticationMethodConfiguration object to its default configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="85cd5-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="85cd5-120">Properties</span></span>
|<span data-ttu-id="85cd5-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="85cd5-121">Property</span></span>|<span data-ttu-id="85cd5-122">Тип</span><span class="sxs-lookup"><span data-stu-id="85cd5-122">Type</span></span>|<span data-ttu-id="85cd5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="85cd5-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85cd5-124">id</span><span class="sxs-lookup"><span data-stu-id="85cd5-124">id</span></span>|<span data-ttu-id="85cd5-125">String</span><span class="sxs-lookup"><span data-stu-id="85cd5-125">String</span></span>|<span data-ttu-id="85cd5-126">Идентификатор политики метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="85cd5-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="85cd5-127">state</span><span class="sxs-lookup"><span data-stu-id="85cd5-127">state</span></span>|<span data-ttu-id="85cd5-128">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="85cd5-128">authenticationMethodState</span></span>|<span data-ttu-id="85cd5-129">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="85cd5-129">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85cd5-130">Связи</span><span class="sxs-lookup"><span data-stu-id="85cd5-130">Relationships</span></span>
|<span data-ttu-id="85cd5-131">Связь</span><span class="sxs-lookup"><span data-stu-id="85cd5-131">Relationship</span></span>|<span data-ttu-id="85cd5-132">Тип</span><span class="sxs-lookup"><span data-stu-id="85cd5-132">Type</span></span>|<span data-ttu-id="85cd5-133">Описание</span><span class="sxs-lookup"><span data-stu-id="85cd5-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85cd5-134">includeTargets</span><span class="sxs-lookup"><span data-stu-id="85cd5-134">includeTargets</span></span>|<span data-ttu-id="85cd5-135">[коллекция microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="85cd5-135">[microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="85cd5-136">Коллекция пользователей или групп, которые могут использовать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="85cd5-136">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85cd5-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85cd5-137">JSON representation</span></span>
<span data-ttu-id="85cd5-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85cd5-138">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```

