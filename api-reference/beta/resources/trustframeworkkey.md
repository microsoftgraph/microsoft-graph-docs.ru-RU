---
title: Тип ресурса trustFrameworkKey
description: Представляет JWK (веб-ключ JSON). TrustFrameworkKey — это структура данных JSON, которая представляет криптографический ключ. Структура этого ресурса следует формату, определенному в разделе 4 RFC 7517.
localization_priority: Normal
author: valnav
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3de9ce67298f31b3c40682040da69f5c2f6ba007
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135858"
---
# <a name="trustframeworkkey-resource-type"></a><span data-ttu-id="c42e1-105">Тип ресурса trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="c42e1-105">trustFrameworkKey resource type</span></span>

<span data-ttu-id="c42e1-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c42e1-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c42e1-107">Представляет JWK (веб-ключ JSON).</span><span class="sxs-lookup"><span data-stu-id="c42e1-107">Represents a JWK (JSON Web Key).</span></span> <span data-ttu-id="c42e1-108">TrustFrameworkKey — это структура данных JSON, которая представляет криптографический ключ.</span><span class="sxs-lookup"><span data-stu-id="c42e1-108">TrustFrameworkKey is a JSON data structure that represents a cryptographic key.</span></span> <span data-ttu-id="c42e1-109">Структура этого ресурса следует формату, определенному в разделе [4 RFC 7517.](https://tools.ietf.org/html/rfc7517#section-4)</span><span class="sxs-lookup"><span data-stu-id="c42e1-109">The structure of this resource follows the format defined in [RFC 7517 Section 4](https://tools.ietf.org/html/rfc7517#section-4).</span></span>

## <a name="properties"></a><span data-ttu-id="c42e1-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="c42e1-110">Properties</span></span>

| <span data-ttu-id="c42e1-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="c42e1-111">Property</span></span>     | <span data-ttu-id="c42e1-112">Тип</span><span class="sxs-lookup"><span data-stu-id="c42e1-112">Type</span></span>        | <span data-ttu-id="c42e1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="c42e1-113">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c42e1-114">1</span><span class="sxs-lookup"><span data-stu-id="c42e1-114">kid</span></span> | <span data-ttu-id="c42e1-115">string</span><span class="sxs-lookup"><span data-stu-id="c42e1-115">string</span></span> | <span data-ttu-id="c42e1-116">Уникальный идентификатор ключа.</span><span class="sxs-lookup"><span data-stu-id="c42e1-116">The unique identifier for the key.</span></span>   |
| <span data-ttu-id="c42e1-117">kty</span><span class="sxs-lookup"><span data-stu-id="c42e1-117">kty</span></span> | <span data-ttu-id="c42e1-118">string</span><span class="sxs-lookup"><span data-stu-id="c42e1-118">string</span></span> | <span data-ttu-id="c42e1-119">Параметр "kty" (тип ключа) определяет семейство криптографических алгоритмов, используемого с ключом. Допустимые значения: rsa, oct.</span><span class="sxs-lookup"><span data-stu-id="c42e1-119">The "kty" (key type) parameter identifies the cryptographic algorithm family used with the key, The valid values are rsa, oct.</span></span> |
| <span data-ttu-id="c42e1-120">use</span><span class="sxs-lookup"><span data-stu-id="c42e1-120">use</span></span> | <span data-ttu-id="c42e1-121">string</span><span class="sxs-lookup"><span data-stu-id="c42e1-121">string</span></span> | <span data-ttu-id="c42e1-122">Параметр "use" (использование открытого ключа) определяет предназначенное использование открытого ключа.</span><span class="sxs-lookup"><span data-stu-id="c42e1-122">The "use" (public key use) parameter identifies the intended use of the public key.</span></span>  <span data-ttu-id="c42e1-123">Параметр "use" используется для того, чтобы указать, используется ли открытый ключ для шифрования данных или проверки подписи данных.</span><span class="sxs-lookup"><span data-stu-id="c42e1-123">The "use" parameter is employed to indicate whether a public key is used for encrypting data or verifying the signature on data.</span></span> <span data-ttu-id="c42e1-124">Возможные значения: 1.</span><span class="sxs-lookup"><span data-stu-id="c42e1-124">Possible values are    1.</span></span> <span data-ttu-id="c42e1-125">"sig" (подпись) 2.</span><span class="sxs-lookup"><span data-stu-id="c42e1-125">"sig" (signature)    2.</span></span>  <span data-ttu-id="c42e1-126">"enc" (шифрование)</span><span class="sxs-lookup"><span data-stu-id="c42e1-126">"enc" (encryption)</span></span>   |
| <span data-ttu-id="c42e1-127">x5c</span><span class="sxs-lookup"><span data-stu-id="c42e1-127">x5c</span></span> | <span data-ttu-id="c42e1-128">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c42e1-128">string collection</span></span> | <span data-ttu-id="c42e1-129">Параметр "x5c" (цепочка сертификатов X.509) содержит цепочку из одного или более сертификатов [PKIX RFC 5280.](https://tools.ietf.org/html/rfc5280)</span><span class="sxs-lookup"><span data-stu-id="c42e1-129">The "x5c" (X.509 certificate chain) parameter contains a chain of one or more PKIX certificates [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="c42e1-130">x5t</span><span class="sxs-lookup"><span data-stu-id="c42e1-130">x5t</span></span> | <span data-ttu-id="c42e1-131">string</span><span class="sxs-lookup"><span data-stu-id="c42e1-131">string</span></span> | <span data-ttu-id="c42e1-132">Параметр "x5t" (отпечаток сертификата SHA-1 X.509) — это отпечаток SHA-1 в коде base64url (т. е. отпечаток SHA-1).</span><span class="sxs-lookup"><span data-stu-id="c42e1-132">The "x5t" (X.509 certificate SHA-1 thumbprint) parameter is a base64url-encoded SHA-1 thumbprint (a.k.a.</span></span> <span data-ttu-id="c42e1-133">дайджест) кодив der сертификата X.509 [RFC 5280.](https://tools.ietf.org/html/rfc5280)</span><span class="sxs-lookup"><span data-stu-id="c42e1-133">digest) of the DER encoding of an X.509 certificate [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="c42e1-134">e</span><span class="sxs-lookup"><span data-stu-id="c42e1-134">e</span></span> | <span data-ttu-id="c42e1-135">string</span><span class="sxs-lookup"><span data-stu-id="c42e1-135">string</span></span> | <span data-ttu-id="c42e1-136">Ключ RSA — открытый экспонент</span><span class="sxs-lookup"><span data-stu-id="c42e1-136">RSA Key - public exponent</span></span> |
| <span data-ttu-id="c42e1-137">d</span><span class="sxs-lookup"><span data-stu-id="c42e1-137">d</span></span>| <span data-ttu-id="c42e1-138">string</span><span class="sxs-lookup"><span data-stu-id="c42e1-138">string</span></span> | <span data-ttu-id="c42e1-139">Ключ RSA — частный экспонент.</span><span class="sxs-lookup"><span data-stu-id="c42e1-139">RSA Key - private exponent.</span></span> <span data-ttu-id="c42e1-140">Поле не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="c42e1-140">Field cannot be read back.</span></span> |
| <span data-ttu-id="c42e1-141">n</span><span class="sxs-lookup"><span data-stu-id="c42e1-141">n</span></span> | <span data-ttu-id="c42e1-142">string</span><span class="sxs-lookup"><span data-stu-id="c42e1-142">string</span></span> | <span data-ttu-id="c42e1-143">Ключ RSA — модулю</span><span class="sxs-lookup"><span data-stu-id="c42e1-143">RSA Key - modulus</span></span> |
| <span data-ttu-id="c42e1-144">p</span><span class="sxs-lookup"><span data-stu-id="c42e1-144">p</span></span> | <span data-ttu-id="c42e1-145">string</span><span class="sxs-lookup"><span data-stu-id="c42e1-145">string</span></span> | <span data-ttu-id="c42e1-146">Ключ RSA — первый простор.</span><span class="sxs-lookup"><span data-stu-id="c42e1-146">RSA Key - first prime.</span></span> <span data-ttu-id="c42e1-147">Поле не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="c42e1-147">Field cannot be read back.</span></span> |
| <span data-ttu-id="c42e1-148">q</span><span class="sxs-lookup"><span data-stu-id="c42e1-148">q</span></span> | <span data-ttu-id="c42e1-149">string</span><span class="sxs-lookup"><span data-stu-id="c42e1-149">string</span></span> | <span data-ttu-id="c42e1-150">Клавиша RSA — second prime.</span><span class="sxs-lookup"><span data-stu-id="c42e1-150">RSA Key - second prime.</span></span> <span data-ttu-id="c42e1-151">Поле не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="c42e1-151">Field cannot be read back.</span></span> |
| <span data-ttu-id="c42e1-152">dp</span><span class="sxs-lookup"><span data-stu-id="c42e1-152">dp</span></span> | <span data-ttu-id="c42e1-153">string</span><span class="sxs-lookup"><span data-stu-id="c42e1-153">string</span></span> | <span data-ttu-id="c42e1-154">Ключ RSA — первый показатель.</span><span class="sxs-lookup"><span data-stu-id="c42e1-154">RSA Key - first exponent.</span></span> <span data-ttu-id="c42e1-155">Поле не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="c42e1-155">Field cannot be read back.</span></span> |
| <span data-ttu-id="c42e1-156">dq</span><span class="sxs-lookup"><span data-stu-id="c42e1-156">dq</span></span> | <span data-ttu-id="c42e1-157">string</span><span class="sxs-lookup"><span data-stu-id="c42e1-157">string</span></span> | <span data-ttu-id="c42e1-158">Ключ RSA — второй показатель.</span><span class="sxs-lookup"><span data-stu-id="c42e1-158">RSA Key - second exponent.</span></span> <span data-ttu-id="c42e1-159">Поле не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="c42e1-159">Field cannot be read back.</span></span> |
| <span data-ttu-id="c42e1-160">фа</span><span class="sxs-lookup"><span data-stu-id="c42e1-160">qi</span></span> | <span data-ttu-id="c42e1-161">string</span><span class="sxs-lookup"><span data-stu-id="c42e1-161">string</span></span> | <span data-ttu-id="c42e1-162">Ключ RSA — коэффициент.</span><span class="sxs-lookup"><span data-stu-id="c42e1-162">RSA Key - Coefficient.</span></span> <span data-ttu-id="c42e1-163">Поле не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="c42e1-163">Field cannot be read back.</span></span> |
| <span data-ttu-id="c42e1-164">k</span><span class="sxs-lookup"><span data-stu-id="c42e1-164">k</span></span> | <span data-ttu-id="c42e1-165">string</span><span class="sxs-lookup"><span data-stu-id="c42e1-165">string</span></span> | <span data-ttu-id="c42e1-166">Симметричный ключ для типа клавиши oct.</span><span class="sxs-lookup"><span data-stu-id="c42e1-166">Symmetric Key for oct key type.</span></span> <span data-ttu-id="c42e1-167">Поле не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="c42e1-167">Field cannot be read back.</span></span>   |
| <span data-ttu-id="c42e1-168">nbf</span><span class="sxs-lookup"><span data-stu-id="c42e1-168">nbf</span></span> | <span data-ttu-id="c42e1-169">int</span><span class="sxs-lookup"><span data-stu-id="c42e1-169">int</span></span> | <span data-ttu-id="c42e1-170">Это значение является числовом значении, определенном в RFC 7519 (число JSON, представляющее количество секунд от 1970-01-01T00:00:00Z UTC до указанной даты и времени UTC, игнорируя високосные секунды.)</span><span class="sxs-lookup"><span data-stu-id="c42e1-170">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |
| <span data-ttu-id="c42e1-171">exp</span><span class="sxs-lookup"><span data-stu-id="c42e1-171">exp</span></span> | <span data-ttu-id="c42e1-172">int</span><span class="sxs-lookup"><span data-stu-id="c42e1-172">int</span></span> | <span data-ttu-id="c42e1-173">Это значение является числовом значении, определенном в RFC 7519 (число JSON, представляющее количество секунд от 1970-01-01T00:00:00Z UTC до указанной даты и времени UTC, игнорируя високосные секунды.)</span><span class="sxs-lookup"><span data-stu-id="c42e1-173">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |



## <a name="json-representation"></a><span data-ttu-id="c42e1-174">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c42e1-174">JSON representation</span></span>

<span data-ttu-id="c42e1-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c42e1-175">The following is a JSON representation of the resource.</span></span>

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


