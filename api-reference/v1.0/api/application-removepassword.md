---
title: 'Приложение: Ремовепассворд'
description: Удаление пароля из приложения
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bd3f5ed410fb7ba2294fb57f4cd7bdb065f99981
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289667"
---
# <a name="application-removepassword"></a><span data-ttu-id="f94fb-103">Приложение: Ремовепассворд</span><span class="sxs-lookup"><span data-stu-id="f94fb-103">application: removePassword</span></span>

<span data-ttu-id="f94fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f94fb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f94fb-105">Удаление пароля из [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="f94fb-105">Remove a password from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f94fb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f94fb-106">Permissions</span></span>

<span data-ttu-id="f94fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f94fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f94fb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f94fb-109">Permission type</span></span>                        | <span data-ttu-id="f94fb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f94fb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f94fb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f94fb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f94fb-112">Application. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="f94fb-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="f94fb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f94fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f94fb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f94fb-114">Not supported.</span></span> |
| <span data-ttu-id="f94fb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f94fb-115">Application</span></span>                            | <span data-ttu-id="f94fb-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f94fb-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f94fb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f94fb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="f94fb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f94fb-118">Request headers</span></span>

| <span data-ttu-id="f94fb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f94fb-119">Name</span></span>           | <span data-ttu-id="f94fb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f94fb-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f94fb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f94fb-121">Authorization</span></span>  | <span data-ttu-id="f94fb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f94fb-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f94fb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f94fb-124">Content-Type</span></span>   | <span data-ttu-id="f94fb-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f94fb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f94fb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f94fb-127">Request body</span></span>

| <span data-ttu-id="f94fb-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f94fb-128">Property</span></span>  | <span data-ttu-id="f94fb-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f94fb-129">Type</span></span> | <span data-ttu-id="f94fb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f94fb-130">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="f94fb-131">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="f94fb-131">keyId</span></span>     | <span data-ttu-id="f94fb-132">Идентификатор GUID</span><span class="sxs-lookup"><span data-stu-id="f94fb-132">GUID</span></span> | <span data-ttu-id="f94fb-133">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="f94fb-133">The unique identifier for the password.</span></span> <span data-ttu-id="f94fb-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f94fb-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f94fb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f94fb-135">Response</span></span>

<span data-ttu-id="f94fb-136">В случае успешного выполнения этот метод возвращает код отклика `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="f94fb-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f94fb-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="f94fb-137">Examples</span></span>

<span data-ttu-id="f94fb-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="f94fb-138">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="f94fb-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f94fb-139">Request</span></span>

<span data-ttu-id="f94fb-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f94fb-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f94fb-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="f94fb-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_removepassword"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```
# <a name="c"></a>[<span data-ttu-id="f94fb-142">C#</span><span class="sxs-lookup"><span data-stu-id="f94fb-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f94fb-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f94fb-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f94fb-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f94fb-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f94fb-145">Java</span><span class="sxs-lookup"><span data-stu-id="f94fb-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-removepassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f94fb-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="f94fb-146">Response</span></span>

<span data-ttu-id="f94fb-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f94fb-147">The following is an example of the response.</span></span>

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
  "description": "application: removePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
