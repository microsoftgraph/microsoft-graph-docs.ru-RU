---
title: тип ресурса fido2AuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности FIDO2
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7684b8b2c6601b4afdad25b3d3c32b7a6b68667d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964964"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="d82c7-103">тип ресурса fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="d82c7-103">fido2AuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="d82c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d82c7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d82c7-105">Представляет политику методов проверки подлинности FIDO2.</span><span class="sxs-lookup"><span data-stu-id="d82c7-105">Represents a FIDO2 authentication methods policy.</span></span> <span data-ttu-id="d82c7-106">Политики методов проверки подлинности определяют параметры конфигурации, а также пользователей или групп, которым включен метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d82c7-106">Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="d82c7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d82c7-107">Methods</span></span>
|<span data-ttu-id="d82c7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d82c7-108">Method</span></span>|<span data-ttu-id="d82c7-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="d82c7-109">Return type</span></span>|<span data-ttu-id="d82c7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d82c7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d82c7-111">[получение](../api/fido2authenticationmethodconfiguration-get.md);</span><span class="sxs-lookup"><span data-stu-id="d82c7-111">[Get](../api/fido2authenticationmethodconfiguration-get.md)</span></span>|[<span data-ttu-id="d82c7-112">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="d82c7-112">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="d82c7-113">Ознакомьтесь с свойствами и отношениями объекта fido2AuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d82c7-113">Read the properties and relationships of a fido2AuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="d82c7-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="d82c7-114">Update</span></span>](../api/fido2authenticationmethodconfiguration-update.md)|[<span data-ttu-id="d82c7-115">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="d82c7-115">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="d82c7-116">Обновление свойств объекта fido2AuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d82c7-116">Update the properties of a fido2AuthenticationMethodConfiguration object.</span></span>|
|<span data-ttu-id="d82c7-117">[удаление](../api/fido2authenticationmethodconfiguration-delete.md);</span><span class="sxs-lookup"><span data-stu-id="d82c7-117">[Delete](../api/fido2authenticationmethodconfiguration-delete.md)</span></span>|<span data-ttu-id="d82c7-118">Нет</span><span class="sxs-lookup"><span data-stu-id="d82c7-118">None</span></span>|<span data-ttu-id="d82c7-119">Возвращает объект fido2AuthenticationMethodConfiguration к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d82c7-119">Reverts the fido2AuthenticationMethodConfiguration object to its default configuration.</span></span>|


## <a name="properties"></a><span data-ttu-id="d82c7-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="d82c7-120">Properties</span></span>
|<span data-ttu-id="d82c7-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="d82c7-121">Property</span></span>|<span data-ttu-id="d82c7-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d82c7-122">Type</span></span>|<span data-ttu-id="d82c7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d82c7-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d82c7-124">id</span><span class="sxs-lookup"><span data-stu-id="d82c7-124">id</span></span>|<span data-ttu-id="d82c7-125">String</span><span class="sxs-lookup"><span data-stu-id="d82c7-125">String</span></span>|<span data-ttu-id="d82c7-126">Идентификатор политики метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d82c7-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="d82c7-127">isAttestationEnforced</span><span class="sxs-lookup"><span data-stu-id="d82c7-127">isAttestationEnforced</span></span>|<span data-ttu-id="d82c7-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="d82c7-128">Boolean</span></span>|<span data-ttu-id="d82c7-129">Определяет, необходимо ли применять проверку для регистрации ключей безопасности FIDO2.</span><span class="sxs-lookup"><span data-stu-id="d82c7-129">Determines whether attestation must be enforced for FIDO2 security key registration.</span></span>|
|<span data-ttu-id="d82c7-130">isSelfServiceRegistrationAllowed</span><span class="sxs-lookup"><span data-stu-id="d82c7-130">isSelfServiceRegistrationAllowed</span></span>|<span data-ttu-id="d82c7-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="d82c7-131">Boolean</span></span>|<span data-ttu-id="d82c7-132">Определяет, могут ли пользователи зарегистрировать новые ключи безопасности FIDO2.</span><span class="sxs-lookup"><span data-stu-id="d82c7-132">Determines if users can register new FIDO2 security keys.</span></span>|
|<span data-ttu-id="d82c7-133">keyRestrictions</span><span class="sxs-lookup"><span data-stu-id="d82c7-133">keyRestrictions</span></span>|[<span data-ttu-id="d82c7-134">fido2KeyRestrictions</span><span class="sxs-lookup"><span data-stu-id="d82c7-134">fido2KeyRestrictions</span></span>](../resources/fido2keyrestrictions.md)|<span data-ttu-id="d82c7-135">Контролирует, применяются ли ключевые ограничения для ключей безопасности FIDO2, разрешая или отменить определенные типы ключей, определенных GUID проверки подлинности (AAGUID), идентификатором, который указывает тип (например, сделать и модель) аутентиста.</span><span class="sxs-lookup"><span data-stu-id="d82c7-135">Controls whether key restrictions are enforced on FIDO2 security keys, either allowing or disallowing certain key types as defined by Authenticator Attestation GUID (AAGUID), an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="d82c7-136">state</span><span class="sxs-lookup"><span data-stu-id="d82c7-136">state</span></span>|<span data-ttu-id="d82c7-137">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="d82c7-137">authenticationMethodState</span></span>|<span data-ttu-id="d82c7-138">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d82c7-138">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d82c7-139">Связи</span><span class="sxs-lookup"><span data-stu-id="d82c7-139">Relationships</span></span>
|<span data-ttu-id="d82c7-140">Связь</span><span class="sxs-lookup"><span data-stu-id="d82c7-140">Relationship</span></span>|<span data-ttu-id="d82c7-141">Тип</span><span class="sxs-lookup"><span data-stu-id="d82c7-141">Type</span></span>|<span data-ttu-id="d82c7-142">Описание</span><span class="sxs-lookup"><span data-stu-id="d82c7-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d82c7-143">includeTargets</span><span class="sxs-lookup"><span data-stu-id="d82c7-143">includeTargets</span></span>|<span data-ttu-id="d82c7-144">[коллекция authenticationMethodTarget](../resources/authenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="d82c7-144">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="d82c7-145">Коллекция пользователей или групп, которые могут использовать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d82c7-145">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d82c7-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d82c7-146">JSON representation</span></span>
<span data-ttu-id="d82c7-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d82c7-147">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fido2AuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2AuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "isSelfServiceRegistrationAllowed": "Boolean",
  "isAttestationEnforced": "Boolean",
  "keyRestrictions": {
    "@odata.type": "microsoft.graph.fido2KeyRestrictions"
  },
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
