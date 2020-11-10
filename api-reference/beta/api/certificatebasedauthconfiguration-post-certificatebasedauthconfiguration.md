---
title: Создание Цертификатебаседаусконфигуратион
description: Используйте этот API для создания нового Цертификатебаседаусконфигуратион.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f424ec111fb7551232bdf102b8debcb9dc248394
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959367"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="b0086-103">Создание Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b0086-103">Create certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="b0086-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0086-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0086-105">Создание нового объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b0086-105">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="b0086-106">Можно создать только один экземпляр **цертификатебаседаусконфигуратион** (коллекция может содержать только один элемент).</span><span class="sxs-lookup"><span data-stu-id="b0086-106">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="b0086-107">Он всегда имеет фиксированный идентификатор со значением "29728ade-6ae4-4ee9-9103-412912537da5".</span><span class="sxs-lookup"><span data-stu-id="b0086-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0086-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0086-108">Permissions</span></span>

<span data-ttu-id="b0086-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0086-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b0086-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0086-111">Permission type</span></span>                        | <span data-ttu-id="b0086-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0086-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b0086-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0086-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0086-114">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0086-114">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="b0086-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0086-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0086-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0086-116">Not supported.</span></span> |
| <span data-ttu-id="b0086-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0086-117">Application</span></span>    | <span data-ttu-id="b0086-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0086-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0086-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0086-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="b0086-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0086-120">Request headers</span></span>

| <span data-ttu-id="b0086-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b0086-121">Name</span></span>          | <span data-ttu-id="b0086-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b0086-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b0086-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0086-123">Authorization</span></span> | <span data-ttu-id="b0086-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="b0086-124">Bearer {token}</span></span> |
| <span data-ttu-id="b0086-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0086-125">Content-Type</span></span> | <span data-ttu-id="b0086-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0086-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0086-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0086-127">Request body</span></span>

<span data-ttu-id="b0086-128">Для создания объекта [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) требуются следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="b0086-128">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="b0086-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0086-129">Property</span></span>     | <span data-ttu-id="b0086-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b0086-130">Type</span></span>        | <span data-ttu-id="b0086-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b0086-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b0086-132">цертификатеаусоритиес</span><span class="sxs-lookup"><span data-stu-id="b0086-132">certificateAuthorities</span></span>| <span data-ttu-id="b0086-133">Коллекция [цертификатеаусорити](../resources/certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="b0086-133">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="b0086-134">Коллекция центров сертификации, которая создает доверенную цепочку сертификатов.</span><span class="sxs-lookup"><span data-stu-id="b0086-134">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="b0086-135">Каждый член коллекции должен содержать свойства **Certificate** и **исрутаусорити** .</span><span class="sxs-lookup"><span data-stu-id="b0086-135">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="b0086-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0086-136">Response</span></span>

<span data-ttu-id="b0086-137">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0086-137">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b0086-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="b0086-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0086-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0086-139">Request</span></span>

<span data-ttu-id="b0086-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0086-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0086-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0086-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_certificatebasedauthconfiguration_from_certificatebasedauthconfiguration"
}-->

```http
POST https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration
Content-type: application/json

{
  "certificateAuthorities": [
    {
      "isRootAuthority": true,
      "certificate": "Binary"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="b0086-142">C#</span><span class="sxs-lookup"><span data-stu-id="b0086-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0086-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0086-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0086-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0086-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0086-145">Java</span><span class="sxs-lookup"><span data-stu-id="b0086-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b0086-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0086-146">Response</span></span>

<span data-ttu-id="b0086-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b0086-147">The following is an example of the response.</span></span>

> <span data-ttu-id="b0086-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0086-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "certificateAuthorities": [
    {
      "isRootAuthority": true,
      "certificate": "Binary",
      "issuer": "issuer-value",
      "issuerSki": "issuerSki-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


