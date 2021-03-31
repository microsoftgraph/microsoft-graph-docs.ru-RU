---
title: тип ресурса microsoftAuthenticatorAuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0700a6811b35123709628abc66d8e4eb6b319a03
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469264"
---
# <a name="microsoftauthenticatorauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="472e8-103">тип ресурса microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="472e8-103">microsoftAuthenticatorAuthenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="472e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="472e8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="472e8-105">Представляет политику методов проверки подлинности Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="472e8-105">Represents a Microsoft Authenticator authentication methods policy.</span></span> <span data-ttu-id="472e8-106">Политики методов проверки подлинности определяют параметры конфигурации, а также пользователей или групп, которые могут использовать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="472e8-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="472e8-107">Методы</span><span class="sxs-lookup"><span data-stu-id="472e8-107">Methods</span></span>
|<span data-ttu-id="472e8-108">Метод</span><span class="sxs-lookup"><span data-stu-id="472e8-108">Method</span></span>|<span data-ttu-id="472e8-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="472e8-109">Return type</span></span>|<span data-ttu-id="472e8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="472e8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="472e8-111">Получение</span><span class="sxs-lookup"><span data-stu-id="472e8-111">Get</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="472e8-112">MicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="472e8-112">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="472e8-113">Ознакомьтесь с свойствами и отношениями объекта MicrosoftAuthenticatorAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="472e8-113">Read the properties and relationships of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="472e8-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="472e8-114">Update</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="472e8-115">MicrosoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="472e8-115">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="472e8-116">Обновление свойств объекта MicrosoftAuthenticatorAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="472e8-116">Update the properties of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|<span data-ttu-id="472e8-117">[удаление](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md);</span><span class="sxs-lookup"><span data-stu-id="472e8-117">[Delete](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md)</span></span>|<span data-ttu-id="472e8-118">Нет</span><span class="sxs-lookup"><span data-stu-id="472e8-118">None</span></span>|<span data-ttu-id="472e8-119">Возвращает объект MicrosoftAuthenticatorAuthenticationMethodConfiguration к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="472e8-119">Reverts the microsoftAuthenticatorAuthenticationMethodConfiguration object to its default configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="472e8-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="472e8-120">Properties</span></span>
|<span data-ttu-id="472e8-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="472e8-121">Property</span></span>|<span data-ttu-id="472e8-122">Тип</span><span class="sxs-lookup"><span data-stu-id="472e8-122">Type</span></span>|<span data-ttu-id="472e8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="472e8-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="472e8-124">id</span><span class="sxs-lookup"><span data-stu-id="472e8-124">id</span></span>|<span data-ttu-id="472e8-125">String</span><span class="sxs-lookup"><span data-stu-id="472e8-125">String</span></span>|<span data-ttu-id="472e8-126">Идентификатор политики метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="472e8-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="472e8-127">state</span><span class="sxs-lookup"><span data-stu-id="472e8-127">state</span></span>|<span data-ttu-id="472e8-128">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="472e8-128">authenticationMethodState</span></span>|<span data-ttu-id="472e8-129">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="472e8-129">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="472e8-130">Связи</span><span class="sxs-lookup"><span data-stu-id="472e8-130">Relationships</span></span>
|<span data-ttu-id="472e8-131">Связь</span><span class="sxs-lookup"><span data-stu-id="472e8-131">Relationship</span></span>|<span data-ttu-id="472e8-132">Тип</span><span class="sxs-lookup"><span data-stu-id="472e8-132">Type</span></span>|<span data-ttu-id="472e8-133">Описание</span><span class="sxs-lookup"><span data-stu-id="472e8-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="472e8-134">includeTargets</span><span class="sxs-lookup"><span data-stu-id="472e8-134">includeTargets</span></span>|<span data-ttu-id="472e8-135">[коллекция microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="472e8-135">[microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="472e8-136">Коллекция пользователей или групп, которые могут использовать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="472e8-136">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="472e8-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="472e8-137">JSON representation</span></span>
<span data-ttu-id="472e8-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="472e8-138">The following is a JSON representation of the resource.</span></span>
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

