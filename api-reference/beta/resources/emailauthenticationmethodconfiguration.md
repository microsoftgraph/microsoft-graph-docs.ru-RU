---
title: Тип ресурса Емаилаусентикатионмесодконфигуратион
description: Представляет политику методов проверки подлинности методом проверки подлинности методом OTP
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3e3e18973759d7f120dd0bd8e984c98568054960
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617145"
---
# <a name="emailauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="4ae0f-103">Тип ресурса Емаилаусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4ae0f-103">emailAuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="4ae0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ae0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ae0f-105">Представляет политику методов проверки подлинности методом проверки подлинности OTP для этого клиента.</span><span class="sxs-lookup"><span data-stu-id="4ae0f-105">Represents this tenant's email OTP authentication methods policy.</span></span> <span data-ttu-id="4ae0f-106">Политики методов проверки подлинности определяют параметры конфигурации, а также пользователей или группы, для которых разрешено использование метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="4ae0f-106">Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method.</span></span> <span data-ttu-id="4ae0f-107">В некоторых случаях для проверки подлинности с помощью облачных пользователей для самостоятельного сброса пароля или внешними пользователями для проверки подлинности может использоваться подтверждение подлинности OTP.</span><span class="sxs-lookup"><span data-stu-id="4ae0f-107">Email OTP may be used by the tenant's cloud-native users for self-service password reset, or by external users for authentication in some circumstances.</span></span>

## <a name="methods"></a><span data-ttu-id="4ae0f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="4ae0f-108">Methods</span></span>

|<span data-ttu-id="4ae0f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="4ae0f-109">Method</span></span>|<span data-ttu-id="4ae0f-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="4ae0f-110">Return type</span></span>|<span data-ttu-id="4ae0f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4ae0f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4ae0f-112">Получение Емаилаусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4ae0f-112">Get emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="4ae0f-113">емаилаусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4ae0f-113">emailAuthenticationMethodConfiguration</span></span>](../resources/emailauthenticationmethodconfiguration.md)|<span data-ttu-id="4ae0f-114">Чтение свойств и связей объекта Емаилаусентикатионмесодконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="4ae0f-114">Read the properties and relationships of an emailAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="4ae0f-115">Обновление Емаилаусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4ae0f-115">Update emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="4ae0f-116">емаилаусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4ae0f-116">emailAuthenticationMethodConfiguration</span></span>](../resources/emailauthenticationmethodconfiguration.md)|<span data-ttu-id="4ae0f-117">Обновление свойств объекта Емаилаусентикатионмесодконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="4ae0f-117">Update the properties of an emailAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="4ae0f-118">Удаление Емаилаусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4ae0f-118">Delete emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="4ae0f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="4ae0f-119">None</span></span>|<span data-ttu-id="4ae0f-120">Удаляет объект Емаилаусентикатионмесодконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="4ae0f-120">Deletes an emailAuthenticationMethodConfiguration object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4ae0f-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ae0f-121">Properties</span></span>

|<span data-ttu-id="4ae0f-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ae0f-122">Property</span></span>|<span data-ttu-id="4ae0f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4ae0f-123">Type</span></span>|<span data-ttu-id="4ae0f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4ae0f-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ae0f-125">id</span><span class="sxs-lookup"><span data-stu-id="4ae0f-125">id</span></span>|<span data-ttu-id="4ae0f-126">String</span><span class="sxs-lookup"><span data-stu-id="4ae0f-126">String</span></span>|<span data-ttu-id="4ae0f-127">Идентификатор политики метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="4ae0f-127">The authentication method policy identifier.</span></span> <span data-ttu-id="4ae0f-128">Наследуется от [аусентикатионмесодконфигуратион](../resources/authenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4ae0f-128">Inherited from [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md).</span></span>|
|<span data-ttu-id="4ae0f-129">state</span><span class="sxs-lookup"><span data-stu-id="4ae0f-129">state</span></span>|<span data-ttu-id="4ae0f-130">аусентикатионмесодстате</span><span class="sxs-lookup"><span data-stu-id="4ae0f-130">authenticationMethodState</span></span>|<span data-ttu-id="4ae0f-131">Указывает, включен ли этот метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="4ae0f-131">Indicates whether this authentication method is enabled or not.</span></span> <span data-ttu-id="4ae0f-132">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4ae0f-132">Possible values are: `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4ae0f-133">алловекстерналидтаусимаилотп</span><span class="sxs-lookup"><span data-stu-id="4ae0f-133">allowExternalIdToUseEmailOtp</span></span>|<span data-ttu-id="4ae0f-134">екстерналемаилотпстате</span><span class="sxs-lookup"><span data-stu-id="4ae0f-134">externalEmailOtpState</span></span>|<span data-ttu-id="4ae0f-135">Определяет, будут ли для проверки подлинности использоваться внешние пользователи для проверки подлинности методом OTP.</span><span class="sxs-lookup"><span data-stu-id="4ae0f-135">Determines whether email OTP is usable by external users for authentication.</span></span> <span data-ttu-id="4ae0f-136">Возможные значения: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4ae0f-136">Possible values are: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span></span> <span data-ttu-id="4ae0f-137">Клиенты, для `default` которых не использовалась общедоступная Предварительная версия, автоматически включили OTP, начиная с 2021 марта.</span><span class="sxs-lookup"><span data-stu-id="4ae0f-137">Tenants in the `default` state who did not use public preview will automatically have email OTP enabled beginning in March 2021.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ae0f-138">Связи</span><span class="sxs-lookup"><span data-stu-id="4ae0f-138">Relationships</span></span>

|<span data-ttu-id="4ae0f-139">Связь</span><span class="sxs-lookup"><span data-stu-id="4ae0f-139">Relationship</span></span>|<span data-ttu-id="4ae0f-140">Тип</span><span class="sxs-lookup"><span data-stu-id="4ae0f-140">Type</span></span>|<span data-ttu-id="4ae0f-141">Описание</span><span class="sxs-lookup"><span data-stu-id="4ae0f-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ae0f-142">инклудетаржетс</span><span class="sxs-lookup"><span data-stu-id="4ae0f-142">includeTargets</span></span>|<span data-ttu-id="4ae0f-143">Коллекция [аусентикатионмесодтаржет](../resources/authenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="4ae0f-143">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="4ae0f-144">Коллекция пользователей или групп, которым разрешено использовать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="4ae0f-144">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ae0f-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ae0f-145">JSON representation</span></span>

<span data-ttu-id="4ae0f-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ae0f-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "allowExternalIdToUseEmailOtp": "String",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
