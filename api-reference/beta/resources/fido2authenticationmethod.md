---
title: тип ресурса fido2AuthenticationMethod
description: Представление ключа безопасности FIDO2, зарегистрированного для пользователя. FIDO2 — это метод проверки подлинности.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 11c0598f19fcc5bf6f9862a2d87fa1f08acb8a2c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945671"
---
# <a name="fido2authenticationmethod-resource-type"></a><span data-ttu-id="0f465-104">тип ресурса fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0f465-104">fido2AuthenticationMethod resource type</span></span>

<span data-ttu-id="0f465-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f465-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f465-106">Представление ключа безопасности FIDO2, зарегистрированного для пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f465-106">A representation of a FIDO2 security key registered to a user.</span></span> <span data-ttu-id="0f465-107">FIDO2 — это метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0f465-107">FIDO2 is a sign-in authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="0f465-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0f465-108">Methods</span></span>
|<span data-ttu-id="0f465-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0f465-109">Method</span></span>|<span data-ttu-id="0f465-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="0f465-110">Return type</span></span>|<span data-ttu-id="0f465-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0f465-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0f465-112">Список</span><span class="sxs-lookup"><span data-stu-id="0f465-112">List</span></span>](../api/fido2authenticationmethod-list.md)|<span data-ttu-id="0f465-113">[коллекция fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="0f465-113">[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) collection</span></span>|<span data-ttu-id="0f465-114">Извлечение списка объектов fido2AuthenticationMethod пользователя и их свойств.</span><span class="sxs-lookup"><span data-stu-id="0f465-114">Retrieve a list of a user's fido2AuthenticationMethod objects and their properties.</span></span>|
|<span data-ttu-id="0f465-115">[получение](../api/fido2authenticationmethod-get.md);</span><span class="sxs-lookup"><span data-stu-id="0f465-115">[Get](../api/fido2authenticationmethod-get.md)</span></span>|[<span data-ttu-id="0f465-116">fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0f465-116">fido2AuthenticationMethod</span></span>](../resources/fido2authenticationmethod.md)|<span data-ttu-id="0f465-117">Ознакомьтесь с свойствами и отношениями объекта fido2AuthenticationMethod пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f465-117">Read the properties and relationships of a user's fido2AuthenticationMethod object.</span></span>|
|<span data-ttu-id="0f465-118">[удаление](../api/fido2authenticationmethod-delete.md);</span><span class="sxs-lookup"><span data-stu-id="0f465-118">[Delete](../api/fido2authenticationmethod-delete.md)</span></span>|<span data-ttu-id="0f465-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0f465-119">None</span></span>|<span data-ttu-id="0f465-120">Удаляет объект fido2AuthenticationMethod пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f465-120">Deletes a user's fido2AuthenticationMethod object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f465-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f465-121">Properties</span></span>
|<span data-ttu-id="0f465-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f465-122">Property</span></span>|<span data-ttu-id="0f465-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0f465-123">Type</span></span>|<span data-ttu-id="0f465-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0f465-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f465-125">id</span><span class="sxs-lookup"><span data-stu-id="0f465-125">id</span></span>|<span data-ttu-id="0f465-126">Строка</span><span class="sxs-lookup"><span data-stu-id="0f465-126">String</span></span>|<span data-ttu-id="0f465-127">Идентификатор метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0f465-127">The authentication method identifier.</span></span>|
|<span data-ttu-id="0f465-128">displayName</span><span class="sxs-lookup"><span data-stu-id="0f465-128">displayName</span></span>|<span data-ttu-id="0f465-129">Строка</span><span class="sxs-lookup"><span data-stu-id="0f465-129">String</span></span>|<span data-ttu-id="0f465-130">Отображает имя ключа, заданное пользователем.</span><span class="sxs-lookup"><span data-stu-id="0f465-130">The display name of the key as given by the user.</span></span>|
|<span data-ttu-id="0f465-131">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="0f465-131">creationDateTime</span></span>|<span data-ttu-id="0f465-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f465-132">DateTimeOffset</span></span>|<span data-ttu-id="0f465-133">Время регистрации этого ключа пользователю.</span><span class="sxs-lookup"><span data-stu-id="0f465-133">The timestamp when this key was registered to the user.</span></span>|
|<span data-ttu-id="0f465-134">aaGuid</span><span class="sxs-lookup"><span data-stu-id="0f465-134">aaGuid</span></span>|<span data-ttu-id="0f465-135">Строка</span><span class="sxs-lookup"><span data-stu-id="0f465-135">String</span></span>|<span data-ttu-id="0f465-136">GUID проверки подлинности, идентификатор, который указывает тип (например, make и model) аутентиста.</span><span class="sxs-lookup"><span data-stu-id="0f465-136">Authenticator Attestation GUID, an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="0f465-137">model</span><span class="sxs-lookup"><span data-stu-id="0f465-137">model</span></span>|<span data-ttu-id="0f465-138">String</span><span class="sxs-lookup"><span data-stu-id="0f465-138">String</span></span>|<span data-ttu-id="0f465-139">Назначенная производителем модель ключа безопасности FIDO2.</span><span class="sxs-lookup"><span data-stu-id="0f465-139">The manufacturer-assigned model of the FIDO2 security key.</span></span>|
|<span data-ttu-id="0f465-140">attestationCertificates</span><span class="sxs-lookup"><span data-stu-id="0f465-140">attestationCertificates</span></span>|<span data-ttu-id="0f465-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0f465-141">String collection</span></span>|<span data-ttu-id="0f465-142">Сертификат аттестации(ы), присоединенный к этому ключу безопасности.</span><span class="sxs-lookup"><span data-stu-id="0f465-142">The attestation certificate(s) attached to this security key.</span></span>|
|<span data-ttu-id="0f465-143">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="0f465-143">attestationLevel</span></span>|<span data-ttu-id="0f465-144">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="0f465-144">attestationLevel</span></span>|<span data-ttu-id="0f465-145">Уровень проверки этого ключа безопасности FIDO2.</span><span class="sxs-lookup"><span data-stu-id="0f465-145">The attestation level of this FIDO2 security key.</span></span> <span data-ttu-id="0f465-146">Возможные значения: `attested`, `notAttested`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0f465-146">Possible values are: `attested`, `notAttested`, `unknownFutureValue`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="0f465-147">Связи</span><span class="sxs-lookup"><span data-stu-id="0f465-147">Relationships</span></span>
<span data-ttu-id="0f465-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0f465-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f465-149">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0f465-149">JSON representation</span></span>
<span data-ttu-id="0f465-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f465-150">The following is a JSON representation of the resource.</span></span>
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
  "aaGuid": "String",
  "model": "String",
  "attestationCertificates": [
    "String"
  ],
  "attestationLevel": "String"
}
```

