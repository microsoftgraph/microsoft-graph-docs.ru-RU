---
title: Тип ресурса microsoftAuthenticatorAuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7f2d5dbc64fe81b629f89cf0b98bd3f2d32c1411
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49874497"
---
# <a name="microsoftauthenticatorauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="fb148-103">Тип ресурса microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb148-103">microsoftAuthenticatorAuthenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="fb148-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb148-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb148-105">Представляет политику методов проверки подлинности Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="fb148-105">Represents a Microsoft Authenticator authentication methods policy.</span></span> <span data-ttu-id="fb148-106">Политики методов проверки подлинности определяют параметры конфигурации и пользователей или группы, которые могут использовать этот метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="fb148-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="fb148-107">Методы</span><span class="sxs-lookup"><span data-stu-id="fb148-107">Methods</span></span>
|<span data-ttu-id="fb148-108">Метод</span><span class="sxs-lookup"><span data-stu-id="fb148-108">Method</span></span>|<span data-ttu-id="fb148-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="fb148-109">Return type</span></span>|<span data-ttu-id="fb148-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fb148-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb148-111">[получение](../api/microsoftauthenticatorauthenticationmethodconfiguration-get.md);</span><span class="sxs-lookup"><span data-stu-id="fb148-111">[Get](../api/microsoftauthenticatorauthenticationmethodconfiguration-get.md)</span></span>|[<span data-ttu-id="fb148-112">microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb148-112">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="fb148-113">Чтение свойств и связей объекта microsoftAuthenticatorAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fb148-113">Read the properties and relationships of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="fb148-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="fb148-114">Update</span></span>](../api/microsoftauthenticatorauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="fb148-115">microsoftAuthenticatorAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb148-115">microsoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="fb148-116">Обновление свойств объекта microsoftAuthenticatorAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fb148-116">Update the properties of a microsoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|<span data-ttu-id="fb148-117">[удаление](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md);</span><span class="sxs-lookup"><span data-stu-id="fb148-117">[Delete](../api/microsoftauthenticatorauthenticationmethodconfiguration-delete.md)</span></span>|<span data-ttu-id="fb148-118">Нет</span><span class="sxs-lookup"><span data-stu-id="fb148-118">None</span></span>|<span data-ttu-id="fb148-119">Возвращает объект microsoftAuthenticatorAuthenticationMethodConfiguration в конфигурацию по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fb148-119">Reverts the microsoftAuthenticatorAuthenticationMethodConfiguration object to its default configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="fb148-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb148-120">Properties</span></span>
|<span data-ttu-id="fb148-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb148-121">Property</span></span>|<span data-ttu-id="fb148-122">Тип</span><span class="sxs-lookup"><span data-stu-id="fb148-122">Type</span></span>|<span data-ttu-id="fb148-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fb148-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb148-124">id</span><span class="sxs-lookup"><span data-stu-id="fb148-124">id</span></span>|<span data-ttu-id="fb148-125">String</span><span class="sxs-lookup"><span data-stu-id="fb148-125">String</span></span>|<span data-ttu-id="fb148-126">Идентификатор политики метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="fb148-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="fb148-127">state</span><span class="sxs-lookup"><span data-stu-id="fb148-127">state</span></span>|<span data-ttu-id="fb148-128">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="fb148-128">authenticationMethodState</span></span>|<span data-ttu-id="fb148-129">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="fb148-129">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb148-130">Связи</span><span class="sxs-lookup"><span data-stu-id="fb148-130">Relationships</span></span>
|<span data-ttu-id="fb148-131">Связь</span><span class="sxs-lookup"><span data-stu-id="fb148-131">Relationship</span></span>|<span data-ttu-id="fb148-132">Тип</span><span class="sxs-lookup"><span data-stu-id="fb148-132">Type</span></span>|<span data-ttu-id="fb148-133">Описание</span><span class="sxs-lookup"><span data-stu-id="fb148-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb148-134">includeTargets</span><span class="sxs-lookup"><span data-stu-id="fb148-134">includeTargets</span></span>|<span data-ttu-id="fb148-135">[Коллекция microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="fb148-135">[microsoftAuthenticatorAuthenticationMethodTarget](../resources/microsoftauthenticatorauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="fb148-136">Коллекция пользователей или групп, которым включен метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="fb148-136">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb148-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb148-137">JSON representation</span></span>
<span data-ttu-id="fb148-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb148-138">The following is a JSON representation of the resource.</span></span>
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

