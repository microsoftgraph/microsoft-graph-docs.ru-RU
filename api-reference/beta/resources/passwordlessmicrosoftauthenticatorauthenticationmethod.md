---
title: passwordlessMicrosoftAuthenticatorAuthenticationMethod resource type
description: Представление метода microsoft Authenticator Passwordless Phone Sign-in, зарегистрированного на пользователя.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0949a92d0adbcfdd53164b550b6d8f8bc07444eb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444079"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethod-resource-type-deprecated"></a><span data-ttu-id="9ce8e-103">passwordlessMicrosoftAuthenticatorAuthenticationMethod resource type (deprecated)</span><span class="sxs-lookup"><span data-stu-id="9ce8e-103">passwordlessMicrosoftAuthenticatorAuthenticationMethod resource type (deprecated)</span></span>

<span data-ttu-id="9ce8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ce8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ce8e-105">Представление метода microsoft Authenticator Passwordless Phone Sign-in, зарегистрированного на пользователя.</span><span class="sxs-lookup"><span data-stu-id="9ce8e-105">A representation of a Microsoft Authenticator Passwordless Phone Sign-in method registered to a user.</span></span>

> [!CAUTION]
> <span data-ttu-id="9ce8e-106">API без пароля Microsoft Authenticator phone is deprecated and will stop returning results on 31 December 2020.</span><span class="sxs-lookup"><span data-stu-id="9ce8e-106">The Microsoft Authenticator Passwordless Phone Sign-in method API is deprecated and will stop returning results on December 31, 2020.</span></span> <span data-ttu-id="9ce8e-107">Используйте новый метод [проверки подлинности Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethod.md)</span><span class="sxs-lookup"><span data-stu-id="9ce8e-107">Please use the new [Microsoft Authenticator Authentication Method](../resources/microsoftAuthenticatorAuthenticationMethod.md).</span></span>


## <a name="methods"></a><span data-ttu-id="9ce8e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="9ce8e-108">Methods</span></span>
|<span data-ttu-id="9ce8e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="9ce8e-109">Method</span></span>|<span data-ttu-id="9ce8e-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="9ce8e-110">Return type</span></span>|<span data-ttu-id="9ce8e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9ce8e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ce8e-112">[Список](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-list.md) (неподготовленный)</span><span class="sxs-lookup"><span data-stu-id="9ce8e-112">[List](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-list.md) (deprecated)</span></span>|<span data-ttu-id="9ce8e-113">[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) collection</span><span class="sxs-lookup"><span data-stu-id="9ce8e-113">[passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) collection</span></span>|<span data-ttu-id="9ce8e-114">Извлечение списка объектов без паролейMicrosoftAuthenticatorAuthenticationMethod и их свойств.</span><span class="sxs-lookup"><span data-stu-id="9ce8e-114">Retrieve a list of a user's passwordlessMicrosoftAuthenticatorAuthenticationMethod objects and their properties.</span></span>|
|<span data-ttu-id="9ce8e-115">[Get](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-get.md) (deprecated)</span><span class="sxs-lookup"><span data-stu-id="9ce8e-115">[Get](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-get.md) (deprecated)</span></span>|[<span data-ttu-id="9ce8e-116">passwordlessMicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9ce8e-116">passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md)|<span data-ttu-id="9ce8e-117">Ознакомьтесь с свойствами и отношениями объекта без пароляMicrosoftAuthenticatorAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="9ce8e-117">Read the properties and relationships of a user's passwordlessMicrosoftAuthenticatorAuthenticationMethod object.</span></span>|
|<span data-ttu-id="9ce8e-118">[Delete](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-delete.md) (deprecated)</span><span class="sxs-lookup"><span data-stu-id="9ce8e-118">[Delete](../api/passwordlessmicrosoftauthenticatorauthenticationmethod-delete.md) (deprecated)</span></span>|<span data-ttu-id="9ce8e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="9ce8e-119">None</span></span>|<span data-ttu-id="9ce8e-120">Удаляет объект без пароляMicrosoftAuthenticatorAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="9ce8e-120">Deletes a user's passwordlessMicrosoftAuthenticatorAuthenticationMethod object.</span></span>|


## <a name="properties"></a><span data-ttu-id="9ce8e-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ce8e-121">Properties</span></span>
|<span data-ttu-id="9ce8e-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ce8e-122">Property</span></span>|<span data-ttu-id="9ce8e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="9ce8e-123">Type</span></span>|<span data-ttu-id="9ce8e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9ce8e-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ce8e-125">id</span><span class="sxs-lookup"><span data-stu-id="9ce8e-125">id</span></span>|<span data-ttu-id="9ce8e-126">String</span><span class="sxs-lookup"><span data-stu-id="9ce8e-126">String</span></span>|<span data-ttu-id="9ce8e-127">Идентификатор метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="9ce8e-127">The authentication method identifier.</span></span>|
|<span data-ttu-id="9ce8e-128">displayName</span><span class="sxs-lookup"><span data-stu-id="9ce8e-128">displayName</span></span>|<span data-ttu-id="9ce8e-129">String</span><span class="sxs-lookup"><span data-stu-id="9ce8e-129">String</span></span>|<span data-ttu-id="9ce8e-130">Отображающее имя мобильного устройства в качестве данной пользователем.</span><span class="sxs-lookup"><span data-stu-id="9ce8e-130">The display name of the mobile device as given by the user.</span></span>|
|<span data-ttu-id="9ce8e-131">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="9ce8e-131">creationDateTime</span></span>|<span data-ttu-id="9ce8e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ce8e-132">DateTimeOffset</span></span>|<span data-ttu-id="9ce8e-133">Время регистрации этого метода пользователем.</span><span class="sxs-lookup"><span data-stu-id="9ce8e-133">The timestamp when this method was registered to the user.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9ce8e-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9ce8e-134">JSON representation</span></span>
<span data-ttu-id="9ce8e-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ce8e-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod",
  "id": "String (identifier)",
  "displayName": "String",
  "creationDateTime": "String (timestamp)"
}
```

