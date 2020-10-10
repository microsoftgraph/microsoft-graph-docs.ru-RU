---
title: Тип ресурса Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион
description: Представляет политику методов проверки подлинности входа с помощью пароля Майкрософт для проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ddf6a66abbf745a769a44cf323ebb245c31ecf60
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418483"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="55610-103">Тип ресурса Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="55610-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="55610-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55610-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55610-105">Представляет политику методов проверки подлинности входа с помощью пароля Майкрософт для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="55610-105">Represents a Microsoft Authenticator Passwordless Phone Sign-in authentication methods policy.</span></span> <span data-ttu-id="55610-106">Методы проверки подлинности определяют параметры конфигурации, а также пользователей или группы, для которых разрешено использование метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="55610-106">Authentication methods policies define configuration settings and users or groups that are enabled to use the authentication method.</span></span>

> [!NOTE]
> <span data-ttu-id="55610-107">Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии.</span><span class="sxs-lookup"><span data-stu-id="55610-107">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="55610-108">Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.</span><span class="sxs-lookup"><span data-stu-id="55610-108">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="methods"></a><span data-ttu-id="55610-109">Методы</span><span class="sxs-lookup"><span data-stu-id="55610-109">Methods</span></span>
|<span data-ttu-id="55610-110">Метод</span><span class="sxs-lookup"><span data-stu-id="55610-110">Method</span></span>|<span data-ttu-id="55610-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="55610-111">Return type</span></span>|<span data-ttu-id="55610-112">Описание</span><span class="sxs-lookup"><span data-stu-id="55610-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="55610-113">Получение</span><span class="sxs-lookup"><span data-stu-id="55610-113">Get</span></span>](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="55610-114">пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="55610-114">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="55610-115">Чтение свойств и связей объекта Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="55610-115">Read the properties and relationships of a passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="55610-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="55610-116">Update</span></span>](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="55610-117">пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="55610-117">passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration</span></span>](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="55610-118">Обновление свойств объекта Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="55610-118">Update the properties of a passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="55610-119">Удаление</span><span class="sxs-lookup"><span data-stu-id="55610-119">Delete</span></span>](../api/passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="55610-120">Нет</span><span class="sxs-lookup"><span data-stu-id="55610-120">None</span></span>|<span data-ttu-id="55610-121">Возвращает объект Пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион в конфигурацию по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="55610-121">Reverts the passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration object to its default configuration.</span></span>|


## <a name="properties"></a><span data-ttu-id="55610-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="55610-122">Properties</span></span>
|<span data-ttu-id="55610-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="55610-123">Property</span></span>|<span data-ttu-id="55610-124">Тип</span><span class="sxs-lookup"><span data-stu-id="55610-124">Type</span></span>|<span data-ttu-id="55610-125">Описание</span><span class="sxs-lookup"><span data-stu-id="55610-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55610-126">id</span><span class="sxs-lookup"><span data-stu-id="55610-126">id</span></span>|<span data-ttu-id="55610-127">String</span><span class="sxs-lookup"><span data-stu-id="55610-127">String</span></span>|<span data-ttu-id="55610-128">Идентификатор политики метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="55610-128">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="55610-129">state</span><span class="sxs-lookup"><span data-stu-id="55610-129">state</span></span>|<span data-ttu-id="55610-130">аусентикатионмесодстате</span><span class="sxs-lookup"><span data-stu-id="55610-130">authenticationMethodState</span></span>|<span data-ttu-id="55610-131">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="55610-131">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55610-132">Связи</span><span class="sxs-lookup"><span data-stu-id="55610-132">Relationships</span></span>
|<span data-ttu-id="55610-133">Связь</span><span class="sxs-lookup"><span data-stu-id="55610-133">Relationship</span></span>|<span data-ttu-id="55610-134">Тип</span><span class="sxs-lookup"><span data-stu-id="55610-134">Type</span></span>|<span data-ttu-id="55610-135">Описание</span><span class="sxs-lookup"><span data-stu-id="55610-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55610-136">инклудетаржетс</span><span class="sxs-lookup"><span data-stu-id="55610-136">includeTargets</span></span>|<span data-ttu-id="55610-137">Коллекция [пассвордлессмикрософтаусентикатораусентикатионмесодтаржет](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="55610-137">[passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget](../resources/passwordlessmicrosoftauthenticatorauthenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="55610-138">Коллекция пользователей или групп, которым разрешено использовать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="55610-138">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55610-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55610-139">JSON representation</span></span>
<span data-ttu-id="55610-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55610-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
