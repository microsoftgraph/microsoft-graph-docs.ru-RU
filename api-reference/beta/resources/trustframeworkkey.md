---
title: Тип ресурса Трустфрамеворккэй
description: Представляет объект ЖВК (веб-ключ JSON). Трустфрамеворккэй — это структура данных JSON, представляющая ключ шифрования. Структура этого ресурса соответствует формату, определенному в разделе 4 RFC 7517.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a9b94075b7a81fdb596038afac21fbf6cbc68f42
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519654"
---
# <a name="trustframeworkkey-resource-type"></a><span data-ttu-id="ec50b-105">Тип ресурса Трустфрамеворккэй</span><span class="sxs-lookup"><span data-stu-id="ec50b-105">trustFrameworkKey resource type</span></span>

<span data-ttu-id="ec50b-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec50b-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec50b-107">Представляет объект ЖВК (веб-ключ JSON).</span><span class="sxs-lookup"><span data-stu-id="ec50b-107">Represents a JWK (JSON Web Key).</span></span> <span data-ttu-id="ec50b-108">Трустфрамеворккэй — это структура данных JSON, представляющая ключ шифрования.</span><span class="sxs-lookup"><span data-stu-id="ec50b-108">TrustFrameworkKey is a JSON data structure that represents a cryptographic key.</span></span> <span data-ttu-id="ec50b-109">Структура этого ресурса соответствует формату, определенному в [разделе 4 RFC 7517](https://tools.ietf.org/html/rfc7517#section-4).</span><span class="sxs-lookup"><span data-stu-id="ec50b-109">The structure of this resource follows the format defined in [RFC 7517 Section 4](https://tools.ietf.org/html/rfc7517#section-4).</span></span>

## <a name="properties"></a><span data-ttu-id="ec50b-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec50b-110">Properties</span></span>

| <span data-ttu-id="ec50b-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec50b-111">Property</span></span>     | <span data-ttu-id="ec50b-112">Тип</span><span class="sxs-lookup"><span data-stu-id="ec50b-112">Type</span></span>        | <span data-ttu-id="ec50b-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ec50b-113">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ec50b-114">детей</span><span class="sxs-lookup"><span data-stu-id="ec50b-114">kid</span></span> | <span data-ttu-id="ec50b-115">string</span><span class="sxs-lookup"><span data-stu-id="ec50b-115">string</span></span> | <span data-ttu-id="ec50b-116">Уникальный идентификатор ключа.</span><span class="sxs-lookup"><span data-stu-id="ec50b-116">The unique identifier for the key.</span></span>   |
| <span data-ttu-id="ec50b-117">кти</span><span class="sxs-lookup"><span data-stu-id="ec50b-117">kty</span></span> | <span data-ttu-id="ec50b-118">string</span><span class="sxs-lookup"><span data-stu-id="ec50b-118">string</span></span> | <span data-ttu-id="ec50b-119">Параметр "КТИ" (тип ключа) определяет семейство алгоритмов шифрования, используемое с ключом, допустимые значения: RSA, Oct.</span><span class="sxs-lookup"><span data-stu-id="ec50b-119">The "kty" (key type) parameter identifies the cryptographic algorithm family used with the key, The valid values are rsa, oct.</span></span> |
| <span data-ttu-id="ec50b-120">Используйте</span><span class="sxs-lookup"><span data-stu-id="ec50b-120">use</span></span> | <span data-ttu-id="ec50b-121">string</span><span class="sxs-lookup"><span data-stu-id="ec50b-121">string</span></span> | <span data-ttu-id="ec50b-122">Параметр "use" (использование открытого ключа) определяет предполагаемое использование открытого ключа.</span><span class="sxs-lookup"><span data-stu-id="ec50b-122">The "use" (public key use) parameter identifies the intended use of the public key.</span></span>  <span data-ttu-id="ec50b-123">Параметр Use используется, чтобы указать, используется ли открытый ключ для шифрования данных или проверки подписи данных.</span><span class="sxs-lookup"><span data-stu-id="ec50b-123">The "use" parameter is employed to indicate whether a public key is used for encrypting data or verifying the signature on data.</span></span> <span data-ttu-id="ec50b-124">Возможные значения: 1.</span><span class="sxs-lookup"><span data-stu-id="ec50b-124">Possible values are    1.</span></span> <span data-ttu-id="ec50b-125">"SIG" (Подпись) 2.</span><span class="sxs-lookup"><span data-stu-id="ec50b-125">"sig" (signature)    2.</span></span>  <span data-ttu-id="ec50b-126">"ENC" (шифрование)</span><span class="sxs-lookup"><span data-stu-id="ec50b-126">"enc" (encryption)</span></span>   |
| <span data-ttu-id="ec50b-127">x5c</span><span class="sxs-lookup"><span data-stu-id="ec50b-127">x5c</span></span> | <span data-ttu-id="ec50b-128">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ec50b-128">string collection</span></span> | <span data-ttu-id="ec50b-129">Параметр "x5c" (цепочка сертификатов X. 509) содержит цепочку из одного или нескольких сертификатов ПКИКС [RFC 5280](https://tools.ietf.org/html/rfc5280).</span><span class="sxs-lookup"><span data-stu-id="ec50b-129">The "x5c" (X.509 certificate chain) parameter contains a chain of one or more PKIX certificates [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="ec50b-130">x5t</span><span class="sxs-lookup"><span data-stu-id="ec50b-130">x5t</span></span> | <span data-ttu-id="ec50b-131">string</span><span class="sxs-lookup"><span data-stu-id="ec50b-131">string</span></span> | <span data-ttu-id="ec50b-132">Параметр "x5t" (отпечаток сертификата X. 509) — это отпечаток SHA-1, закодированный с помощью base64decode.</span><span class="sxs-lookup"><span data-stu-id="ec50b-132">The "x5t" (X.509 certificate SHA-1 thumbprint) parameter is a base64url-encoded SHA-1 thumbprint (a.k.a.</span></span> <span data-ttu-id="ec50b-133">Дайджест) кодировки DER для сертификата X. 509, [RFC 5280](https://tools.ietf.org/html/rfc5280).</span><span class="sxs-lookup"><span data-stu-id="ec50b-133">digest) of the DER encoding of an X.509 certificate [RFC 5280](https://tools.ietf.org/html/rfc5280).</span></span> |
| <span data-ttu-id="ec50b-134">e</span><span class="sxs-lookup"><span data-stu-id="ec50b-134">e</span></span> | <span data-ttu-id="ec50b-135">string</span><span class="sxs-lookup"><span data-stu-id="ec50b-135">string</span></span> | <span data-ttu-id="ec50b-136">Ключ RSA — открытый показатель степени</span><span class="sxs-lookup"><span data-stu-id="ec50b-136">RSA Key - public exponent</span></span> |
| <span data-ttu-id="ec50b-137">d</span><span class="sxs-lookup"><span data-stu-id="ec50b-137">d</span></span>| <span data-ttu-id="ec50b-138">string</span><span class="sxs-lookup"><span data-stu-id="ec50b-138">string</span></span> | <span data-ttu-id="ec50b-139">Закрытый показатель ключа RSA.</span><span class="sxs-lookup"><span data-stu-id="ec50b-139">RSA Key - private exponent.</span></span> <span data-ttu-id="ec50b-140">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="ec50b-140">Field cannot be read back.</span></span> |
| <span data-ttu-id="ec50b-141">n</span><span class="sxs-lookup"><span data-stu-id="ec50b-141">n</span></span> | <span data-ttu-id="ec50b-142">string</span><span class="sxs-lookup"><span data-stu-id="ec50b-142">string</span></span> | <span data-ttu-id="ec50b-143">Ключ RSA — модуль</span><span class="sxs-lookup"><span data-stu-id="ec50b-143">RSA Key - modulus</span></span> |
| <span data-ttu-id="ec50b-144">p</span><span class="sxs-lookup"><span data-stu-id="ec50b-144">p</span></span> | <span data-ttu-id="ec50b-145">string</span><span class="sxs-lookup"><span data-stu-id="ec50b-145">string</span></span> | <span data-ttu-id="ec50b-146">Первый простой ключ RSA.</span><span class="sxs-lookup"><span data-stu-id="ec50b-146">RSA Key - first prime.</span></span> <span data-ttu-id="ec50b-147">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="ec50b-147">Field cannot be read back.</span></span> |
| <span data-ttu-id="ec50b-148">q</span><span class="sxs-lookup"><span data-stu-id="ec50b-148">q</span></span> | <span data-ttu-id="ec50b-149">string</span><span class="sxs-lookup"><span data-stu-id="ec50b-149">string</span></span> | <span data-ttu-id="ec50b-150">Клавиша RSA, простое в секунду.</span><span class="sxs-lookup"><span data-stu-id="ec50b-150">RSA Key - second prime.</span></span> <span data-ttu-id="ec50b-151">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="ec50b-151">Field cannot be read back.</span></span> |
| <span data-ttu-id="ec50b-152">двухпроцессорный</span><span class="sxs-lookup"><span data-stu-id="ec50b-152">dp</span></span> | <span data-ttu-id="ec50b-153">string</span><span class="sxs-lookup"><span data-stu-id="ec50b-153">string</span></span> | <span data-ttu-id="ec50b-154">Экспонента RSA Key — первый показатель.</span><span class="sxs-lookup"><span data-stu-id="ec50b-154">RSA Key - first exponent.</span></span> <span data-ttu-id="ec50b-155">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="ec50b-155">Field cannot be read back.</span></span> |
| <span data-ttu-id="ec50b-156">DQ</span><span class="sxs-lookup"><span data-stu-id="ec50b-156">dq</span></span> | <span data-ttu-id="ec50b-157">string</span><span class="sxs-lookup"><span data-stu-id="ec50b-157">string</span></span> | <span data-ttu-id="ec50b-158">Экспонента RSA Key — секунды.</span><span class="sxs-lookup"><span data-stu-id="ec50b-158">RSA Key - second exponent.</span></span> <span data-ttu-id="ec50b-159">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="ec50b-159">Field cannot be read back.</span></span> |
| <span data-ttu-id="ec50b-160">типом</span><span class="sxs-lookup"><span data-stu-id="ec50b-160">qi</span></span> | <span data-ttu-id="ec50b-161">string</span><span class="sxs-lookup"><span data-stu-id="ec50b-161">string</span></span> | <span data-ttu-id="ec50b-162">Ключ RSA Key — коэффициент.</span><span class="sxs-lookup"><span data-stu-id="ec50b-162">RSA Key - Coefficient.</span></span> <span data-ttu-id="ec50b-163">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="ec50b-163">Field cannot be read back.</span></span> |
| <span data-ttu-id="ec50b-164">звонить</span><span class="sxs-lookup"><span data-stu-id="ec50b-164">k</span></span> | <span data-ttu-id="ec50b-165">string</span><span class="sxs-lookup"><span data-stu-id="ec50b-165">string</span></span> | <span data-ttu-id="ec50b-166">Симметричный ключ для типа ключа центра развертывания Office.</span><span class="sxs-lookup"><span data-stu-id="ec50b-166">Symmetric Key for oct key type.</span></span> <span data-ttu-id="ec50b-167">Невозможно считать поле обратно.</span><span class="sxs-lookup"><span data-stu-id="ec50b-167">Field cannot be read back.</span></span>   |
| <span data-ttu-id="ec50b-168">nbf</span><span class="sxs-lookup"><span data-stu-id="ec50b-168">nbf</span></span> | <span data-ttu-id="ec50b-169">int</span><span class="sxs-lookup"><span data-stu-id="ec50b-169">int</span></span> | <span data-ttu-id="ec50b-170">Это значение является Нумерикдате, как определено в RFC 7519 (числовое значение JSON, представляющее число секунд от 1970 до 01-01T00:00:00Z UTC до указанной даты и времени в формате UTC, игнорируя високосные секунды.)</span><span class="sxs-lookup"><span data-stu-id="ec50b-170">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |
| <span data-ttu-id="ec50b-171">exp</span><span class="sxs-lookup"><span data-stu-id="ec50b-171">exp</span></span> | <span data-ttu-id="ec50b-172">int</span><span class="sxs-lookup"><span data-stu-id="ec50b-172">int</span></span> | <span data-ttu-id="ec50b-173">Это значение является Нумерикдате, как определено в RFC 7519 (числовое значение JSON, представляющее число секунд от 1970 до 01-01T00:00:00Z UTC до указанной даты и времени в формате UTC, игнорируя високосные секунды.)</span><span class="sxs-lookup"><span data-stu-id="ec50b-173">This value is a NumericDate as defined in RFC 7519 (A JSON numeric value representing the number of seconds from 1970-01-01T00:00:00Z UTC until the specified UTC date/time, ignoring leap seconds.)</span></span> |



## <a name="json-representation"></a><span data-ttu-id="ec50b-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ec50b-174">JSON representation</span></span>

<span data-ttu-id="ec50b-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec50b-175">The following is a JSON representation of the resource.</span></span>

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
