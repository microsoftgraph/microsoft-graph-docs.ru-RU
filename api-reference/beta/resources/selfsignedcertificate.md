---
title: тип ресурса selfSignedCertificate
description: Содержит сведения о публичной части сертификата подписи.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: luleonpla
ms.openlocfilehash: a32720520c804d13048babe8a779132780abc782
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266866"
---
# <a name="selfsignedcertificate-resource-type"></a><span data-ttu-id="a4dc0-103">тип ресурса selfSignedCertificate</span><span class="sxs-lookup"><span data-stu-id="a4dc0-103">selfSignedCertificate resource type</span></span>

<span data-ttu-id="a4dc0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4dc0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4dc0-105">Содержит публичную часть сертификата подписи.</span><span class="sxs-lookup"><span data-stu-id="a4dc0-105">Contains the public part of a signing certificate.</span></span> <span data-ttu-id="a4dc0-106">Это возвращающий тип действия [addSelfSignedSigningCertificate.](../api/serviceprincipal-addtokensigningcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="a4dc0-106">It's the return type of the action [addSelfSignedSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md).</span></span> <span data-ttu-id="a4dc0-107">Поставщики услуг используют публичную часть сертификата подписи для проверки эмитента маркера.</span><span class="sxs-lookup"><span data-stu-id="a4dc0-107">Service providers use the public part of the signing certificate to validate the issuer of the token.</span></span>

## <a name="properties"></a><span data-ttu-id="a4dc0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4dc0-108">Properties</span></span>
<span data-ttu-id="a4dc0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4dc0-109">Property</span></span>|<span data-ttu-id="a4dc0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a4dc0-110">Type</span></span>|<span data-ttu-id="a4dc0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a4dc0-111">Description</span></span>
----|--|---
|<span data-ttu-id="a4dc0-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="a4dc0-112">customKeyIdentifier</span></span>|<span data-ttu-id="a4dc0-113">В двоичном формате</span><span class="sxs-lookup"><span data-stu-id="a4dc0-113">Binary</span></span>| <span data-ttu-id="a4dc0-114">Настраиваемый идентификатор ключа.</span><span class="sxs-lookup"><span data-stu-id="a4dc0-114">Custom key identifier.</span></span> |
| <span data-ttu-id="a4dc0-115">displayName</span><span class="sxs-lookup"><span data-stu-id="a4dc0-115">displayName</span></span> | <span data-ttu-id="a4dc0-116">Строка</span><span class="sxs-lookup"><span data-stu-id="a4dc0-116">String</span></span> | <span data-ttu-id="a4dc0-117">Удобное имя для ключа.</span><span class="sxs-lookup"><span data-stu-id="a4dc0-117">The friendly name for the key.</span></span> |
|<span data-ttu-id="a4dc0-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a4dc0-118">endDateTime</span></span>|<span data-ttu-id="a4dc0-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4dc0-119">DateTimeOffset</span></span>|<span data-ttu-id="a4dc0-120">Дата и время истечения срока действия учетных данных.</span><span class="sxs-lookup"><span data-stu-id="a4dc0-120">The date and time at which the credential expires.</span></span> <span data-ttu-id="a4dc0-121">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a4dc0-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a4dc0-122">Например, полночь UTC 1 января 2014 г. выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="a4dc0-122">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="a4dc0-123">keyId</span><span class="sxs-lookup"><span data-stu-id="a4dc0-123">keyId</span></span>|<span data-ttu-id="a4dc0-124">Guid</span><span class="sxs-lookup"><span data-stu-id="a4dc0-124">Guid</span></span>|<span data-ttu-id="a4dc0-125">Уникальный идентификатор (GUID) для ключа.</span><span class="sxs-lookup"><span data-stu-id="a4dc0-125">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="a4dc0-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a4dc0-126">startDateTime</span></span>|<span data-ttu-id="a4dc0-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4dc0-127">DateTimeOffset</span></span>|<span data-ttu-id="a4dc0-128">Дата и время, в течение которых учетные данные становятся действительными.</span><span class="sxs-lookup"><span data-stu-id="a4dc0-128">The date and time at which the credential becomes valid.</span></span> <span data-ttu-id="a4dc0-129">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a4dc0-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a4dc0-130">Например, полночь UTC 1 января 2014 г. выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="a4dc0-130">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="a4dc0-131">type</span><span class="sxs-lookup"><span data-stu-id="a4dc0-131">type</span></span>|<span data-ttu-id="a4dc0-132">Строка</span><span class="sxs-lookup"><span data-stu-id="a4dc0-132">String</span></span>|<span data-ttu-id="a4dc0-133">Тип учетных данных ключей.</span><span class="sxs-lookup"><span data-stu-id="a4dc0-133">The type of key credential.</span></span> <span data-ttu-id="a4dc0-134">"AsymmetricX509Cert".</span><span class="sxs-lookup"><span data-stu-id="a4dc0-134">"AsymmetricX509Cert".</span></span>|
|<span data-ttu-id="a4dc0-135">использование</span><span class="sxs-lookup"><span data-stu-id="a4dc0-135">usage</span></span>|<span data-ttu-id="a4dc0-136">Строка</span><span class="sxs-lookup"><span data-stu-id="a4dc0-136">String</span></span>|<span data-ttu-id="a4dc0-137">Строка, описываемая цель, для которой можно использовать ключ.</span><span class="sxs-lookup"><span data-stu-id="a4dc0-137">A string that describes the purpose for which the key can be used.</span></span> <span data-ttu-id="a4dc0-138">Например, "Проверка".</span><span class="sxs-lookup"><span data-stu-id="a4dc0-138">For example, "Verify".</span></span>|
|<span data-ttu-id="a4dc0-139">key</span><span class="sxs-lookup"><span data-stu-id="a4dc0-139">key</span></span>|<span data-ttu-id="a4dc0-140">Двоичный</span><span class="sxs-lookup"><span data-stu-id="a4dc0-140">Binary</span></span>| <span data-ttu-id="a4dc0-141">Значение для учетных данных ключа.</span><span class="sxs-lookup"><span data-stu-id="a4dc0-141">The value for the key credential.</span></span> <span data-ttu-id="a4dc0-142">Должно быть закодированное значение base-64.</span><span class="sxs-lookup"><span data-stu-id="a4dc0-142">Should be a base-64 encoded value.</span></span> |
|<span data-ttu-id="a4dc0-143">отпечатки пальцев</span><span class="sxs-lookup"><span data-stu-id="a4dc0-143">thumbprint</span></span>| <span data-ttu-id="a4dc0-144">Строка</span><span class="sxs-lookup"><span data-stu-id="a4dc0-144">String</span></span> | <span data-ttu-id="a4dc0-145">Значение отпечатка пальца для ключа.</span><span class="sxs-lookup"><span data-stu-id="a4dc0-145">The thumbprint value for the key.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4dc0-146">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a4dc0-146">JSON representation</span></span>

<span data-ttu-id="a4dc0-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4dc0-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.selfSignedCertificate"
}-->

```json
{
    "customKeyIdentifier": "string (binary)",
    "displayName": "string",
    "endDateTime": "string (timestamp)",
    "key": "string (binary)",
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

