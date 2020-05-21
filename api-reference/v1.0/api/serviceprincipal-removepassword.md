---
title: 'servicePrincipal: Ремовепассворд'
description: Удаление пароля из servicePrincipal
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a9538448ab43d1d05ab9a904958dafe42eb65e02
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336620"
---
# <a name="serviceprincipal-removepassword"></a><span data-ttu-id="8799a-103">servicePrincipal: Ремовепассворд</span><span class="sxs-lookup"><span data-stu-id="8799a-103">servicePrincipal: removePassword</span></span>

<span data-ttu-id="8799a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8799a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8799a-105">Удаление пароля из объекта [servicePrincipal](../resources/serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="8799a-105">Remove a password from a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8799a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8799a-106">Permissions</span></span>

<span data-ttu-id="8799a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8799a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8799a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8799a-109">Permission type</span></span>                        | <span data-ttu-id="8799a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8799a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8799a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8799a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8799a-112">Application. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="8799a-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="8799a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8799a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8799a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8799a-114">Not supported.</span></span> |
| <span data-ttu-id="8799a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8799a-115">Application</span></span>                            | <span data-ttu-id="8799a-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8799a-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8799a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8799a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="8799a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8799a-118">Request headers</span></span>

| <span data-ttu-id="8799a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8799a-119">Name</span></span>           | <span data-ttu-id="8799a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8799a-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="8799a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8799a-121">Authorization</span></span>  | <span data-ttu-id="8799a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8799a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8799a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8799a-124">Content-type</span></span>   | <span data-ttu-id="8799a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8799a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8799a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8799a-127">Request body</span></span>

| <span data-ttu-id="8799a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="8799a-128">Property</span></span>     | <span data-ttu-id="8799a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="8799a-129">Type</span></span>   |<span data-ttu-id="8799a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="8799a-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8799a-131">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="8799a-131">keyId</span></span> | <span data-ttu-id="8799a-132">Идентификатор GUID</span><span class="sxs-lookup"><span data-stu-id="8799a-132">GUID</span></span> | <span data-ttu-id="8799a-133">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="8799a-133">The unique identifier for the password.</span></span> <span data-ttu-id="8799a-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8799a-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8799a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8799a-135">Response</span></span>

<span data-ttu-id="8799a-136">В случае успешного выполнения этот метод возвращает код отклика `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="8799a-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8799a-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="8799a-137">Examples</span></span>

<span data-ttu-id="8799a-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="8799a-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8799a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="8799a-139">Request</span></span>

<span data-ttu-id="8799a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8799a-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8799a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="8799a-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8799a-142">C#</span><span class="sxs-lookup"><span data-stu-id="8799a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8799a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8799a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8799a-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8799a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8799a-145">Java</span><span class="sxs-lookup"><span data-stu-id="8799a-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-removepassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8799a-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8799a-146">Response</span></span>

<span data-ttu-id="8799a-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8799a-147">The following is an example of the response.</span></span>

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
