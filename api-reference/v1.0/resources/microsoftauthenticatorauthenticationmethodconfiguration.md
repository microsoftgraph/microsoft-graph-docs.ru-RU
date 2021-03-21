---
title: тип ресурса microsoftAuthenticatorAuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 375044feffd7ba22a2e2174808d639d2d2c3b6f4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964940"
---
# <a name="microsoftauthenticatorauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="7bea1-103">тип ресурса microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="7bea1-103">microsoftAuthenticatorAuthenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="7bea1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bea1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7bea1-105">Представляет политику методов проверки подлинности Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="7bea1-105">Represents a Microsoft Authenticator authentication methods policy.</span></span> <span data-ttu-id="7bea1-106">Политики методов проверки подлинности определяют параметры конфигурации, а также пользователей или групп, которые могут использовать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="7bea1-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="7bea1-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7bea1-107">Methods</span></span>
|<span data-ttu-id="7bea1-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7bea1-108">Method</span></span>|<span data-ttu-id="7bea1-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="7bea1-109">Return type</span></span>|<span data-ttu-id="7bea1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7bea1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bea1-111">[получение](../api/microsoftauthenticatorauthenticationmethodconfiguration-get.md);</span><span class="sxs-lookup"><span data-stu-id="7bea1-111">[Get](../api/microsoftauthenticatorauthenticationmethodconfiguration-get.md)</span></span>|[<span data-ttu-id="7bea1-112">MicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="7bea1-112">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="7bea1-113">Ознакомьтесь с свойствами и отношениями объекта MicrosoftAuthenticatorAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7bea1-113">Read the properties and relationships of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="7bea1-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="7bea1-114">Update</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="7bea1-115">MicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="7bea1-115">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="7bea1-116">Обновление свойств объекта MicrosoftAuthenticatorAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7bea1-116">Update the properties of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|<span data-ttu-id="7bea1-117">[удаление](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md);</span><span class="sxs-lookup"><span data-stu-id="7bea1-117">[Delete](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md)</span></span>|<span data-ttu-id="7bea1-118">Нет</span><span class="sxs-lookup"><span data-stu-id="7bea1-118">None</span></span>|<span data-ttu-id="7bea1-119">Возвращает объект MicrosoftAuthenticatorAuthenticationMethodConfiguration к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7bea1-119">Reverts the microsoftAuthenticatorAuthenticationMethodConfiguration object to its default configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="7bea1-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bea1-120">Properties</span></span>
|<span data-ttu-id="7bea1-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bea1-121">Property</span></span>|<span data-ttu-id="7bea1-122">Тип</span><span class="sxs-lookup"><span data-stu-id="7bea1-122">Type</span></span>|<span data-ttu-id="7bea1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7bea1-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bea1-124">id</span><span class="sxs-lookup"><span data-stu-id="7bea1-124">id</span></span>|<span data-ttu-id="7bea1-125">String</span><span class="sxs-lookup"><span data-stu-id="7bea1-125">String</span></span>|<span data-ttu-id="7bea1-126">Идентификатор политики метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="7bea1-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="7bea1-127">state</span><span class="sxs-lookup"><span data-stu-id="7bea1-127">state</span></span>|<span data-ttu-id="7bea1-128">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="7bea1-128">authenticationMethodState</span></span>|<span data-ttu-id="7bea1-129">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="7bea1-129">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bea1-130">Связи</span><span class="sxs-lookup"><span data-stu-id="7bea1-130">Relationships</span></span>
|<span data-ttu-id="7bea1-131">Связь</span><span class="sxs-lookup"><span data-stu-id="7bea1-131">Relationship</span></span>|<span data-ttu-id="7bea1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="7bea1-132">Type</span></span>|<span data-ttu-id="7bea1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7bea1-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bea1-134">includeTargets</span><span class="sxs-lookup"><span data-stu-id="7bea1-134">includeTargets</span></span>|<span data-ttu-id="7bea1-135">[коллекция microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="7bea1-135">[microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="7bea1-136">Коллекция пользователей или групп, которые могут использовать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="7bea1-136">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7bea1-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7bea1-137">JSON representation</span></span>
<span data-ttu-id="7bea1-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bea1-138">The following is a JSON representation of the resource.</span></span>
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

