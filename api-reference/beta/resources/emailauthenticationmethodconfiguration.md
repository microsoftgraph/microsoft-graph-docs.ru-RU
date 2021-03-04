---
title: тип ресурса emailAuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности OTP электронной почты
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 73b620a3fd5bea62aa927722a7dac7ce3d5a9fab
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440362"
---
# <a name="emailauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="0473f-103">тип ресурса emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="0473f-103">emailAuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="0473f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0473f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0473f-105">Представляет политику методов проверки подлинности электронной почты этого клиента.</span><span class="sxs-lookup"><span data-stu-id="0473f-105">Represents this tenant's email OTP authentication methods policy.</span></span> <span data-ttu-id="0473f-106">Политики методов проверки подлинности определяют параметры конфигурации, а также пользователей или групп, которым включен метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0473f-106">Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method.</span></span> <span data-ttu-id="0473f-107">OTP-адрес электронной почты может использоваться облачными пользователями клиента для сброса пароля самообслуживления или внешними пользователями для проверки подлинности в некоторых случаях.</span><span class="sxs-lookup"><span data-stu-id="0473f-107">Email OTP may be used by the tenant's cloud-native users for self-service password reset, or by external users for authentication in some circumstances.</span></span>

## <a name="methods"></a><span data-ttu-id="0473f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0473f-108">Methods</span></span>

|<span data-ttu-id="0473f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0473f-109">Method</span></span>|<span data-ttu-id="0473f-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="0473f-110">Return type</span></span>|<span data-ttu-id="0473f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0473f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0473f-112">Получить emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="0473f-112">Get emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="0473f-113">emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="0473f-113">emailAuthenticationMethodConfiguration</span></span>](../resources/emailauthenticationmethodconfiguration.md)|<span data-ttu-id="0473f-114">Ознакомьтесь с свойствами и отношениями объекта emailAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0473f-114">Read the properties and relationships of an emailAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="0473f-115">Обновление emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="0473f-115">Update emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="0473f-116">emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="0473f-116">emailAuthenticationMethodConfiguration</span></span>](../resources/emailauthenticationmethodconfiguration.md)|<span data-ttu-id="0473f-117">Обновление свойств объекта emailAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0473f-117">Update the properties of an emailAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="0473f-118">Удаление emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="0473f-118">Delete emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="0473f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0473f-119">None</span></span>|<span data-ttu-id="0473f-120">Удаляет объект emailAuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0473f-120">Deletes an emailAuthenticationMethodConfiguration object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0473f-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="0473f-121">Properties</span></span>

|<span data-ttu-id="0473f-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="0473f-122">Property</span></span>|<span data-ttu-id="0473f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0473f-123">Type</span></span>|<span data-ttu-id="0473f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0473f-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0473f-125">id</span><span class="sxs-lookup"><span data-stu-id="0473f-125">id</span></span>|<span data-ttu-id="0473f-126">String</span><span class="sxs-lookup"><span data-stu-id="0473f-126">String</span></span>|<span data-ttu-id="0473f-127">Идентификатор политики метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0473f-127">The authentication method policy identifier.</span></span> <span data-ttu-id="0473f-128">Унаследованный от [проверки подлинностиMethodConfiguration](../resources/authenticationmethodconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0473f-128">Inherited from [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md).</span></span>|
|<span data-ttu-id="0473f-129">state</span><span class="sxs-lookup"><span data-stu-id="0473f-129">state</span></span>|<span data-ttu-id="0473f-130">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="0473f-130">authenticationMethodState</span></span>|<span data-ttu-id="0473f-131">Указывает, включен этот метод проверки подлинности или нет.</span><span class="sxs-lookup"><span data-stu-id="0473f-131">Indicates whether this authentication method is enabled or not.</span></span> <span data-ttu-id="0473f-132">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="0473f-132">Possible values are: `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0473f-133">allowExternalIdToUseEmailOtp</span><span class="sxs-lookup"><span data-stu-id="0473f-133">allowExternalIdToUseEmailOtp</span></span>|<span data-ttu-id="0473f-134">externalEmailOtpState</span><span class="sxs-lookup"><span data-stu-id="0473f-134">externalEmailOtpState</span></span>|<span data-ttu-id="0473f-135">Определяет, является ли OTP электронной почты для внешних пользователей для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0473f-135">Determines whether email OTP is usable by external users for authentication.</span></span> <span data-ttu-id="0473f-136">Возможные значения: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0473f-136">Possible values are: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span></span> <span data-ttu-id="0473f-137">Клиенты в состоянии, которое не использует общедоступный предварительный просмотр, автоматически будут иметь включенную OTP-почту начиная с `default` марта 2021 г.</span><span class="sxs-lookup"><span data-stu-id="0473f-137">Tenants in the `default` state who did not use public preview will automatically have email OTP enabled beginning in March 2021.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0473f-138">Связи</span><span class="sxs-lookup"><span data-stu-id="0473f-138">Relationships</span></span>

|<span data-ttu-id="0473f-139">Связь</span><span class="sxs-lookup"><span data-stu-id="0473f-139">Relationship</span></span>|<span data-ttu-id="0473f-140">Тип</span><span class="sxs-lookup"><span data-stu-id="0473f-140">Type</span></span>|<span data-ttu-id="0473f-141">Описание</span><span class="sxs-lookup"><span data-stu-id="0473f-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0473f-142">includeTargets</span><span class="sxs-lookup"><span data-stu-id="0473f-142">includeTargets</span></span>|<span data-ttu-id="0473f-143">[коллекция authenticationMethodTarget](../resources/authenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="0473f-143">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="0473f-144">Коллекция пользователей или групп, которые могут использовать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0473f-144">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0473f-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0473f-145">JSON representation</span></span>

<span data-ttu-id="0473f-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0473f-146">The following is a JSON representation of the resource.</span></span>
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
