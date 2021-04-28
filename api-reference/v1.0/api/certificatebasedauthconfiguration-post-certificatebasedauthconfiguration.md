---
title: Создание certificateBasedAuthConfiguration
description: Используйте этот API для создания нового сертификатаBasedAuthConfiguration.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1f1c759cade945fb8dad05d82ae30c9044074e5f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051573"
---
# <a name="create-certificatebasedauthconfiguration"></a><span data-ttu-id="6b347-103">Создание certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="6b347-103">Create certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="6b347-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b347-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b347-105">Создайте новый [объект certificateBasedAuthConfiguration.](../resources/certificateBasedAuthConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b347-105">Create a new [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="6b347-106">Можно создать только один экземпляр **сертификатаBasedAuthConfiguration** (в коллекции может быть только один член).</span><span class="sxs-lookup"><span data-stu-id="6b347-106">Only a single instance of a **certificateBasedAuthConfiguration** can be created (the collection can only have one member).</span></span> <span data-ttu-id="6b347-107">Он всегда имеет фиксированный ID со значением '29728ade-6ae4-4ee9-9103-412912537da5'.</span><span class="sxs-lookup"><span data-stu-id="6b347-107">It always has a fixed ID with a value of '29728ade-6ae4-4ee9-9103-412912537da5'.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b347-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b347-108">Permissions</span></span>

<span data-ttu-id="6b347-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b347-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b347-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b347-111">Permission type</span></span>                        | <span data-ttu-id="6b347-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b347-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6b347-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b347-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b347-114">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b347-114">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="6b347-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b347-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b347-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b347-116">Not supported.</span></span> |
| <span data-ttu-id="6b347-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b347-117">Application</span></span>    | <span data-ttu-id="6b347-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b347-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b347-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b347-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/certificateBasedAuthConfiguration/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6b347-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b347-120">Request headers</span></span>

| <span data-ttu-id="6b347-121">Имя</span><span class="sxs-lookup"><span data-stu-id="6b347-121">Name</span></span>          | <span data-ttu-id="6b347-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6b347-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6b347-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b347-123">Authorization</span></span> | <span data-ttu-id="6b347-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b347-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6b347-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6b347-126">Content-Type</span></span> | <span data-ttu-id="6b347-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b347-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b347-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b347-129">Request body</span></span>

<span data-ttu-id="6b347-130">Для создания объекта [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) необходимы следующие свойства.</span><span class="sxs-lookup"><span data-stu-id="6b347-130">The following properties are required to create the [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object.</span></span>

| <span data-ttu-id="6b347-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b347-131">Property</span></span>     | <span data-ttu-id="6b347-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6b347-132">Type</span></span>        | <span data-ttu-id="6b347-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6b347-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6b347-134">certificateAuthorities</span><span class="sxs-lookup"><span data-stu-id="6b347-134">certificateAuthorities</span></span>| <span data-ttu-id="6b347-135">[коллекция certificateAuthority](../resources/certificateauthority.md)</span><span class="sxs-lookup"><span data-stu-id="6b347-135">[certificateAuthority](../resources/certificateauthority.md) collection</span></span> |<span data-ttu-id="6b347-136">Коллекция органов сертификации, создав цепочку доверенных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="6b347-136">Collection of certificate authorities that creates a trusted certificate chain.</span></span>  <span data-ttu-id="6b347-137">Каждый член коллекции должен содержать **свойства сертификата** **и isRootAuthority.**</span><span class="sxs-lookup"><span data-stu-id="6b347-137">Each member of the collection must contain **certificate** and **isRootAuthority** properties.</span></span> |

## <a name="response"></a><span data-ttu-id="6b347-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b347-138">Response</span></span>

<span data-ttu-id="6b347-139">В случае успешной работы этот метод возвращает код отклика и новый `201 Created` [объект certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6b347-139">If successful, this method returns `201 Created` response code and a new [certificateBasedAuthConfiguration](../resources/certificatebasedauthconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6b347-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="6b347-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6b347-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b347-141">Request</span></span>

<span data-ttu-id="6b347-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b347-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b347-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b347-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_certificatebasedauthconfiguration_from_certificatebasedauthconfiguration"
}-->

```http
POST https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/$ref
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
# <a name="c"></a>[<span data-ttu-id="6b347-144">C#</span><span class="sxs-lookup"><span data-stu-id="6b347-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b347-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b347-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b347-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b347-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b347-147">Java</span><span class="sxs-lookup"><span data-stu-id="6b347-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-certificatebasedauthconfiguration-from-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


---


### <a name="response"></a><span data-ttu-id="6b347-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b347-148">Response</span></span>

<span data-ttu-id="6b347-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6b347-149">The following is an example of the response.</span></span>

> <span data-ttu-id="6b347-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6b347-150">**Note:** The response object shown here might be shortened for readability.</span></span>

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

