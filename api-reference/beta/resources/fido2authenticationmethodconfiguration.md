---
title: Тип ресурса fido2AuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности FIDO2
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 62aa22fa22b70235f5221bc820cee5178b55b51b
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418431"
---
# <a name="fido2authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="ad52a-103">Тип ресурса fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ad52a-103">fido2AuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="ad52a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad52a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad52a-105">Представляет политику методов проверки подлинности FIDO2.</span><span class="sxs-lookup"><span data-stu-id="ad52a-105">Represents a FIDO2 authentication methods policy.</span></span> <span data-ttu-id="ad52a-106">Политики методов проверки подлинности определяют параметры конфигурации, а также пользователей или группы, для которых разрешено использование метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ad52a-106">Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="ad52a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ad52a-107">Methods</span></span>
|<span data-ttu-id="ad52a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ad52a-108">Method</span></span>|<span data-ttu-id="ad52a-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="ad52a-109">Return type</span></span>|<span data-ttu-id="ad52a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ad52a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ad52a-111">Получение</span><span class="sxs-lookup"><span data-stu-id="ad52a-111">Get</span></span>](../api/fido2authenticationmethodconfiguration-get.md)|[<span data-ttu-id="ad52a-112">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ad52a-112">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="ad52a-113">Чтение свойств и связей объекта fido2AuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ad52a-113">Read the properties and relationships of a fido2AuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="ad52a-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="ad52a-114">Update</span></span>](../api/fido2authenticationmethodconfiguration-update.md)|[<span data-ttu-id="ad52a-115">fido2AuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ad52a-115">fido2AuthenticationMethodConfiguration</span></span>](../resources/fido2authenticationmethodconfiguration.md)|<span data-ttu-id="ad52a-116">Обновление свойств объекта fido2AuthenticationMethodConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ad52a-116">Update the properties of a fido2AuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="ad52a-117">Удаление</span><span class="sxs-lookup"><span data-stu-id="ad52a-117">Delete</span></span>](../api/fido2authenticationmethodconfiguration-delete.md)|<span data-ttu-id="ad52a-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ad52a-118">None</span></span>|<span data-ttu-id="ad52a-119">Возвращает объект fido2AuthenticationMethodConfiguration в конфигурацию по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ad52a-119">Reverts the fido2AuthenticationMethodConfiguration object to its default configuration.</span></span>|


## <a name="properties"></a><span data-ttu-id="ad52a-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad52a-120">Properties</span></span>
|<span data-ttu-id="ad52a-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad52a-121">Property</span></span>|<span data-ttu-id="ad52a-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ad52a-122">Type</span></span>|<span data-ttu-id="ad52a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ad52a-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad52a-124">id</span><span class="sxs-lookup"><span data-stu-id="ad52a-124">id</span></span>|<span data-ttu-id="ad52a-125">String</span><span class="sxs-lookup"><span data-stu-id="ad52a-125">String</span></span>|<span data-ttu-id="ad52a-126">Идентификатор политики метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ad52a-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="ad52a-127">исаттестатионенфорцед</span><span class="sxs-lookup"><span data-stu-id="ad52a-127">isAttestationEnforced</span></span>|<span data-ttu-id="ad52a-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad52a-128">Boolean</span></span>|<span data-ttu-id="ad52a-129">Определяет, следует ли применять аттестацию для регистрации ключа безопасности FIDO2.</span><span class="sxs-lookup"><span data-stu-id="ad52a-129">Determines whether attestation must be enforced for FIDO2 security key registration.</span></span>|
|<span data-ttu-id="ad52a-130">исселфсервицерегистратионалловед</span><span class="sxs-lookup"><span data-stu-id="ad52a-130">isSelfServiceRegistrationAllowed</span></span>|<span data-ttu-id="ad52a-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad52a-131">Boolean</span></span>|<span data-ttu-id="ad52a-132">Определяет, могут ли пользователи регистрировать новые ключи безопасности FIDO2.</span><span class="sxs-lookup"><span data-stu-id="ad52a-132">Determines if users can register new FIDO2 security keys.</span></span>|
|<span data-ttu-id="ad52a-133">кэйрестриктионс</span><span class="sxs-lookup"><span data-stu-id="ad52a-133">keyRestrictions</span></span>|[<span data-ttu-id="ad52a-134">fido2KeyRestrictions</span><span class="sxs-lookup"><span data-stu-id="ad52a-134">fido2KeyRestrictions</span></span>](../resources/fido2keyrestrictions.md)|<span data-ttu-id="ad52a-135">Определяет, применяются ли ограничения ключей к ключам безопасности FIDO2, разрешать или запрещать определенные типы ключей, как определено идентификатором GUID аттестации (ААГУИД), идентификатором, указывающим тип (например, make and model) средства проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ad52a-135">Controls whether key restrictions are enforced on FIDO2 security keys, either allowing or disallowing certain key types as defined by Authenticator Attestation GUID (AAGUID), an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="ad52a-136">state</span><span class="sxs-lookup"><span data-stu-id="ad52a-136">state</span></span>|<span data-ttu-id="ad52a-137">аусентикатионмесодстате</span><span class="sxs-lookup"><span data-stu-id="ad52a-137">authenticationMethodState</span></span>|<span data-ttu-id="ad52a-138">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ad52a-138">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad52a-139">Связи</span><span class="sxs-lookup"><span data-stu-id="ad52a-139">Relationships</span></span>
|<span data-ttu-id="ad52a-140">Связь</span><span class="sxs-lookup"><span data-stu-id="ad52a-140">Relationship</span></span>|<span data-ttu-id="ad52a-141">Тип</span><span class="sxs-lookup"><span data-stu-id="ad52a-141">Type</span></span>|<span data-ttu-id="ad52a-142">Описание</span><span class="sxs-lookup"><span data-stu-id="ad52a-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad52a-143">инклудетаржетс</span><span class="sxs-lookup"><span data-stu-id="ad52a-143">includeTargets</span></span>|<span data-ttu-id="ad52a-144">Коллекция [аусентикатионмесодтаржет](../resources/authenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="ad52a-144">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="ad52a-145">Коллекция пользователей или групп, которым разрешено использовать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="ad52a-145">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad52a-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad52a-146">JSON representation</span></span>
<span data-ttu-id="ad52a-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad52a-147">The following is a JSON representation of the resource.</span></span>
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
