---
title: тип ресурса selfSignedCertificate
description: Содержит сведения о публичной части сертификата подписи.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: luleonpla
ms.openlocfilehash: 641748720be99272569c08874d91be7b7bb56888
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469033"
---
# <a name="selfsignedcertificate-resource-type"></a><span data-ttu-id="809f1-103">тип ресурса selfSignedCertificate</span><span class="sxs-lookup"><span data-stu-id="809f1-103">selfSignedCertificate resource type</span></span>

<span data-ttu-id="809f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="809f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="809f1-105">Содержит публичную часть сертификата подписи.</span><span class="sxs-lookup"><span data-stu-id="809f1-105">Contains the public part of a signing certificate.</span></span> <span data-ttu-id="809f1-106">Это возвращающий тип действия [addSelfSignedSigningCertificate.](../api/serviceprincipal-addtokensigningcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="809f1-106">It's the return type of the action [addSelfSignedSigningCertificate](../api/serviceprincipal-addtokensigningcertificate.md).</span></span> <span data-ttu-id="809f1-107">Поставщики услуг используют публичную часть сертификата подписи для проверки эмитента маркера.</span><span class="sxs-lookup"><span data-stu-id="809f1-107">Service providers use the the public part of the signing certificate to validate the issuer of the token.</span></span>

## <a name="properties"></a><span data-ttu-id="809f1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="809f1-108">Properties</span></span>
<span data-ttu-id="809f1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="809f1-109">Property</span></span>|<span data-ttu-id="809f1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="809f1-110">Type</span></span>|<span data-ttu-id="809f1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="809f1-111">Description</span></span>
----|--|---
|<span data-ttu-id="809f1-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="809f1-112">customKeyIdentifier</span></span>|<span data-ttu-id="809f1-113">В двоичном формате</span><span class="sxs-lookup"><span data-stu-id="809f1-113">Binary</span></span>| <span data-ttu-id="809f1-114">Настраиваемый идентификатор ключа</span><span class="sxs-lookup"><span data-stu-id="809f1-114">Custom key identifier</span></span> |
| <span data-ttu-id="809f1-115">displayName</span><span class="sxs-lookup"><span data-stu-id="809f1-115">displayName</span></span> | <span data-ttu-id="809f1-116">String</span><span class="sxs-lookup"><span data-stu-id="809f1-116">String</span></span> | <span data-ttu-id="809f1-117">Удобное имя для ключа.</span><span class="sxs-lookup"><span data-stu-id="809f1-117">The friendly name for the key.</span></span> |
|<span data-ttu-id="809f1-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="809f1-118">endDateTime</span></span>|<span data-ttu-id="809f1-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="809f1-119">DateTimeOffset</span></span>|<span data-ttu-id="809f1-120">Дата и время истечения срока действия учетных данных. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="809f1-120">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="809f1-121">Например, полночь UTC 1 января 2014 г. выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="809f1-121">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="809f1-122">keyId</span><span class="sxs-lookup"><span data-stu-id="809f1-122">keyId</span></span>|<span data-ttu-id="809f1-123">Guid</span><span class="sxs-lookup"><span data-stu-id="809f1-123">Guid</span></span>|<span data-ttu-id="809f1-124">Уникальный идентификатор (GUID) для ключа.</span><span class="sxs-lookup"><span data-stu-id="809f1-124">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="809f1-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="809f1-125">startDateTime</span></span>|<span data-ttu-id="809f1-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="809f1-126">DateTimeOffset</span></span>|<span data-ttu-id="809f1-127">Дата и время, в течение которых учетные данные становятся действительными. Тип Timestamp представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="809f1-127">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="809f1-128">Например, полночь UTC 1 января 2014 г. выглядит так: "2014-01-01T00:00:00Z".</span><span class="sxs-lookup"><span data-stu-id="809f1-128">For example, midnight UTC on Jan 1, 2014 would look like this: "2014-01-01T00:00:00Z".</span></span> |
|<span data-ttu-id="809f1-129">type</span><span class="sxs-lookup"><span data-stu-id="809f1-129">type</span></span>|<span data-ttu-id="809f1-130">String</span><span class="sxs-lookup"><span data-stu-id="809f1-130">String</span></span>|<span data-ttu-id="809f1-131">Тип учетных данных ключей.</span><span class="sxs-lookup"><span data-stu-id="809f1-131">The type of key credential.</span></span> <span data-ttu-id="809f1-132">"AsymmetricX509Cert".</span><span class="sxs-lookup"><span data-stu-id="809f1-132">"AsymmetricX509Cert".</span></span>|
|<span data-ttu-id="809f1-133">использование</span><span class="sxs-lookup"><span data-stu-id="809f1-133">usage</span></span>|<span data-ttu-id="809f1-134">String</span><span class="sxs-lookup"><span data-stu-id="809f1-134">String</span></span>|<span data-ttu-id="809f1-135">Строка, описываемая цель, для которой можно использовать ключ.</span><span class="sxs-lookup"><span data-stu-id="809f1-135">A string that describes the purpose for which the key can be used.</span></span> <span data-ttu-id="809f1-136">Например, "Проверка".</span><span class="sxs-lookup"><span data-stu-id="809f1-136">For example, "Verify".</span></span>|
|<span data-ttu-id="809f1-137">key</span><span class="sxs-lookup"><span data-stu-id="809f1-137">key</span></span>|<span data-ttu-id="809f1-138">Двоичный</span><span class="sxs-lookup"><span data-stu-id="809f1-138">Binary</span></span>| <span data-ttu-id="809f1-139">Значение для учетных данных ключа.</span><span class="sxs-lookup"><span data-stu-id="809f1-139">The value for the key credential.</span></span> <span data-ttu-id="809f1-140">Должно быть закодированное значение base-64.</span><span class="sxs-lookup"><span data-stu-id="809f1-140">Should be a base-64 encoded value.</span></span> |
|<span data-ttu-id="809f1-141">отпечатки пальцев</span><span class="sxs-lookup"><span data-stu-id="809f1-141">thumbprint</span></span>| <span data-ttu-id="809f1-142">String</span><span class="sxs-lookup"><span data-stu-id="809f1-142">String</span></span> | <span data-ttu-id="809f1-143">Значение отпечатка пальца для ключа.</span><span class="sxs-lookup"><span data-stu-id="809f1-143">The thumbprint value for the key.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="809f1-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="809f1-144">JSON representation</span></span>

<span data-ttu-id="809f1-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="809f1-145">Here is a JSON representation of the resource</span></span>

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

