---
title: 'servicePrincipal: removePassword'
description: Удаление пароля из servicePrincipal
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 30f66a540a7a140e6381ff4f4f556b3509a04a3b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130538"
---
# <a name="serviceprincipal-removepassword"></a><span data-ttu-id="ec6e9-103">servicePrincipal: removePassword</span><span class="sxs-lookup"><span data-stu-id="ec6e9-103">servicePrincipal: removePassword</span></span>

<span data-ttu-id="ec6e9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec6e9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ec6e9-105">Удаление пароля из объекта [servicePrincipal.](../resources/serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="ec6e9-105">Remove a password from a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec6e9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec6e9-106">Permissions</span></span>

<span data-ttu-id="ec6e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec6e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec6e9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec6e9-109">Permission type</span></span>                        | <span data-ttu-id="ec6e9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec6e9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ec6e9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec6e9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec6e9-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ec6e9-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="ec6e9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec6e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec6e9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec6e9-114">Not supported.</span></span> |
| <span data-ttu-id="ec6e9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ec6e9-115">Application</span></span>                            | <span data-ttu-id="ec6e9-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec6e9-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec6e9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec6e9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="ec6e9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec6e9-118">Request headers</span></span>

| <span data-ttu-id="ec6e9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ec6e9-119">Name</span></span>           | <span data-ttu-id="ec6e9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ec6e9-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="ec6e9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec6e9-121">Authorization</span></span>  | <span data-ttu-id="ec6e9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec6e9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ec6e9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec6e9-124">Content-type</span></span>   | <span data-ttu-id="ec6e9-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec6e9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec6e9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec6e9-127">Request body</span></span>

| <span data-ttu-id="ec6e9-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec6e9-128">Property</span></span>     | <span data-ttu-id="ec6e9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ec6e9-129">Type</span></span>   |<span data-ttu-id="ec6e9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ec6e9-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ec6e9-131">keyId</span><span class="sxs-lookup"><span data-stu-id="ec6e9-131">keyId</span></span> | <span data-ttu-id="ec6e9-132">GUID</span><span class="sxs-lookup"><span data-stu-id="ec6e9-132">GUID</span></span> | <span data-ttu-id="ec6e9-133">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="ec6e9-133">The unique identifier for the password.</span></span> <span data-ttu-id="ec6e9-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec6e9-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ec6e9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec6e9-135">Response</span></span>

<span data-ttu-id="ec6e9-136">В случае успешного выполнения этот метод возвращает код отклика `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="ec6e9-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ec6e9-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="ec6e9-137">Examples</span></span>

<span data-ttu-id="ec6e9-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="ec6e9-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="ec6e9-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec6e9-139">Request</span></span>

<span data-ttu-id="ec6e9-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec6e9-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ec6e9-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec6e9-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_removepassword"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```
# <a name="c"></a>[<span data-ttu-id="ec6e9-142">C#</span><span class="sxs-lookup"><span data-stu-id="ec6e9-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec6e9-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec6e9-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec6e9-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec6e9-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec6e9-145">Java</span><span class="sxs-lookup"><span data-stu-id="ec6e9-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-removepassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ec6e9-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec6e9-146">Response</span></span>

<span data-ttu-id="ec6e9-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ec6e9-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordCredential"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: removePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

