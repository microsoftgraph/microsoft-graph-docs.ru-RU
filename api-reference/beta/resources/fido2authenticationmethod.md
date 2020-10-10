---
title: Тип ресурса fido2AuthenticationMethod
description: Представление ключа безопасности FIDO2, зарегистрированного для пользователя. FIDO2 — метод проверки подлинности при входе.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c4d10252201781d1339e6baa26aea248429ae462
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418435"
---
# <a name="fido2authenticationmethod-resource-type"></a><span data-ttu-id="3521e-104">Тип ресурса fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3521e-104">fido2AuthenticationMethod resource type</span></span>

<span data-ttu-id="3521e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3521e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3521e-106">Представление ключа безопасности FIDO2, зарегистрированного для пользователя.</span><span class="sxs-lookup"><span data-stu-id="3521e-106">A representation of a FIDO2 security key registered to a user.</span></span> <span data-ttu-id="3521e-107">FIDO2 — метод проверки подлинности при входе.</span><span class="sxs-lookup"><span data-stu-id="3521e-107">FIDO2 is a sign-in authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="3521e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="3521e-108">Methods</span></span>
|<span data-ttu-id="3521e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="3521e-109">Method</span></span>|<span data-ttu-id="3521e-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="3521e-110">Return type</span></span>|<span data-ttu-id="3521e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3521e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3521e-112">Перечисление</span><span class="sxs-lookup"><span data-stu-id="3521e-112">List</span></span>](../api/fido2authenticationmethod-list.md)|<span data-ttu-id="3521e-113">Коллекция [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="3521e-113">[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) collection</span></span>|<span data-ttu-id="3521e-114">Получение списка объектов fido2AuthenticationMethod пользователя и их свойств.</span><span class="sxs-lookup"><span data-stu-id="3521e-114">Retrieve a list of a user's fido2AuthenticationMethod objects and their properties.</span></span>|
|[<span data-ttu-id="3521e-115">Получение</span><span class="sxs-lookup"><span data-stu-id="3521e-115">Get</span></span>](../api/fido2authenticationmethod-get.md)|[<span data-ttu-id="3521e-116">fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3521e-116">fido2AuthenticationMethod</span></span>](../resources/fido2authenticationmethod.md)|<span data-ttu-id="3521e-117">Чтение свойств и связей объекта fido2AuthenticationMethod пользователя.</span><span class="sxs-lookup"><span data-stu-id="3521e-117">Read the properties and relationships of a user's fido2AuthenticationMethod object.</span></span>|
|[<span data-ttu-id="3521e-118">Удаление</span><span class="sxs-lookup"><span data-stu-id="3521e-118">Delete</span></span>](../api/fido2authenticationmethod-delete.md)|<span data-ttu-id="3521e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="3521e-119">None</span></span>|<span data-ttu-id="3521e-120">Удаляет объект fido2AuthenticationMethod пользователя.</span><span class="sxs-lookup"><span data-stu-id="3521e-120">Deletes a user's fido2AuthenticationMethod object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3521e-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="3521e-121">Properties</span></span>
|<span data-ttu-id="3521e-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="3521e-122">Property</span></span>|<span data-ttu-id="3521e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="3521e-123">Type</span></span>|<span data-ttu-id="3521e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3521e-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3521e-125">id</span><span class="sxs-lookup"><span data-stu-id="3521e-125">id</span></span>|<span data-ttu-id="3521e-126">String</span><span class="sxs-lookup"><span data-stu-id="3521e-126">String</span></span>|<span data-ttu-id="3521e-127">Идентификатор метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="3521e-127">The authentication method identifier.</span></span>|
|<span data-ttu-id="3521e-128">displayName</span><span class="sxs-lookup"><span data-stu-id="3521e-128">displayName</span></span>|<span data-ttu-id="3521e-129">String</span><span class="sxs-lookup"><span data-stu-id="3521e-129">String</span></span>|<span data-ttu-id="3521e-130">Отображаемое имя ключа, заданное пользователем.</span><span class="sxs-lookup"><span data-stu-id="3521e-130">The display name of the key as given by the user.</span></span>|
|<span data-ttu-id="3521e-131">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="3521e-131">creationDateTime</span></span>|<span data-ttu-id="3521e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3521e-132">DateTimeOffset</span></span>|<span data-ttu-id="3521e-133">Временная метка, когда этот ключ был зарегистрирован для пользователя.</span><span class="sxs-lookup"><span data-stu-id="3521e-133">The timestamp when this key was registered to the user.</span></span>|
|<span data-ttu-id="3521e-134">аагуид</span><span class="sxs-lookup"><span data-stu-id="3521e-134">aaGuid</span></span>|<span data-ttu-id="3521e-135">String</span><span class="sxs-lookup"><span data-stu-id="3521e-135">String</span></span>|<span data-ttu-id="3521e-136">GUID аттестации для проверки подлинности, идентификатор, указывающий тип (например, создание и модель) средства проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="3521e-136">Authenticator Attestation GUID, an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="3521e-137">model</span><span class="sxs-lookup"><span data-stu-id="3521e-137">model</span></span>|<span data-ttu-id="3521e-138">String</span><span class="sxs-lookup"><span data-stu-id="3521e-138">String</span></span>|<span data-ttu-id="3521e-139">Модель ключа безопасности FIDO2, назначенная производителем.</span><span class="sxs-lookup"><span data-stu-id="3521e-139">The manufacturer-assigned model of the FIDO2 security key.</span></span>|
|<span data-ttu-id="3521e-140">аттестатионцертификатес</span><span class="sxs-lookup"><span data-stu-id="3521e-140">attestationCertificates</span></span>|<span data-ttu-id="3521e-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3521e-141">String collection</span></span>|<span data-ttu-id="3521e-142">Сертификаты аттестации, вложенные в этот ключ безопасности.</span><span class="sxs-lookup"><span data-stu-id="3521e-142">The attestation certificate(s) attached to this security key.</span></span>|
|<span data-ttu-id="3521e-143">аттестатионлевел</span><span class="sxs-lookup"><span data-stu-id="3521e-143">attestationLevel</span></span>|<span data-ttu-id="3521e-144">аттестатионлевел</span><span class="sxs-lookup"><span data-stu-id="3521e-144">attestationLevel</span></span>|<span data-ttu-id="3521e-145">Уровень аттестации этого ключа безопасности FIDO2.</span><span class="sxs-lookup"><span data-stu-id="3521e-145">The attestation level of this FIDO2 security key.</span></span> <span data-ttu-id="3521e-146">Возможные значения: `attested` , или `notAttested` .</span><span class="sxs-lookup"><span data-stu-id="3521e-146">Possible values are: `attested`, or `notAttested`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="3521e-147">Связи</span><span class="sxs-lookup"><span data-stu-id="3521e-147">Relationships</span></span>
<span data-ttu-id="3521e-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3521e-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3521e-149">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3521e-149">JSON representation</span></span>
<span data-ttu-id="3521e-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3521e-150">The following is a JSON representation of the resource.</span></span>
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

