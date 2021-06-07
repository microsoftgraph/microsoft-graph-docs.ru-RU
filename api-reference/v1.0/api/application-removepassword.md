---
title: 'приложение: removePassword'
description: Удаление пароля из приложения
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: cfe32e9743bbae164065416adfa1873431a1bb51
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787977"
---
# <a name="application-removepassword"></a><span data-ttu-id="3096d-103">приложение: removePassword</span><span class="sxs-lookup"><span data-stu-id="3096d-103">application: removePassword</span></span>

<span data-ttu-id="3096d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3096d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3096d-105">Удаление пароля из [приложения.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="3096d-105">Remove a password from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3096d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3096d-106">Permissions</span></span>

<span data-ttu-id="3096d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3096d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3096d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3096d-109">Permission type</span></span>                        | <span data-ttu-id="3096d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3096d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3096d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3096d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3096d-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3096d-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="3096d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3096d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3096d-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3096d-114">Application.ReadWrite.All</span></span> |
| <span data-ttu-id="3096d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3096d-115">Application</span></span>                            | <span data-ttu-id="3096d-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3096d-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3096d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3096d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="3096d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3096d-118">Request headers</span></span>

| <span data-ttu-id="3096d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3096d-119">Name</span></span>           | <span data-ttu-id="3096d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3096d-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="3096d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3096d-121">Authorization</span></span>  | <span data-ttu-id="3096d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3096d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3096d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3096d-124">Content-Type</span></span>   | <span data-ttu-id="3096d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3096d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3096d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3096d-127">Request body</span></span>

| <span data-ttu-id="3096d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3096d-128">Property</span></span>  | <span data-ttu-id="3096d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3096d-129">Type</span></span> | <span data-ttu-id="3096d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3096d-130">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="3096d-131">keyId</span><span class="sxs-lookup"><span data-stu-id="3096d-131">keyId</span></span>     | <span data-ttu-id="3096d-132">GUID</span><span class="sxs-lookup"><span data-stu-id="3096d-132">GUID</span></span> | <span data-ttu-id="3096d-133">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="3096d-133">The unique identifier for the password.</span></span> <span data-ttu-id="3096d-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3096d-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3096d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3096d-135">Response</span></span>

<span data-ttu-id="3096d-136">В случае успешного выполнения этот метод возвращает код отклика `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="3096d-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3096d-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="3096d-137">Examples</span></span>

<span data-ttu-id="3096d-138">В следующем примере показано, как вызвать этот API.</span><span class="sxs-lookup"><span data-stu-id="3096d-138">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="3096d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="3096d-139">Request</span></span>

<span data-ttu-id="3096d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3096d-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3096d-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="3096d-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3096d-142">C#</span><span class="sxs-lookup"><span data-stu-id="3096d-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3096d-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3096d-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3096d-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3096d-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3096d-145">Java</span><span class="sxs-lookup"><span data-stu-id="3096d-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-removepassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3096d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="3096d-146">Response</span></span>

<span data-ttu-id="3096d-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3096d-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
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

