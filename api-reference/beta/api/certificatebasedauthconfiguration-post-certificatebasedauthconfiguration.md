---
title: Создание Цертификатебаседаусконфигуратион
description: Используйте этот API для создания нового Цертификатебаседаусконфигуратион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 454179de952f4b757ba5b11181b110a7d3df9917
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720102"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="19e70-103">Создание Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="19e70-103">Create certificateBasedAuthConfiguration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19e70-104">Создание нового объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="19e70-104">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="19e70-105">Можно создать только один экземпляр **цертификатебаседаусконфигуратион** (коллекция может содержать только один элемент).</span><span class="sxs-lookup"><span data-stu-id="19e70-105">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="19e70-106">Он всегда имеет фиксированный идентификатор со значением "29728ade-6ae4-4ee9-9103-412912537da5".</span><span class="sxs-lookup"><span data-stu-id="19e70-106">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="19e70-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19e70-107">Permissions</span></span>

<span data-ttu-id="19e70-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19e70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19e70-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19e70-110">Permission type</span></span>                        | <span data-ttu-id="19e70-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19e70-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="19e70-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19e70-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="19e70-113">Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="19e70-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="19e70-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19e70-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19e70-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19e70-115">Not supported.</span></span> |
| <span data-ttu-id="19e70-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19e70-116">Application</span></span>    | <span data-ttu-id="19e70-117">Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="19e70-117">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19e70-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19e70-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="19e70-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19e70-119">Request headers</span></span>

| <span data-ttu-id="19e70-120">Имя</span><span class="sxs-lookup"><span data-stu-id="19e70-120">Name</span></span>          | <span data-ttu-id="19e70-121">Описание</span><span class="sxs-lookup"><span data-stu-id="19e70-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="19e70-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19e70-122">Authorization</span></span> | <span data-ttu-id="19e70-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="19e70-123">Bearer {token}</span></span> |
| <span data-ttu-id="19e70-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19e70-124">Content-Type</span></span> | <span data-ttu-id="19e70-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19e70-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="19e70-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19e70-126">Request body</span></span>

<span data-ttu-id="19e70-127">Для создания объекта [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) требуются следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="19e70-127">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="19e70-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="19e70-128">Property</span></span>     | <span data-ttu-id="19e70-129">Тип</span><span class="sxs-lookup"><span data-stu-id="19e70-129">Type</span></span>        | <span data-ttu-id="19e70-130">Описание</span><span class="sxs-lookup"><span data-stu-id="19e70-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="19e70-131">цертификатеаусоритиес</span><span class="sxs-lookup"><span data-stu-id="19e70-131">certificateAuthorities</span></span>| <span data-ttu-id="19e70-132">Коллекция [цертификатеаусорити](../resources/certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="19e70-132">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="19e70-133">Коллекция центров сертификации, которая создает доверенную цепочку сертификатов.</span><span class="sxs-lookup"><span data-stu-id="19e70-133">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="19e70-134">Каждый член коллекции должен содержать свойства **Certificate** и **исрутаусорити** .</span><span class="sxs-lookup"><span data-stu-id="19e70-134">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="19e70-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="19e70-135">Response</span></span>

<span data-ttu-id="19e70-136">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и новый объект [цертификатебаседаусконфигуратион](../resources/certificatebasedauthconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="19e70-136">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19e70-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="19e70-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="19e70-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="19e70-138">Request</span></span>

<span data-ttu-id="19e70-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19e70-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="19e70-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="19e70-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="19e70-141">C#</span><span class="sxs-lookup"><span data-stu-id="19e70-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19e70-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19e70-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19e70-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="19e70-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="19e70-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="19e70-144">Response</span></span>

<span data-ttu-id="19e70-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="19e70-145">The following is an example of the response.</span></span>

> <span data-ttu-id="19e70-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19e70-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
