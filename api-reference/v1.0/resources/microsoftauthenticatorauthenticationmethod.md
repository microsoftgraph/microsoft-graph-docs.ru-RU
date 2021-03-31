---
title: тип ресурса microsoftAuthenticatorAuthenticationMethod
description: Представление приложения Microsoft Authenticator, зарегистрированного для пользователя. Microsoft Authenticator — это метод проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7438ca72a4f5d4063eec0444d3b0028237083d9
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468991"
---
# <a name="microsoftauthenticatorauthenticationmethod-resource-type"></a><span data-ttu-id="87318-104">тип ресурса microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="87318-104">microsoftAuthenticatorAuthenticationMethod resource type</span></span>

<span data-ttu-id="87318-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87318-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="87318-106">Представление приложения Microsoft Authenticator, зарегистрированного для пользователя.</span><span class="sxs-lookup"><span data-stu-id="87318-106">A representation of the Microsoft Authenticator app registered to a user.</span></span> <span data-ttu-id="87318-107">Microsoft Authenticator — это метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="87318-107">Microsoft Authenticator is an authentication method.</span></span>

<span data-ttu-id="87318-108">Наследует от [проверки подлинностиMethod](../resources/authenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="87318-108">Inherits from [authenticationMethod](../resources/authenticationmethod.md).</span></span>

## <a name="methods"></a><span data-ttu-id="87318-109">Методы</span><span class="sxs-lookup"><span data-stu-id="87318-109">Methods</span></span>
|<span data-ttu-id="87318-110">Метод</span><span class="sxs-lookup"><span data-stu-id="87318-110">Method</span></span>|<span data-ttu-id="87318-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="87318-111">Return type</span></span>|<span data-ttu-id="87318-112">Описание</span><span class="sxs-lookup"><span data-stu-id="87318-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="87318-113">Список microsoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="87318-113">List microsoftAuthenticatorAuthenticationMethods</span></span>](../api/microsoftauthenticatorauthenticationmethod-list.md)|<span data-ttu-id="87318-114">[коллекция microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="87318-114">[microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) collection</span></span>|<span data-ttu-id="87318-115">Получите список объектов [MicrosoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="87318-115">Get a list of the [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>|
|[<span data-ttu-id="87318-116">Get microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="87318-116">Get microsoftAuthenticatorAuthenticationMethod</span></span>](../api/microsoftauthenticatorauthenticationmethod-get.md)|[<span data-ttu-id="87318-117">MicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="87318-117">microsoftAuthenticatorAuthenticationMethod</span></span>](../resources/microsoftauthenticatorauthenticationmethod.md)|<span data-ttu-id="87318-118">Ознакомьтесь с свойствами и отношениями объекта [MicrosoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="87318-118">Read the properties and relationships of a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>|
|[<span data-ttu-id="87318-119">Удаление MicrosoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="87318-119">Delete microsoftAuthenticatorAuthenticationMethod</span></span>](../api/microsoftauthenticatorauthenticationmethod-delete.md)|<span data-ttu-id="87318-120">Нет</span><span class="sxs-lookup"><span data-stu-id="87318-120">None</span></span>|<span data-ttu-id="87318-121">Удаляет объект [MicrosoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="87318-121">Deletes a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="87318-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="87318-122">Properties</span></span>
|<span data-ttu-id="87318-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="87318-123">Property</span></span>|<span data-ttu-id="87318-124">Тип</span><span class="sxs-lookup"><span data-stu-id="87318-124">Type</span></span>|<span data-ttu-id="87318-125">Описание</span><span class="sxs-lookup"><span data-stu-id="87318-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87318-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87318-126">createdDateTime</span></span>|<span data-ttu-id="87318-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87318-127">DateTimeOffset</span></span>|<span data-ttu-id="87318-128">Дата и время регистрации этого приложения.</span><span class="sxs-lookup"><span data-stu-id="87318-128">The date and time that this app was registered.</span></span> <span data-ttu-id="87318-129">Это свойство является нулевым, если устройство не зарегистрировано для без пароля.</span><span class="sxs-lookup"><span data-stu-id="87318-129">This property is null if the device is not registered for passwordless Phone Sign-In.</span></span>|
|<span data-ttu-id="87318-130">displayName</span><span class="sxs-lookup"><span data-stu-id="87318-130">displayName</span></span>|<span data-ttu-id="87318-131">String</span><span class="sxs-lookup"><span data-stu-id="87318-131">String</span></span>|<span data-ttu-id="87318-132">Имя устройства, на котором зарегистрировано это приложение.</span><span class="sxs-lookup"><span data-stu-id="87318-132">The name of the device on which this app is registered.</span></span>|
|<span data-ttu-id="87318-133">id</span><span class="sxs-lookup"><span data-stu-id="87318-133">id</span></span>|<span data-ttu-id="87318-134">String</span><span class="sxs-lookup"><span data-stu-id="87318-134">String</span></span>|<span data-ttu-id="87318-135">Уникальный идентификатор для этого метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="87318-135">A unique identifier for this authentication method.</span></span> <span data-ttu-id="87318-136">Унаследованный от [проверки подлинностиMethod](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="87318-136">Inherited from [authenticationMethod](../resources/authenticationmethod.md)</span></span>|
|<span data-ttu-id="87318-137">deviceTag</span><span class="sxs-lookup"><span data-stu-id="87318-137">deviceTag</span></span>|<span data-ttu-id="87318-138">String</span><span class="sxs-lookup"><span data-stu-id="87318-138">String</span></span>|<span data-ttu-id="87318-139">Теги, содержащие метаданные приложений.</span><span class="sxs-lookup"><span data-stu-id="87318-139">Tags containing app metadata.</span></span>|
|<span data-ttu-id="87318-140">phoneAppVersion</span><span class="sxs-lookup"><span data-stu-id="87318-140">phoneAppVersion</span></span>|<span data-ttu-id="87318-141">String</span><span class="sxs-lookup"><span data-stu-id="87318-141">String</span></span>|<span data-ttu-id="87318-142">Числовая версия этого экземпляра приложения Authenticator.</span><span class="sxs-lookup"><span data-stu-id="87318-142">Numerical version of this instance of the Authenticator app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87318-143">Связи</span><span class="sxs-lookup"><span data-stu-id="87318-143">Relationships</span></span>
|<span data-ttu-id="87318-144">Связь</span><span class="sxs-lookup"><span data-stu-id="87318-144">Relationship</span></span>|<span data-ttu-id="87318-145">Тип</span><span class="sxs-lookup"><span data-stu-id="87318-145">Type</span></span>|<span data-ttu-id="87318-146">Описание</span><span class="sxs-lookup"><span data-stu-id="87318-146">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87318-147">device;</span><span class="sxs-lookup"><span data-stu-id="87318-147">device</span></span>|[<span data-ttu-id="87318-148">device</span><span class="sxs-lookup"><span data-stu-id="87318-148">device</span></span>](../resources/device.md)|<span data-ttu-id="87318-149">Зарегистрированное устройство, на котором находится Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="87318-149">The registered device on which Microsoft Authenticator resides.</span></span> <span data-ttu-id="87318-150">Это свойство является нулевым, если устройство не зарегистрировано для без пароля.</span><span class="sxs-lookup"><span data-stu-id="87318-150">This property is null if the device is not registered for passwordless Phone Sign-In.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87318-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87318-151">JSON representation</span></span>
<span data-ttu-id="87318-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87318-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
  "id": "String (Identifier)",
  "displayName": "String",
  "deviceTag": "String",
  "phoneAppVersion": "String",
  "createdDateTime": "DateTimeOffset"
}
```
