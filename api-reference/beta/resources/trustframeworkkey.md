---
title: тип ресурса trustFrameworkKey
description: Представляет JWK (веб-ключ JSON). TrustFrameworkKey — это структура данных JSON, представляюная криптографический ключ. Структура этого ресурса следует формату, определенному в разделе RFC 7517 4.
localization_priority: Normal
author: valnav
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b50e82748db6c0c26252ce6b79290781fa88819b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945636"
---
# <a name="trustframeworkkey-resource-type"></a><span data-ttu-id="cff3d-105">тип ресурса trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="cff3d-105">trustFrameworkKey resource type</span></span>

<span data-ttu-id="cff3d-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cff3d-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cff3d-107">Представляет JWK (веб-ключ JSON).</span><span class="sxs-lookup"><span data-stu-id="cff3d-107">Represents a JWK (JSON Web Key).</span></span> <span data-ttu-id="cff3d-108">TrustFrameworkKey — это структура данных JSON, представляюная криптографический ключ.</span><span class="sxs-lookup"><span data-stu-id="cff3d-108">TrustFrameworkKey is a JSON data structure that represents a cryptographic key.</span></span> <span data-ttu-id="cff3d-109">Структура этого ресурса следует формату, определенному в [разделе RFC 7517 4](https://tools.ietf.org/html/rfc7517#section-4).</span><span class="sxs-lookup"><span data-stu-id="cff3d-109">The structure of this resource follows the format defined in [RFC 7517 Section 4](https://tools.ietf.org/html/rfc7517#section-4).</span></span>

## <a name="properties"></a><span data-ttu-id="cff3d-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="cff3d-110">Properties</span></span>

| <span data-ttu-id="cff3d-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="cff3d-111">Property</span></span>     | <span data-ttu-id="cff3d-112">Тип</span><span class="sxs-lookup"><span data-stu-id="cff3d-112">Type</span></span>        | <span data-ttu-id="cff3d-113">Описание</span><span class="sxs-lookup"><span data-stu-id="cff3d-113">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cff3d-114">малыш</span><span class="sxs-lookup"><span data-stu-id="cff3d-114">kid</span></span> | <span data-ttu-id="cff3d-115">string</span><span class="sxs-lookup"><span data-stu-id="cff3d-115">string</span></span> | <span data-ttu-id="cff3d-116">Уникальный идентификатор для ключа.</span><span class="sxs-lookup"><span data-stu-id="cff3d-116">The unique identifier for the key.</span></span>   |
| <span data-ttu-id="cff3d-117">kty</span><span class="sxs-lookup"><span data-stu-id="cff3d-117">kty</span></span> | <span data-ttu-id="cff3d-118">Строка</span><span class="sxs-lookup"><span data-stu-id="cff3d-118">String</span></span> | <span data-ttu-id="cff3d-119">Параметр **kty** (тип ключа) определяет семейство криптографических алгоритмов, используемых с ключом, Допустимые значения `rsa` , `oct` .</span><span class="sxs-lookup"><span data-stu-id="cff3d-119">The **kty** (key type) parameter identifies the cryptographic algorithm family used with the key, The valid values are `rsa`, `oct`.</span></span> |
| <span data-ttu-id="cff3d-120">использование</span><span class="sxs-lookup"><span data-stu-id="cff3d-120">use</span></span> | <span data-ttu-id="cff3d-121">Строка</span><span class="sxs-lookup"><span data-stu-id="cff3d-121">String</span></span> | <span data-ttu-id="cff3d-122">Параметр **use** (public key use) определяет предназначенное использование общедоступных ключей.</span><span class="sxs-lookup"><span data-stu-id="cff3d-122">The **use** (public key use) parameter identifies the intended use of the public key.</span></span>  <span data-ttu-id="cff3d-123">Параметр **use** используется для того, чтобы указать, используется ли общедоступный ключ для шифрования данных или проверки подписи на данных.</span><span class="sxs-lookup"><span data-stu-id="cff3d-123">The **use** parameter is employed to indicate whether a public key is used for encrypting data or verifying the signature on data.</span></span> <span data-ttu-id="cff3d-124">Возможные значения: `sig` (подпись), `enc` (шифрование)</span><span class="sxs-lookup"><span data-stu-id="cff3d-124">Possible values are: `sig` (signature), `enc` (encryption)</span></span>  |
| <span data-ttu-id="cff3d-125">x5c</span><span class="sxs-lookup"><span data-stu-id="cff3d-125">x5c</span></span> | <span data-ttu-id="cff3d-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cff3d-126">string collection</span></span> | <span data-ttu-id="cff3d-127">Параметр **x5c** (цепочка сертификатов X.509) содержит цепочку из одного или более сертификатов [PKIX RFC 5280.](https://tools.ietf.org/html/rfc5280)</span><span class="sxs-lookup"><span data-stu-id="cff3d-127">The **x5c** (X.509 certificate chain) parameter contains a chain of one or more PKIX certificates [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="cff3d-128">x5t</span><span class="sxs-lookup"><span data-stu-id="cff3d-128">x5t</span></span> | <span data-ttu-id="cff3d-129">string</span><span class="sxs-lookup"><span data-stu-id="cff3d-129">string</span></span> | <span data-ttu-id="cff3d-130">Параметр **x5t** (X.509 сертификата SHA-1) является отпечатком пальца sha-1 с кодированной базой 64url (sha-1).</span><span class="sxs-lookup"><span data-stu-id="cff3d-130">The **x5t** (X.509 certificate SHA-1 thumbprint) parameter is a base64url-encoded SHA-1 thumbprint (a.k.a.</span></span> <span data-ttu-id="cff3d-131">дайджест) кодилизовки DER сертификата X.509 [RFC 5280.](https://tools.ietf.org/html/rfc5280)</span><span class="sxs-lookup"><span data-stu-id="cff3d-131">digest) of the DER encoding of an X.509 certificate [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="cff3d-132">e</span><span class="sxs-lookup"><span data-stu-id="cff3d-132">e</span></span> | <span data-ttu-id="cff3d-133">string</span><span class="sxs-lookup"><span data-stu-id="cff3d-133">string</span></span> | <span data-ttu-id="cff3d-134">Клавиша RSA — публичный показатель</span><span class="sxs-lookup"><span data-stu-id="cff3d-134">RSA Key - public exponent</span></span> |
| <span data-ttu-id="cff3d-135">d</span><span class="sxs-lookup"><span data-stu-id="cff3d-135">d</span></span>| <span data-ttu-id="cff3d-136">string</span><span class="sxs-lookup"><span data-stu-id="cff3d-136">string</span></span> | <span data-ttu-id="cff3d-137">Ключ RSA — частный экспонент.</span><span class="sxs-lookup"><span data-stu-id="cff3d-137">RSA Key - private exponent.</span></span> <span data-ttu-id="cff3d-138">Поле не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="cff3d-138">Field cannot be read back.</span></span> |
| <span data-ttu-id="cff3d-139">n</span><span class="sxs-lookup"><span data-stu-id="cff3d-139">n</span></span> | <span data-ttu-id="cff3d-140">string</span><span class="sxs-lookup"><span data-stu-id="cff3d-140">string</span></span> | <span data-ttu-id="cff3d-141">Клавиша RSA — modulus</span><span class="sxs-lookup"><span data-stu-id="cff3d-141">RSA Key - modulus</span></span> |
| <span data-ttu-id="cff3d-142">p</span><span class="sxs-lookup"><span data-stu-id="cff3d-142">p</span></span> | <span data-ttu-id="cff3d-143">string</span><span class="sxs-lookup"><span data-stu-id="cff3d-143">string</span></span> | <span data-ttu-id="cff3d-144">Клавиша RSA — первый прайм.</span><span class="sxs-lookup"><span data-stu-id="cff3d-144">RSA Key - first prime.</span></span> <span data-ttu-id="cff3d-145">Поле не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="cff3d-145">Field cannot be read back.</span></span> |
| <span data-ttu-id="cff3d-146">q</span><span class="sxs-lookup"><span data-stu-id="cff3d-146">q</span></span> | <span data-ttu-id="cff3d-147">string</span><span class="sxs-lookup"><span data-stu-id="cff3d-147">string</span></span> | <span data-ttu-id="cff3d-148">Клавиша RSA — второй прайм.</span><span class="sxs-lookup"><span data-stu-id="cff3d-148">RSA Key - second prime.</span></span> <span data-ttu-id="cff3d-149">Поле не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="cff3d-149">Field cannot be read back.</span></span> |
| <span data-ttu-id="cff3d-150">dp</span><span class="sxs-lookup"><span data-stu-id="cff3d-150">dp</span></span> | <span data-ttu-id="cff3d-151">string</span><span class="sxs-lookup"><span data-stu-id="cff3d-151">string</span></span> | <span data-ttu-id="cff3d-152">Клавиша RSA — первый экспонент.</span><span class="sxs-lookup"><span data-stu-id="cff3d-152">RSA Key - first exponent.</span></span> <span data-ttu-id="cff3d-153">Поле не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="cff3d-153">Field cannot be read back.</span></span> |
| <span data-ttu-id="cff3d-154">dq</span><span class="sxs-lookup"><span data-stu-id="cff3d-154">dq</span></span> | <span data-ttu-id="cff3d-155">string</span><span class="sxs-lookup"><span data-stu-id="cff3d-155">string</span></span> | <span data-ttu-id="cff3d-156">Клавиша RSA — второй показатель.</span><span class="sxs-lookup"><span data-stu-id="cff3d-156">RSA Key - second exponent.</span></span> <span data-ttu-id="cff3d-157">Поле не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="cff3d-157">Field cannot be read back.</span></span> |
| <span data-ttu-id="cff3d-158">qi</span><span class="sxs-lookup"><span data-stu-id="cff3d-158">qi</span></span> | <span data-ttu-id="cff3d-159">string</span><span class="sxs-lookup"><span data-stu-id="cff3d-159">string</span></span> | <span data-ttu-id="cff3d-160">Ключ RSA — коэффициент.</span><span class="sxs-lookup"><span data-stu-id="cff3d-160">RSA Key - Coefficient.</span></span> <span data-ttu-id="cff3d-161">Поле не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="cff3d-161">Field cannot be read back.</span></span> |
| <span data-ttu-id="cff3d-162">k</span><span class="sxs-lookup"><span data-stu-id="cff3d-162">k</span></span> | <span data-ttu-id="cff3d-163">string</span><span class="sxs-lookup"><span data-stu-id="cff3d-163">string</span></span> | <span data-ttu-id="cff3d-164">Симметричный ключ для типа ключа oct.</span><span class="sxs-lookup"><span data-stu-id="cff3d-164">Symmetric Key for oct key type.</span></span> <span data-ttu-id="cff3d-165">Поле не может быть прочитано обратно.</span><span class="sxs-lookup"><span data-stu-id="cff3d-165">Field cannot be read back.</span></span>   |
| <span data-ttu-id="cff3d-166">nbf</span><span class="sxs-lookup"><span data-stu-id="cff3d-166">nbf</span></span> | <span data-ttu-id="cff3d-167">int</span><span class="sxs-lookup"><span data-stu-id="cff3d-167">int</span></span> | <span data-ttu-id="cff3d-168">Это значение — numericDate, как определено в RFC 7519 (численное значение JSON, представляющее число секунд с 1970-01-01T00:00:00:00Z UTC до указанной даты UTC/времени, игнорируя високосные секунды.)</span><span class="sxs-lookup"><span data-stu-id="cff3d-168">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |
| <span data-ttu-id="cff3d-169">exp</span><span class="sxs-lookup"><span data-stu-id="cff3d-169">exp</span></span> | <span data-ttu-id="cff3d-170">int</span><span class="sxs-lookup"><span data-stu-id="cff3d-170">int</span></span> | <span data-ttu-id="cff3d-171">Это значение — numericDate, как определено в RFC 7519 (численное значение JSON, представляющее число секунд с 1970-01-01T00:00:00:00Z UTC до указанной даты UTC/времени, игнорируя високосные секунды.)</span><span class="sxs-lookup"><span data-stu-id="cff3d-171">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |



## <a name="json-representation"></a><span data-ttu-id="cff3d-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cff3d-172">JSON representation</span></span>

<span data-ttu-id="cff3d-173">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cff3d-173">The following is a JSON representation of the resource.</span></span>

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


