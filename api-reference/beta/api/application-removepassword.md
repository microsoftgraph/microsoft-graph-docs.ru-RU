---
title: 'application: removePassword'
description: Удаление пароля из приложения
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8c8865470e67418e877d130ea9143631a5398e92
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129046"
---
# <a name="application-removepassword"></a><span data-ttu-id="e5bc8-103">application: removePassword</span><span class="sxs-lookup"><span data-stu-id="e5bc8-103">application: removePassword</span></span>

<span data-ttu-id="e5bc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5bc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5bc8-105">Удаляет пароль из [приложения.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="e5bc8-105">Removes a password from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e5bc8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5bc8-106">Permissions</span></span>

<span data-ttu-id="e5bc8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5bc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5bc8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5bc8-109">Permission type</span></span>                        | <span data-ttu-id="e5bc8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5bc8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e5bc8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5bc8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5bc8-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5bc8-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="e5bc8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5bc8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5bc8-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5bc8-114">Application.ReadWrite.All</span></span> |
| <span data-ttu-id="e5bc8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e5bc8-115">Application</span></span>                            | <span data-ttu-id="e5bc8-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5bc8-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5bc8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5bc8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="e5bc8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5bc8-118">Request headers</span></span>

| <span data-ttu-id="e5bc8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e5bc8-119">Name</span></span>           | <span data-ttu-id="e5bc8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e5bc8-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="e5bc8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5bc8-121">Authorization</span></span>  | <span data-ttu-id="e5bc8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5bc8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e5bc8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5bc8-124">Content-Type</span></span>   | <span data-ttu-id="e5bc8-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5bc8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5bc8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5bc8-127">Request body</span></span>

| <span data-ttu-id="e5bc8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5bc8-128">Property</span></span>  | <span data-ttu-id="e5bc8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e5bc8-129">Type</span></span> | <span data-ttu-id="e5bc8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e5bc8-130">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="e5bc8-131">keyId</span><span class="sxs-lookup"><span data-stu-id="e5bc8-131">keyId</span></span>     | <span data-ttu-id="e5bc8-132">GUID</span><span class="sxs-lookup"><span data-stu-id="e5bc8-132">GUID</span></span> | <span data-ttu-id="e5bc8-133">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="e5bc8-133">The unique identifier for the password.</span></span> <span data-ttu-id="e5bc8-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5bc8-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e5bc8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5bc8-135">Response</span></span>

<span data-ttu-id="e5bc8-136">В случае успешного выполнения этот метод возвращает код отклика `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="e5bc8-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e5bc8-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="e5bc8-137">Examples</span></span>

<span data-ttu-id="e5bc8-138">Ниже показано, как вызвать этот API.</span><span class="sxs-lookup"><span data-stu-id="e5bc8-138">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="e5bc8-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5bc8-139">Request</span></span>

<span data-ttu-id="e5bc8-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5bc8-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5bc8-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5bc8-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_removepassword"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```
# <a name="c"></a>[<span data-ttu-id="e5bc8-142">C#</span><span class="sxs-lookup"><span data-stu-id="e5bc8-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5bc8-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5bc8-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5bc8-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5bc8-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5bc8-145">Java</span><span class="sxs-lookup"><span data-stu-id="e5bc8-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-removepassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e5bc8-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5bc8-146">Response</span></span>

<span data-ttu-id="e5bc8-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e5bc8-147">The following is an example of the response.</span></span>

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



