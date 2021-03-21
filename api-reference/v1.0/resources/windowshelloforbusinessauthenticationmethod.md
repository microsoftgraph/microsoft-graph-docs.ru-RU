---
title: тип ресурса windowsHelloForBusinessAuthenticationMethod
description: Представление экземпляра Windows Hello для бизнеса, зарегистрированного для пользователя. Windows Hello для бизнеса — это метод проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ad3fd83605d49351e2c57b469339fcfe222f05cb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964857"
---
# <a name="windowshelloforbusinessauthenticationmethod-resource-type"></a><span data-ttu-id="60c10-104">тип ресурса windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="60c10-104">windowsHelloForBusinessAuthenticationMethod resource type</span></span>

<span data-ttu-id="60c10-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60c10-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60c10-106">Представление метода проверки подлинности Windows Hello для бизнеса, зарегистрированного для пользователя.</span><span class="sxs-lookup"><span data-stu-id="60c10-106">A representation of a Windows Hello for Business authentication method registered to a user.</span></span> <span data-ttu-id="60c10-107">Windows Hello для бизнеса — это метод проверки подлинности для устройств Windows.</span><span class="sxs-lookup"><span data-stu-id="60c10-107">Windows Hello for Business is a sign-in authentication method for Windows devices.</span></span>

<span data-ttu-id="60c10-108">Наследует от [проверки подлинностиMethod](../resources/authenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="60c10-108">Inherits from [authenticationMethod](../resources/authenticationmethod.md).</span></span>

## <a name="methods"></a><span data-ttu-id="60c10-109">Методы</span><span class="sxs-lookup"><span data-stu-id="60c10-109">Methods</span></span>
|<span data-ttu-id="60c10-110">Метод</span><span class="sxs-lookup"><span data-stu-id="60c10-110">Method</span></span>|<span data-ttu-id="60c10-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="60c10-111">Return type</span></span>|<span data-ttu-id="60c10-112">Описание</span><span class="sxs-lookup"><span data-stu-id="60c10-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="60c10-113">Список windowsHelloForBusinessAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="60c10-113">List windowsHelloForBusinessAuthenticationMethods</span></span>](../api/windowshelloforbusinessauthenticationmethod-list.md)|<span data-ttu-id="60c10-114">[коллекция windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="60c10-114">[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) collection</span></span>|<span data-ttu-id="60c10-115">Получите список объектов [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="60c10-115">Get a list of the [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) objects and their properties.</span></span>|
|[<span data-ttu-id="60c10-116">Get windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="60c10-116">Get windowsHelloForBusinessAuthenticationMethod</span></span>](../api/windowshelloforbusinessauthenticationmethod-get.md)|[<span data-ttu-id="60c10-117">windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="60c10-117">windowsHelloForBusinessAuthenticationMethod</span></span>](../resources/windowshelloforbusinessauthenticationmethod.md)|<span data-ttu-id="60c10-118">Ознакомьтесь с свойствами и отношениями [объекта windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="60c10-118">Read the properties and relationships of a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>|
|[<span data-ttu-id="60c10-119">Удаление windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="60c10-119">Delete windowsHelloForBusinessAuthenticationMethod</span></span>](../api/windowshelloforbusinessauthenticationmethod-delete.md)|<span data-ttu-id="60c10-120">Нет</span><span class="sxs-lookup"><span data-stu-id="60c10-120">None</span></span>|<span data-ttu-id="60c10-121">Удаляет [объект windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="60c10-121">Deletes a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="60c10-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="60c10-122">Properties</span></span>
|<span data-ttu-id="60c10-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="60c10-123">Property</span></span>|<span data-ttu-id="60c10-124">Тип</span><span class="sxs-lookup"><span data-stu-id="60c10-124">Type</span></span>|<span data-ttu-id="60c10-125">Описание</span><span class="sxs-lookup"><span data-stu-id="60c10-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60c10-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="60c10-126">createdDateTime</span></span>|<span data-ttu-id="60c10-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60c10-127">DateTimeOffset</span></span>|<span data-ttu-id="60c10-128">Дата и время регистрации этого ключа Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="60c10-128">The date and time that this Windows Hello for Business key was registered.</span></span>|
|<span data-ttu-id="60c10-129">displayName</span><span class="sxs-lookup"><span data-stu-id="60c10-129">displayName</span></span>|<span data-ttu-id="60c10-130">String</span><span class="sxs-lookup"><span data-stu-id="60c10-130">String</span></span>|<span data-ttu-id="60c10-131">Имя устройства, на котором зарегистрирована Windows Hello для бизнеса</span><span class="sxs-lookup"><span data-stu-id="60c10-131">The name of the device on which Windows Hello for Business is registered</span></span>|
|<span data-ttu-id="60c10-132">id</span><span class="sxs-lookup"><span data-stu-id="60c10-132">id</span></span>|<span data-ttu-id="60c10-133">String</span><span class="sxs-lookup"><span data-stu-id="60c10-133">String</span></span>|<span data-ttu-id="60c10-134">Уникальный идентификатор для этого метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="60c10-134">A unique identifier for this authentication method.</span></span> <span data-ttu-id="60c10-135">Унаследованный от [проверки подлинностиMethod](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="60c10-135">Inherited from [authenticationMethod](../resources/authenticationmethod.md)</span></span>|
|<span data-ttu-id="60c10-136">keyStrength</span><span class="sxs-lookup"><span data-stu-id="60c10-136">keyStrength</span></span>|<span data-ttu-id="60c10-137">authenticationMethodKeyStrength</span><span class="sxs-lookup"><span data-stu-id="60c10-137">authenticationMethodKeyStrength</span></span>|<span data-ttu-id="60c10-138">Ключевая сила этого ключа Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="60c10-138">Key strength of this Windows Hello for Business key.</span></span> <span data-ttu-id="60c10-139">Возможные значения: `normal`, `weak`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="60c10-139">Possible values are: `normal`, `weak`, `unknown`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60c10-140">Связи</span><span class="sxs-lookup"><span data-stu-id="60c10-140">Relationships</span></span>
|<span data-ttu-id="60c10-141">Связь</span><span class="sxs-lookup"><span data-stu-id="60c10-141">Relationship</span></span>|<span data-ttu-id="60c10-142">Тип</span><span class="sxs-lookup"><span data-stu-id="60c10-142">Type</span></span>|<span data-ttu-id="60c10-143">Описание</span><span class="sxs-lookup"><span data-stu-id="60c10-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60c10-144">device;</span><span class="sxs-lookup"><span data-stu-id="60c10-144">device</span></span>|[<span data-ttu-id="60c10-145">device</span><span class="sxs-lookup"><span data-stu-id="60c10-145">device</span></span>](../resources/device.md)|<span data-ttu-id="60c10-146">Зарегистрированное устройство, на котором находится этот ключ Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="60c10-146">The registered device on which this Windows Hello for Business key resides.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60c10-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60c10-147">JSON representation</span></span>
<span data-ttu-id="60c10-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60c10-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
  "id": "String (Identifier)",
  "displayName": "String",
  "createdDateTime": "String",
  "keyStrength": {"@odata.type": "microsoft.graph.authenticationMethodKeyStrength"}
}
```
