---
title: тип ресурса fido2AuthenticationMethod
description: Представление ключа безопасности FIDO2, зарегистрированного для пользователя. FIDO2 — это метод проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 87c7f5e0f9ed29e6e1f5aa7c8ec332620bcc8a0a
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335648"
---
# <a name="fido2authenticationmethod-resource-type"></a><span data-ttu-id="70556-104">тип ресурса fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="70556-104">fido2AuthenticationMethod resource type</span></span>

<span data-ttu-id="70556-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70556-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70556-106">Представление ключа безопасности FIDO2, зарегистрированного для пользователя.</span><span class="sxs-lookup"><span data-stu-id="70556-106">A representation of a FIDO2 security key registered to a user.</span></span> <span data-ttu-id="70556-107">FIDO2 — это метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="70556-107">FIDO2 is a sign-in authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="70556-108">Методы</span><span class="sxs-lookup"><span data-stu-id="70556-108">Methods</span></span>
|<span data-ttu-id="70556-109">Метод</span><span class="sxs-lookup"><span data-stu-id="70556-109">Method</span></span>|<span data-ttu-id="70556-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="70556-110">Return type</span></span>|<span data-ttu-id="70556-111">Описание</span><span class="sxs-lookup"><span data-stu-id="70556-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="70556-112">Список</span><span class="sxs-lookup"><span data-stu-id="70556-112">List</span></span>](../api/fido2authenticationmethod-list.md)|<span data-ttu-id="70556-113">[коллекция fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="70556-113">[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) collection</span></span>|<span data-ttu-id="70556-114">Извлечение списка объектов fido2AuthenticationMethod пользователя и их свойств.</span><span class="sxs-lookup"><span data-stu-id="70556-114">Retrieve a list of a user's fido2AuthenticationMethod objects and their properties.</span></span>|
|<span data-ttu-id="70556-115">[получение](../api/fido2authenticationmethod-get.md);</span><span class="sxs-lookup"><span data-stu-id="70556-115">[Get](../api/fido2authenticationmethod-get.md)</span></span>|[<span data-ttu-id="70556-116">fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="70556-116">fido2AuthenticationMethod</span></span>](../resources/fido2authenticationmethod.md)|<span data-ttu-id="70556-117">Ознакомьтесь с свойствами и отношениями объекта fido2AuthenticationMethod пользователя.</span><span class="sxs-lookup"><span data-stu-id="70556-117">Read the properties and relationships of a user's fido2AuthenticationMethod object.</span></span>|
|<span data-ttu-id="70556-118">[удаление](../api/fido2authenticationmethod-delete.md);</span><span class="sxs-lookup"><span data-stu-id="70556-118">[Delete](../api/fido2authenticationmethod-delete.md)</span></span>|<span data-ttu-id="70556-119">Нет</span><span class="sxs-lookup"><span data-stu-id="70556-119">None</span></span>|<span data-ttu-id="70556-120">Удаляет объект fido2AuthenticationMethod пользователя.</span><span class="sxs-lookup"><span data-stu-id="70556-120">Deletes a user's fido2AuthenticationMethod object.</span></span>|

## <a name="properties"></a><span data-ttu-id="70556-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="70556-121">Properties</span></span>
|<span data-ttu-id="70556-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="70556-122">Property</span></span>|<span data-ttu-id="70556-123">Тип</span><span class="sxs-lookup"><span data-stu-id="70556-123">Type</span></span>|<span data-ttu-id="70556-124">Описание</span><span class="sxs-lookup"><span data-stu-id="70556-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70556-125">id</span><span class="sxs-lookup"><span data-stu-id="70556-125">id</span></span>|<span data-ttu-id="70556-126">String</span><span class="sxs-lookup"><span data-stu-id="70556-126">String</span></span>|<span data-ttu-id="70556-127">Идентификатор метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="70556-127">The authentication method identifier.</span></span>|
|<span data-ttu-id="70556-128">displayName</span><span class="sxs-lookup"><span data-stu-id="70556-128">displayName</span></span>|<span data-ttu-id="70556-129">String</span><span class="sxs-lookup"><span data-stu-id="70556-129">String</span></span>|<span data-ttu-id="70556-130">Отображает имя ключа, заданное пользователем.</span><span class="sxs-lookup"><span data-stu-id="70556-130">The display name of the key as given by the user.</span></span>|
|<span data-ttu-id="70556-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70556-131">createdDateTime</span></span>|<span data-ttu-id="70556-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70556-132">DateTimeOffset</span></span>|<span data-ttu-id="70556-133">Время регистрации этого ключа пользователю.</span><span class="sxs-lookup"><span data-stu-id="70556-133">The timestamp when this key was registered to the user.</span></span>|
|<span data-ttu-id="70556-134">creationDateTime (Deprecated)</span><span class="sxs-lookup"><span data-stu-id="70556-134">creationDateTime (Deprecated)</span></span>|<span data-ttu-id="70556-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70556-135">DateTimeOffset</span></span>|<span data-ttu-id="70556-136">Время регистрации этого ключа пользователю.</span><span class="sxs-lookup"><span data-stu-id="70556-136">The timestamp when this key was registered to the user.</span></span>|
|<span data-ttu-id="70556-137">aaGuid</span><span class="sxs-lookup"><span data-stu-id="70556-137">aaGuid</span></span>|<span data-ttu-id="70556-138">String</span><span class="sxs-lookup"><span data-stu-id="70556-138">String</span></span>|<span data-ttu-id="70556-139">Authenticator GuID-идентификатор attestation, который указывает тип (например, make и model) аутентиста.</span><span class="sxs-lookup"><span data-stu-id="70556-139">Authenticator Attestation GUID, an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="70556-140">model</span><span class="sxs-lookup"><span data-stu-id="70556-140">model</span></span>|<span data-ttu-id="70556-141">String</span><span class="sxs-lookup"><span data-stu-id="70556-141">String</span></span>|<span data-ttu-id="70556-142">Назначенная производителем модель ключа безопасности FIDO2.</span><span class="sxs-lookup"><span data-stu-id="70556-142">The manufacturer-assigned model of the FIDO2 security key.</span></span>|
|<span data-ttu-id="70556-143">attestationCertificates</span><span class="sxs-lookup"><span data-stu-id="70556-143">attestationCertificates</span></span>|<span data-ttu-id="70556-144">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="70556-144">String collection</span></span>|<span data-ttu-id="70556-145">Сертификат аттестации(ы), присоединенный к этому ключу безопасности.</span><span class="sxs-lookup"><span data-stu-id="70556-145">The attestation certificate(s) attached to this security key.</span></span>|
|<span data-ttu-id="70556-146">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="70556-146">attestationLevel</span></span>|<span data-ttu-id="70556-147">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="70556-147">attestationLevel</span></span>|<span data-ttu-id="70556-148">Уровень проверки этого ключа безопасности FIDO2.</span><span class="sxs-lookup"><span data-stu-id="70556-148">The attestation level of this FIDO2 security key.</span></span> <span data-ttu-id="70556-149">Возможные значения: `attested`, `notAttested`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="70556-149">Possible values are: `attested`, `notAttested`, `unknownFutureValue`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="70556-150">Связи</span><span class="sxs-lookup"><span data-stu-id="70556-150">Relationships</span></span>
<span data-ttu-id="70556-151">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="70556-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="70556-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="70556-152">JSON representation</span></span>
<span data-ttu-id="70556-153">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70556-153">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fido2AuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2AuthenticationMethod",
  "id": "String (identifier)",
  "displayName": "String",
  "creationDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "aaGuid": "String",
  "model": "String",
  "attestationCertificates": [
    "String"
  ],
  "attestationLevel": "String"
}
```

