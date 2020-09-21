---
title: Тип ресурса Трустфрамеворккэй
description: Представляет объект ЖВК (веб-ключ JSON). Трустфрамеворккэй — это структура данных JSON, представляющая ключ шифрования. Структура этого ресурса соответствует формату, определенному в разделе 4 RFC 7517.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7650976a437eb862acd5994d7e1dd14830d5e3b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083934"
---
# <a name="trustframeworkkey-resource-type"></a><span data-ttu-id="2d435-105">Тип ресурса Трустфрамеворккэй</span><span class="sxs-lookup"><span data-stu-id="2d435-105">trustFrameworkKey resource type</span></span>

<span data-ttu-id="2d435-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d435-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d435-107">Представляет объект ЖВК (веб-ключ JSON).</span><span class="sxs-lookup"><span data-stu-id="2d435-107">Represents a JWK (JSON Web Key).</span></span> <span data-ttu-id="2d435-108">Трустфрамеворккэй — это структура данных JSON, представляющая ключ шифрования.</span><span class="sxs-lookup"><span data-stu-id="2d435-108">TrustFrameworkKey is a JSON data structure that represents a cryptographic key.</span></span> <span data-ttu-id="2d435-109">Структура этого ресурса соответствует формату, определенному в [разделе 4 RFC 7517](https://tools.ietf.org/html/rfc7517#section-4).</span><span class="sxs-lookup"><span data-stu-id="2d435-109">The structure of this resource follows the format defined in [RFC 7517 Section 4](https://tools.ietf.org/html/rfc7517#section-4).</span></span>

## <a name="properties"></a><span data-ttu-id="2d435-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d435-110">Properties</span></span>

| <span data-ttu-id="2d435-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d435-111">Property</span></span>     | <span data-ttu-id="2d435-112">Тип</span><span class="sxs-lookup"><span data-stu-id="2d435-112">Type</span></span>        | <span data-ttu-id="2d435-113">Описание</span><span class="sxs-lookup"><span data-stu-id="2d435-113">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2d435-114">детей</span><span class="sxs-lookup"><span data-stu-id="2d435-114">kid</span></span> | <span data-ttu-id="2d435-115">string</span><span class="sxs-lookup"><span data-stu-id="2d435-115">string</span></span> | <span data-ttu-id="2d435-116">Уникальный идентификатор ключа.</span><span class="sxs-lookup"><span data-stu-id="2d435-116">The unique identifier for the key.</span></span>   |
| <span data-ttu-id="2d435-117">кти</span><span class="sxs-lookup"><span data-stu-id="2d435-117">kty</span></span> | <span data-ttu-id="2d435-118">string</span><span class="sxs-lookup"><span data-stu-id="2d435-118">string</span></span> | <span data-ttu-id="2d435-119">Параметр "КТИ" (тип ключа) определяет семейство алгоритмов шифрования, используемое с ключом, допустимые значения: RSA, Oct.</span><span class="sxs-lookup"><span data-stu-id="2d435-119">The "kty" (key type) parameter identifies the cryptographic algorithm family used with the key, The valid values are rsa, oct.</span></span> |
| <span data-ttu-id="2d435-120">Используйте</span><span class="sxs-lookup"><span data-stu-id="2d435-120">use</span></span> | <span data-ttu-id="2d435-121">string</span><span class="sxs-lookup"><span data-stu-id="2d435-121">string</span></span> | <span data-ttu-id="2d435-122">Параметр "use" (использование открытого ключа) определяет предполагаемое использование открытого ключа.</span><span class="sxs-lookup"><span data-stu-id="2d435-122">The "use" (public key use) parameter identifies the intended use of the public key.</span></span>  <span data-ttu-id="2d435-123">Параметр Use используется, чтобы указать, используется ли открытый ключ для шифрования данных или проверки подписи данных.</span><span class="sxs-lookup"><span data-stu-id="2d435-123">The "use" parameter is employed to indicate whether a public key is used for encrypting data or verifying the signature on data.</span></span> <span data-ttu-id="2d435-124">Возможные значения: 1.</span><span class="sxs-lookup"><span data-stu-id="2d435-124">Possible values are    1.</span></span> <span data-ttu-id="2d435-125">"SIG" (Подпись) 2.</span><span class="sxs-lookup"><span data-stu-id="2d435-125">"sig" (signature)    2.</span></span>  <span data-ttu-id="2d435-126">"ENC" (шифрование)</span><span class="sxs-lookup"><span data-stu-id="2d435-126">"enc" (encryption)</span></span>   |
| <span data-ttu-id="2d435-127">x5c</span><span class="sxs-lookup"><span data-stu-id="2d435-127">x5c</span></span> | <span data-ttu-id="2d435-128">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2d435-128">string collection</span></span> | <span data-ttu-id="2d435-129">Параметр "x5c" (цепочка сертификатов X. 509) содержит цепочку из одного или нескольких сертификатов ПКИКС [RFC 5280](https://tools.ietf.org/html/rfc5280).</span><span class="sxs-lookup"><span data-stu-id="2d435-129">The "x5c" (X.509 certificate chain) parameter contains a chain of one or more PKIX certificates [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="2d435-130">x5t</span><span class="sxs-lookup"><span data-stu-id="2d435-130">x5t</span></span> | <span data-ttu-id="2d435-131">string</span><span class="sxs-lookup"><span data-stu-id="2d435-131">string</span></span> | <span data-ttu-id="2d435-132">Параметр "x5t" (отпечаток сертификата X. 509) — это отпечаток SHA-1, закодированный с помощью base64decode.</span><span class="sxs-lookup"><span data-stu-id="2d435-132">The "x5t" (X.509 certificate SHA-1 thumbprint) parameter is a base64url-encoded SHA-1 thumbprint (a.k.a.</span></span> <span data-ttu-id="2d435-133">Дайджест) кодировки DER для сертификата X. 509, [RFC 5280](https://tools.ietf.org/html/rfc5280).</span><span class="sxs-lookup"><span data-stu-id="2d435-133">digest) of the DER encoding of an X.509 certificate [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="2d435-134">e</span><span class="sxs-lookup"><span data-stu-id="2d435-134">e</span></span> | <span data-ttu-id="2d435-135">string</span><span class="sxs-lookup"><span data-stu-id="2d435-135">string</span></span> | <span data-ttu-id="2d435-136">Ключ RSA — открытый показатель степени</span><span class="sxs-lookup"><span data-stu-id="2d435-136">RSA Key - public exponent</span></span> |
| <span data-ttu-id="2d435-137">d</span><span class="sxs-lookup"><span data-stu-id="2d435-137">d</span></span>| <span data-ttu-id="2d435-138">string</span><span class="sxs-lookup"><span data-stu-id="2d435-138">string</span></span> | <span data-ttu-id="2d435-139">Закрытый показатель ключа RSA.</span><span class="sxs-lookup"><span data-stu-id="2d435-139">RSA Key - private exponent.</span></span> <span data-ttu-id="2d435-140">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="2d435-140">Field cannot be read back.</span></span> |
| <span data-ttu-id="2d435-141">n</span><span class="sxs-lookup"><span data-stu-id="2d435-141">n</span></span> | <span data-ttu-id="2d435-142">string</span><span class="sxs-lookup"><span data-stu-id="2d435-142">string</span></span> | <span data-ttu-id="2d435-143">Ключ RSA — модуль</span><span class="sxs-lookup"><span data-stu-id="2d435-143">RSA Key - modulus</span></span> |
| <span data-ttu-id="2d435-144">p</span><span class="sxs-lookup"><span data-stu-id="2d435-144">p</span></span> | <span data-ttu-id="2d435-145">string</span><span class="sxs-lookup"><span data-stu-id="2d435-145">string</span></span> | <span data-ttu-id="2d435-146">Первый простой ключ RSA.</span><span class="sxs-lookup"><span data-stu-id="2d435-146">RSA Key - first prime.</span></span> <span data-ttu-id="2d435-147">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="2d435-147">Field cannot be read back.</span></span> |
| <span data-ttu-id="2d435-148">q</span><span class="sxs-lookup"><span data-stu-id="2d435-148">q</span></span> | <span data-ttu-id="2d435-149">string</span><span class="sxs-lookup"><span data-stu-id="2d435-149">string</span></span> | <span data-ttu-id="2d435-150">Клавиша RSA, простое в секунду.</span><span class="sxs-lookup"><span data-stu-id="2d435-150">RSA Key - second prime.</span></span> <span data-ttu-id="2d435-151">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="2d435-151">Field cannot be read back.</span></span> |
| <span data-ttu-id="2d435-152">двухпроцессорный</span><span class="sxs-lookup"><span data-stu-id="2d435-152">dp</span></span> | <span data-ttu-id="2d435-153">string</span><span class="sxs-lookup"><span data-stu-id="2d435-153">string</span></span> | <span data-ttu-id="2d435-154">Экспонента RSA Key — первый показатель.</span><span class="sxs-lookup"><span data-stu-id="2d435-154">RSA Key - first exponent.</span></span> <span data-ttu-id="2d435-155">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="2d435-155">Field cannot be read back.</span></span> |
| <span data-ttu-id="2d435-156">DQ</span><span class="sxs-lookup"><span data-stu-id="2d435-156">dq</span></span> | <span data-ttu-id="2d435-157">string</span><span class="sxs-lookup"><span data-stu-id="2d435-157">string</span></span> | <span data-ttu-id="2d435-158">Экспонента RSA Key — секунды.</span><span class="sxs-lookup"><span data-stu-id="2d435-158">RSA Key - second exponent.</span></span> <span data-ttu-id="2d435-159">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="2d435-159">Field cannot be read back.</span></span> |
| <span data-ttu-id="2d435-160">типом</span><span class="sxs-lookup"><span data-stu-id="2d435-160">qi</span></span> | <span data-ttu-id="2d435-161">string</span><span class="sxs-lookup"><span data-stu-id="2d435-161">string</span></span> | <span data-ttu-id="2d435-162">Ключ RSA Key — коэффициент.</span><span class="sxs-lookup"><span data-stu-id="2d435-162">RSA Key - Coefficient.</span></span> <span data-ttu-id="2d435-163">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="2d435-163">Field cannot be read back.</span></span> |
| <span data-ttu-id="2d435-164">звонить</span><span class="sxs-lookup"><span data-stu-id="2d435-164">k</span></span> | <span data-ttu-id="2d435-165">string</span><span class="sxs-lookup"><span data-stu-id="2d435-165">string</span></span> | <span data-ttu-id="2d435-166">Симметричный ключ для типа ключа центра развертывания Office.</span><span class="sxs-lookup"><span data-stu-id="2d435-166">Symmetric Key for oct key type.</span></span> <span data-ttu-id="2d435-167">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="2d435-167">Field cannot be read back.</span></span>   |
| <span data-ttu-id="2d435-168">nbf</span><span class="sxs-lookup"><span data-stu-id="2d435-168">nbf</span></span> | <span data-ttu-id="2d435-169">int</span><span class="sxs-lookup"><span data-stu-id="2d435-169">int</span></span> | <span data-ttu-id="2d435-170">Это значение является Нумерикдате, как определено в RFC 7519 (числовое значение JSON, представляющее число секунд от 1970 до 01-01T00:00:00Z UTC до указанной даты и времени в формате UTC, игнорируя високосные секунды.)</span><span class="sxs-lookup"><span data-stu-id="2d435-170">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |
| <span data-ttu-id="2d435-171">exp</span><span class="sxs-lookup"><span data-stu-id="2d435-171">exp</span></span> | <span data-ttu-id="2d435-172">int</span><span class="sxs-lookup"><span data-stu-id="2d435-172">int</span></span> | <span data-ttu-id="2d435-173">Это значение является Нумерикдате, как определено в RFC 7519 (числовое значение JSON, представляющее число секунд от 1970 до 01-01T00:00:00Z UTC до указанной даты и времени в формате UTC, игнорируя високосные секунды.)</span><span class="sxs-lookup"><span data-stu-id="2d435-173">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |



## <a name="json-representation"></a><span data-ttu-id="2d435-174">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2d435-174">JSON representation</span></span>

<span data-ttu-id="2d435-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d435-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKey",
  "baseType": null
}-->

```json
{
  "d": "String",
  "dp": "String",
  "dq": "String",
  "e": "String",
  "exp": 1024,
  "k": "String",
  "kid": "String",
  "kty": "String",
  "n": "String",
  "nbf": 1024,
  "p": "String",
  "q": "String",
  "qi": "String",
  "use": "String",
  "x5c": ["String"],
  "x5t": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKey resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


