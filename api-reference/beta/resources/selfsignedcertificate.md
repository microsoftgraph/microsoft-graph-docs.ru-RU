---
title: тип ресурса selfSignedCertificate
description: Содержит сведения о публичной части сертификата подписи.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: luleonpla
ms.openlocfilehash: 1dbb9bcb15a3e820b3676e336826a741ecbb5e9f
ms.sourcegitcommit: 40a8e4b9e344811267025e23c372a6e60e31a1b9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/01/2021
ms.locfileid: "52118979"
---
# <a name="selfsignedcertificate-resource-type"></a><span data-ttu-id="f227d-103">тип ресурса selfSignedCertificate</span><span class="sxs-lookup"><span data-stu-id="f227d-103">selfSignedCertificate resource type</span></span>

<span data-ttu-id="f227d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f227d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f227d-105">Содержит публичную часть сертификата подписи.</span><span class="sxs-lookup"><span data-stu-id="f227d-105">Contains the public part of a signing certificate.</span></span> <span data-ttu-id="f227d-106">Это возвращающий тип действия [addSelfSignedSigningCertificate.](../api/serviceprincipal-addtokensigningcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="f227d-106">It's the return type of the action [addSelfSignedSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md).</span></span> <span data-ttu-id="f227d-107">Поставщики услуг используют публичную часть сертификата подписи для проверки эмитента маркера.</span><span class="sxs-lookup"><span data-stu-id="f227d-107">Service providers use the public part of the signing certificate to validate the issuer of the token.</span></span>

## <a name="properties"></a><span data-ttu-id="f227d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f227d-108">Properties</span></span>
<span data-ttu-id="f227d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f227d-109">Property</span></span>|<span data-ttu-id="f227d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f227d-110">Type</span></span>|<span data-ttu-id="f227d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f227d-111">Description</span></span>
----|--|---
|<span data-ttu-id="f227d-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="f227d-112">customKeyIdentifier</span></span>|<span data-ttu-id="f227d-113">В двоичном формате</span><span class="sxs-lookup"><span data-stu-id="f227d-113">Binary</span></span>| <span data-ttu-id="f227d-114">Настраиваемый идентификатор ключа.</span><span class="sxs-lookup"><span data-stu-id="f227d-114">Custom key identifier.</span></span> |
| <span data-ttu-id="f227d-115">displayName</span><span class="sxs-lookup"><span data-stu-id="f227d-115">displayName</span></span> | <span data-ttu-id="f227d-116">String</span><span class="sxs-lookup"><span data-stu-id="f227d-116">String</span></span> | <span data-ttu-id="f227d-117">Удобное имя для ключа.</span><span class="sxs-lookup"><span data-stu-id="f227d-117">The friendly name for the key.</span></span> |
|<span data-ttu-id="f227d-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f227d-118">endDateTime</span></span>|<span data-ttu-id="f227d-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f227d-119">DateTimeOffset</span></span>|<span data-ttu-id="f227d-120">Дата и время истечения срока действия учетных данных.</span><span class="sxs-lookup"><span data-stu-id="f227d-120">The date and time at which the credential expires.</span></span> <span data-ttu-id="f227d-121">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f227d-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f227d-122">Например, полночь UTC 1 января 2014 г. выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="f227d-122">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="f227d-123">keyId</span><span class="sxs-lookup"><span data-stu-id="f227d-123">keyId</span></span>|<span data-ttu-id="f227d-124">Guid</span><span class="sxs-lookup"><span data-stu-id="f227d-124">Guid</span></span>|<span data-ttu-id="f227d-125">Уникальный идентификатор (GUID) для ключа.</span><span class="sxs-lookup"><span data-stu-id="f227d-125">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="f227d-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f227d-126">startDateTime</span></span>|<span data-ttu-id="f227d-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f227d-127">DateTimeOffset</span></span>|<span data-ttu-id="f227d-128">Дата и время, в течение которых учетные данные становятся действительными.</span><span class="sxs-lookup"><span data-stu-id="f227d-128">The date and time at which the credential becomes valid.</span></span> <span data-ttu-id="f227d-129">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f227d-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f227d-130">Например, полночь UTC 1 января 2014 г. выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="f227d-130">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="f227d-131">type</span><span class="sxs-lookup"><span data-stu-id="f227d-131">type</span></span>|<span data-ttu-id="f227d-132">String</span><span class="sxs-lookup"><span data-stu-id="f227d-132">String</span></span>|<span data-ttu-id="f227d-133">Тип учетных данных ключей.</span><span class="sxs-lookup"><span data-stu-id="f227d-133">The type of key credential.</span></span> <span data-ttu-id="f227d-134">"AsymmetricX509Cert".</span><span class="sxs-lookup"><span data-stu-id="f227d-134">"AsymmetricX509Cert".</span></span>|
|<span data-ttu-id="f227d-135">использование</span><span class="sxs-lookup"><span data-stu-id="f227d-135">usage</span></span>|<span data-ttu-id="f227d-136">String</span><span class="sxs-lookup"><span data-stu-id="f227d-136">String</span></span>|<span data-ttu-id="f227d-137">Строка, описываемая цель, для которой можно использовать ключ.</span><span class="sxs-lookup"><span data-stu-id="f227d-137">A string that describes the purpose for which the key can be used.</span></span> <span data-ttu-id="f227d-138">Например, "Проверка".</span><span class="sxs-lookup"><span data-stu-id="f227d-138">For example, "Verify".</span></span>|
|<span data-ttu-id="f227d-139">key</span><span class="sxs-lookup"><span data-stu-id="f227d-139">key</span></span>|<span data-ttu-id="f227d-140">Двоичный</span><span class="sxs-lookup"><span data-stu-id="f227d-140">Binary</span></span>| <span data-ttu-id="f227d-141">Значение для учетных данных ключа.</span><span class="sxs-lookup"><span data-stu-id="f227d-141">The value for the key credential.</span></span> <span data-ttu-id="f227d-142">Должно быть закодированное значение base-64.</span><span class="sxs-lookup"><span data-stu-id="f227d-142">Should be a base-64 encoded value.</span></span> |
|<span data-ttu-id="f227d-143">отпечатки пальцев</span><span class="sxs-lookup"><span data-stu-id="f227d-143">thumbprint</span></span>| <span data-ttu-id="f227d-144">String</span><span class="sxs-lookup"><span data-stu-id="f227d-144">String</span></span> | <span data-ttu-id="f227d-145">Значение отпечатка пальца для ключа.</span><span class="sxs-lookup"><span data-stu-id="f227d-145">The thumbprint value for the key.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f227d-146">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f227d-146">JSON representation</span></span>

<span data-ttu-id="f227d-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f227d-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.selfSignedCertificate"
}-->

```json
{
    "customKeyIdentifier": "binary",
    "displayName": "string",
    "endDateTime": "string (timestamp)",
    "key": "binary",
    "keyId": "guid",
    "startDateTime": "String (timestamp)",
    "type": "string",
    "thumbprint":"string",
    "usage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "selfSignedCertificate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

