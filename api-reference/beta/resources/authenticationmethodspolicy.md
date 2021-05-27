---
title: тип ресурса authenticationMethodsPolicy
description: Определяет методы проверки подлинности и пользователей, которые могут использовать их для регистрации и выполнения многофакторной проверки подлинности (MFA).
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: fdf86929b4098d9fb62f1426883b55d95c669f32
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682936"
---
# <a name="authenticationmethodspolicy-resource-type"></a><span data-ttu-id="75b13-103">тип ресурса authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="75b13-103">authenticationMethodsPolicy resource type</span></span>

<span data-ttu-id="75b13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75b13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75b13-105">Определяет методы проверки подлинности и пользователей, которые могут использовать их для регистрации и выполнения многофакторной проверки подлинности (MFA) в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="75b13-105">Defines authentication methods and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="75b13-106">Методы</span><span class="sxs-lookup"><span data-stu-id="75b13-106">Methods</span></span>
|<span data-ttu-id="75b13-107">Метод</span><span class="sxs-lookup"><span data-stu-id="75b13-107">Method</span></span>|<span data-ttu-id="75b13-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="75b13-108">Return type</span></span>|<span data-ttu-id="75b13-109">Описание</span><span class="sxs-lookup"><span data-stu-id="75b13-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="75b13-110">Получить проверку подлинностиMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="75b13-110">Get authenticationMethodsPolicy</span></span>](../api/authenticationmethodspolicy-get.md)|[<span data-ttu-id="75b13-111">authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="75b13-111">authenticationMethodsPolicy</span></span>](../resources/authenticationmethodspolicy.md)|<span data-ttu-id="75b13-112">Ознакомьтесь с свойствами и отношениями объекта [authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="75b13-112">Read the properties and relationships of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>|
|[<span data-ttu-id="75b13-113">Обновление проверки подлинностиMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="75b13-113">Update authenticationMethodsPolicy</span></span>](../api/authenticationmethodspolicy-update.md)|[<span data-ttu-id="75b13-114">authenticationMethodsPolicy</span><span class="sxs-lookup"><span data-stu-id="75b13-114">authenticationMethodsPolicy</span></span>](../resources/authenticationmethodspolicy.md)|<span data-ttu-id="75b13-115">Обновление свойств объекта [authenticationMethodsPolicy.](../resources/authenticationmethodspolicy.md)</span><span class="sxs-lookup"><span data-stu-id="75b13-115">Update the properties of an [authenticationMethodsPolicy](../resources/authenticationmethodspolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="75b13-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="75b13-116">Properties</span></span>
|<span data-ttu-id="75b13-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="75b13-117">Property</span></span>|<span data-ttu-id="75b13-118">Тип</span><span class="sxs-lookup"><span data-stu-id="75b13-118">Type</span></span>|<span data-ttu-id="75b13-119">Описание</span><span class="sxs-lookup"><span data-stu-id="75b13-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75b13-120">description</span><span class="sxs-lookup"><span data-stu-id="75b13-120">description</span></span>|<span data-ttu-id="75b13-121">String</span><span class="sxs-lookup"><span data-stu-id="75b13-121">String</span></span>|<span data-ttu-id="75b13-122">Описание политики.</span><span class="sxs-lookup"><span data-stu-id="75b13-122">A description of the policy.</span></span>|
|<span data-ttu-id="75b13-123">displayName</span><span class="sxs-lookup"><span data-stu-id="75b13-123">displayName</span></span>|<span data-ttu-id="75b13-124">String</span><span class="sxs-lookup"><span data-stu-id="75b13-124">String</span></span>|<span data-ttu-id="75b13-125">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="75b13-125">The name of the policy.</span></span>|
|<span data-ttu-id="75b13-126">id</span><span class="sxs-lookup"><span data-stu-id="75b13-126">id</span></span>|<span data-ttu-id="75b13-127">String</span><span class="sxs-lookup"><span data-stu-id="75b13-127">String</span></span>|<span data-ttu-id="75b13-128">Идентификатор политики.</span><span class="sxs-lookup"><span data-stu-id="75b13-128">The identifier of the policy.</span></span> <span data-ttu-id="75b13-129">Наследуется от [сущности](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="75b13-129">Inherited from [entity](../resources/entity.md).</span></span>|
|<span data-ttu-id="75b13-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75b13-130">lastModifiedDateTime</span></span>|<span data-ttu-id="75b13-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75b13-131">DateTimeOffset</span></span>|<span data-ttu-id="75b13-132">Дата и время последнего обновления политики.</span><span class="sxs-lookup"><span data-stu-id="75b13-132">The date and time of the last update to the policy.</span></span>|
|<span data-ttu-id="75b13-133">policyVersion</span><span class="sxs-lookup"><span data-stu-id="75b13-133">policyVersion</span></span>|<span data-ttu-id="75b13-134">String</span><span class="sxs-lookup"><span data-stu-id="75b13-134">String</span></span>|<span data-ttu-id="75b13-135">Версия используемой политики.</span><span class="sxs-lookup"><span data-stu-id="75b13-135">The version of the policy in use.</span></span>|
|<span data-ttu-id="75b13-136">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="75b13-136">registrationEnforcement</span></span>|[<span data-ttu-id="75b13-137">registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="75b13-137">registrationEnforcement</span></span>](../resources/registrationenforcement.md)|<span data-ttu-id="75b13-138">Принудительное выполнение регистрации во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="75b13-138">Enforce registration at sign-in time.</span></span> <span data-ttu-id="75b13-139">Это свойство можно использовать для напоминания пользователям о том, как настроить целевые методы проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="75b13-139">This property can be used to remind users to set up targeted authentication methods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75b13-140">Связи</span><span class="sxs-lookup"><span data-stu-id="75b13-140">Relationships</span></span>
|<span data-ttu-id="75b13-141">Связь</span><span class="sxs-lookup"><span data-stu-id="75b13-141">Relationship</span></span>|<span data-ttu-id="75b13-142">Тип</span><span class="sxs-lookup"><span data-stu-id="75b13-142">Type</span></span>|<span data-ttu-id="75b13-143">Описание</span><span class="sxs-lookup"><span data-stu-id="75b13-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75b13-144">authenticationMethodConfigurations</span><span class="sxs-lookup"><span data-stu-id="75b13-144">authenticationMethodConfigurations</span></span>|<span data-ttu-id="75b13-145">[коллекция authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75b13-145">[authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md) collection</span></span>|<span data-ttu-id="75b13-146">Представляет параметры для каждого метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="75b13-146">Represents the settings for each authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75b13-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="75b13-147">JSON representation</span></span>
<span data-ttu-id="75b13-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75b13-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodsPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "policyVersion": "String",
  "registrationEnforcement": {
    "@odata.type": "microsoft.graph.registrationEnforcement"
  } 
}
```
