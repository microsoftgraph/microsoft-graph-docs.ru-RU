---
title: Тип ресурса Трустфрамеворккэй
description: Представляет объект ЖВК (веб-ключ JSON). Трустфрамеворккэй — это структура данных JSON, представляющая ключ шифрования. Структура этого ресурса соответствует формату, определенному в разделе 4 RFC 7517.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7d61548707d9530d30f81b61ad88dd29ae2576c8
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734699"
---
# <a name="trustframeworkkey-resource-type"></a><span data-ttu-id="fffd4-105">Тип ресурса Трустфрамеворккэй</span><span class="sxs-lookup"><span data-stu-id="fffd4-105">trustFrameworkKey resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fffd4-106">Представляет объект ЖВК (веб-ключ JSON).</span><span class="sxs-lookup"><span data-stu-id="fffd4-106">Represents a JWK (JSON Web Key).</span></span> <span data-ttu-id="fffd4-107">Трустфрамеворккэй — это структура данных JSON, представляющая ключ шифрования.</span><span class="sxs-lookup"><span data-stu-id="fffd4-107">TrustFrameworkKey is a JSON data structure that represents a cryptographic key.</span></span> <span data-ttu-id="fffd4-108">Структура этого ресурса соответствует формату, определенному в [разделе 4 RFC 7517](https://tools.ietf.org/html/rfc7517#section-4).</span><span class="sxs-lookup"><span data-stu-id="fffd4-108">The structure of this resource follows the format defined in [RFC 7517 Section 4](https://tools.ietf.org/html/rfc7517#section-4).</span></span>

## <a name="properties"></a><span data-ttu-id="fffd4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fffd4-109">Properties</span></span>

| <span data-ttu-id="fffd4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fffd4-110">Property</span></span>     | <span data-ttu-id="fffd4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fffd4-111">Type</span></span>        | <span data-ttu-id="fffd4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fffd4-112">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fffd4-113">детей</span><span class="sxs-lookup"><span data-stu-id="fffd4-113">kid</span></span> | <span data-ttu-id="fffd4-114">string</span><span class="sxs-lookup"><span data-stu-id="fffd4-114">string</span></span> | <span data-ttu-id="fffd4-115">Уникальный идентификатор ключа.</span><span class="sxs-lookup"><span data-stu-id="fffd4-115">The unique identifier for the key.</span></span>   |
| <span data-ttu-id="fffd4-116">кти</span><span class="sxs-lookup"><span data-stu-id="fffd4-116">kty</span></span> | <span data-ttu-id="fffd4-117">string</span><span class="sxs-lookup"><span data-stu-id="fffd4-117">string</span></span> | <span data-ttu-id="fffd4-118">Параметр "КТИ" (тип ключа) определяет семейство алгоритмов шифрования, используемое с ключом, допустимые значения: RSA, Oct.</span><span class="sxs-lookup"><span data-stu-id="fffd4-118">The "kty" (key type) parameter identifies the cryptographic algorithm family used with the key, The valid values are rsa, oct.</span></span> |
| <span data-ttu-id="fffd4-119">Используйте</span><span class="sxs-lookup"><span data-stu-id="fffd4-119">use</span></span> | <span data-ttu-id="fffd4-120">string</span><span class="sxs-lookup"><span data-stu-id="fffd4-120">string</span></span> | <span data-ttu-id="fffd4-121">Параметр "use" (использование открытого ключа) определяет предполагаемое использование открытого ключа.</span><span class="sxs-lookup"><span data-stu-id="fffd4-121">The "use" (public key use) parameter identifies the intended use of the public key.</span></span>  <span data-ttu-id="fffd4-122">Параметр Use используется, чтобы указать, используется ли открытый ключ для шифрования данных или проверки подписи данных.</span><span class="sxs-lookup"><span data-stu-id="fffd4-122">The "use" parameter is employed to indicate whether a public key is used for encrypting data or verifying the signature on data.</span></span> <span data-ttu-id="fffd4-123">Возможные значения: 1.</span><span class="sxs-lookup"><span data-stu-id="fffd4-123">Possible values are    1.</span></span> <span data-ttu-id="fffd4-124">"SIG" (Подпись) 2.</span><span class="sxs-lookup"><span data-stu-id="fffd4-124">"sig" (signature)    2.</span></span>  <span data-ttu-id="fffd4-125">"ENC" (шифрование)</span><span class="sxs-lookup"><span data-stu-id="fffd4-125">"enc" (encryption)</span></span>   |
| <span data-ttu-id="fffd4-126">x5c</span><span class="sxs-lookup"><span data-stu-id="fffd4-126">x5c</span></span> | <span data-ttu-id="fffd4-127">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fffd4-127">string collection</span></span> | <span data-ttu-id="fffd4-128">Параметр "x5c" (цепочка сертификатов X. 509) содержит цепочку из одного или нескольких сертификатов ПКИКС [RFC 5280](https://tools.ietf.org/html/rfc5280).</span><span class="sxs-lookup"><span data-stu-id="fffd4-128">The "x5c" (X.509 certificate chain) parameter contains a chain of one or more PKIX certificates [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="fffd4-129">x5t</span><span class="sxs-lookup"><span data-stu-id="fffd4-129">x5t</span></span> | <span data-ttu-id="fffd4-130">string</span><span class="sxs-lookup"><span data-stu-id="fffd4-130">string</span></span> | <span data-ttu-id="fffd4-131">Параметр "x5t" (отпечаток сертификата X. 509) — это отпечаток SHA-1, закодированный с помощью base64decode.</span><span class="sxs-lookup"><span data-stu-id="fffd4-131">The "x5t" (X.509 certificate SHA-1 thumbprint) parameter is a base64url-encoded SHA-1 thumbprint (a.k.a.</span></span> <span data-ttu-id="fffd4-132">Дайджест) кодировки DER для сертификата X. 509, [RFC 5280](https://tools.ietf.org/html/rfc5280).</span><span class="sxs-lookup"><span data-stu-id="fffd4-132">digest) of the DER encoding of an X.509 certificate [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="fffd4-133">e</span><span class="sxs-lookup"><span data-stu-id="fffd4-133">e</span></span> | <span data-ttu-id="fffd4-134">string</span><span class="sxs-lookup"><span data-stu-id="fffd4-134">string</span></span> | <span data-ttu-id="fffd4-135">Ключ RSA — открытый показатель степени</span><span class="sxs-lookup"><span data-stu-id="fffd4-135">RSA Key - public exponent</span></span> |
| <span data-ttu-id="fffd4-136">d</span><span class="sxs-lookup"><span data-stu-id="fffd4-136">d</span></span>| <span data-ttu-id="fffd4-137">string</span><span class="sxs-lookup"><span data-stu-id="fffd4-137">string</span></span> | <span data-ttu-id="fffd4-138">Закрытый показатель ключа RSA.</span><span class="sxs-lookup"><span data-stu-id="fffd4-138">RSA Key - private exponent.</span></span> <span data-ttu-id="fffd4-139">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="fffd4-139">Field cannot be read back.</span></span> |
| <span data-ttu-id="fffd4-140">n</span><span class="sxs-lookup"><span data-stu-id="fffd4-140">n</span></span> | <span data-ttu-id="fffd4-141">string</span><span class="sxs-lookup"><span data-stu-id="fffd4-141">string</span></span> | <span data-ttu-id="fffd4-142">Ключ RSA — модуль</span><span class="sxs-lookup"><span data-stu-id="fffd4-142">RSA Key - modulus</span></span> |
| <span data-ttu-id="fffd4-143">p</span><span class="sxs-lookup"><span data-stu-id="fffd4-143">p</span></span> | <span data-ttu-id="fffd4-144">string</span><span class="sxs-lookup"><span data-stu-id="fffd4-144">string</span></span> | <span data-ttu-id="fffd4-145">Первый простой ключ RSA.</span><span class="sxs-lookup"><span data-stu-id="fffd4-145">RSA Key - first prime.</span></span> <span data-ttu-id="fffd4-146">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="fffd4-146">Field cannot be read back.</span></span> |
| <span data-ttu-id="fffd4-147">q</span><span class="sxs-lookup"><span data-stu-id="fffd4-147">q</span></span> | <span data-ttu-id="fffd4-148">string</span><span class="sxs-lookup"><span data-stu-id="fffd4-148">string</span></span> | <span data-ttu-id="fffd4-149">Клавиша RSA, простое в секунду.</span><span class="sxs-lookup"><span data-stu-id="fffd4-149">RSA Key - second prime.</span></span> <span data-ttu-id="fffd4-150">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="fffd4-150">Field cannot be read back.</span></span> |
| <span data-ttu-id="fffd4-151">двухпроцессорный</span><span class="sxs-lookup"><span data-stu-id="fffd4-151">dp</span></span> | <span data-ttu-id="fffd4-152">string</span><span class="sxs-lookup"><span data-stu-id="fffd4-152">string</span></span> | <span data-ttu-id="fffd4-153">Экспонента RSA Key — первый показатель.</span><span class="sxs-lookup"><span data-stu-id="fffd4-153">RSA Key - first exponent.</span></span> <span data-ttu-id="fffd4-154">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="fffd4-154">Field cannot be read back.</span></span> |
| <span data-ttu-id="fffd4-155">DQ</span><span class="sxs-lookup"><span data-stu-id="fffd4-155">dq</span></span> | <span data-ttu-id="fffd4-156">string</span><span class="sxs-lookup"><span data-stu-id="fffd4-156">string</span></span> | <span data-ttu-id="fffd4-157">Экспонента RSA Key — секунды.</span><span class="sxs-lookup"><span data-stu-id="fffd4-157">RSA Key - second exponent.</span></span> <span data-ttu-id="fffd4-158">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="fffd4-158">Field cannot be read back.</span></span> |
| <span data-ttu-id="fffd4-159">типом</span><span class="sxs-lookup"><span data-stu-id="fffd4-159">qi</span></span> | <span data-ttu-id="fffd4-160">string</span><span class="sxs-lookup"><span data-stu-id="fffd4-160">string</span></span> | <span data-ttu-id="fffd4-161">Ключ RSA Key — коэффициент.</span><span class="sxs-lookup"><span data-stu-id="fffd4-161">RSA Key - Coefficient.</span></span> <span data-ttu-id="fffd4-162">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="fffd4-162">Field cannot be read back.</span></span> |
| <span data-ttu-id="fffd4-163">звонить</span><span class="sxs-lookup"><span data-stu-id="fffd4-163">k</span></span> | <span data-ttu-id="fffd4-164">string</span><span class="sxs-lookup"><span data-stu-id="fffd4-164">string</span></span> | <span data-ttu-id="fffd4-165">Симметричный ключ для типа ключа центра развертывания Office.</span><span class="sxs-lookup"><span data-stu-id="fffd4-165">Symmetric Key for oct key type.</span></span> <span data-ttu-id="fffd4-166">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="fffd4-166">Field cannot be read back.</span></span>   |
| <span data-ttu-id="fffd4-167">nbf</span><span class="sxs-lookup"><span data-stu-id="fffd4-167">nbf</span></span> | <span data-ttu-id="fffd4-168">int</span><span class="sxs-lookup"><span data-stu-id="fffd4-168">int</span></span> | <span data-ttu-id="fffd4-169">Это значение является Нумерикдате, как определено в RFC 7519 (числовое значение JSON, представляющее число секунд от 1970 до 01-01T00:00:00Z UTC до указанной даты и времени в формате UTC, игнорируя високосные секунды.)</span><span class="sxs-lookup"><span data-stu-id="fffd4-169">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |
| <span data-ttu-id="fffd4-170">exp</span><span class="sxs-lookup"><span data-stu-id="fffd4-170">exp</span></span> | <span data-ttu-id="fffd4-171">int</span><span class="sxs-lookup"><span data-stu-id="fffd4-171">int</span></span> | <span data-ttu-id="fffd4-172">Это значение является Нумерикдате, как определено в RFC 7519 (числовое значение JSON, представляющее число секунд от 1970 до 01-01T00:00:00Z UTC до указанной даты и времени в формате UTC, игнорируя високосные секунды.)</span><span class="sxs-lookup"><span data-stu-id="fffd4-172">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |



## <a name="json-representation"></a><span data-ttu-id="fffd4-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fffd4-173">JSON representation</span></span>

<span data-ttu-id="fffd4-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fffd4-174">The following is a JSON representation of the resource.</span></span>

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
