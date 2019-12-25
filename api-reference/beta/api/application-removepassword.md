---
title: 'Приложение: Ремовепассворд'
description: Удаление пароля из приложения
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6a83c1e128d319f76a4e52fad91a59193811b390
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "37994966"
---
# <a name="application-removepassword"></a><span data-ttu-id="0bba7-103">Приложение: Ремовепассворд</span><span class="sxs-lookup"><span data-stu-id="0bba7-103">application: removePassword</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bba7-104">Удаляет пароль из [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="0bba7-104">Removes a password from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0bba7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0bba7-105">Permissions</span></span>

<span data-ttu-id="0bba7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bba7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0bba7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0bba7-108">Permission type</span></span>                        | <span data-ttu-id="0bba7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0bba7-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0bba7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0bba7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0bba7-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0bba7-111">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="0bba7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0bba7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bba7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bba7-113">Not supported.</span></span> |
| <span data-ttu-id="0bba7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0bba7-114">Application</span></span>                            | <span data-ttu-id="0bba7-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bba7-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bba7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0bba7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="0bba7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0bba7-117">Request headers</span></span>

| <span data-ttu-id="0bba7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0bba7-118">Name</span></span>           | <span data-ttu-id="0bba7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0bba7-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="0bba7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0bba7-120">Authorization</span></span>  | <span data-ttu-id="0bba7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0bba7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0bba7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0bba7-123">Content-type</span></span>   | <span data-ttu-id="0bba7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0bba7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bba7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0bba7-126">Request body</span></span>

| <span data-ttu-id="0bba7-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="0bba7-127">Property</span></span>  | <span data-ttu-id="0bba7-128">Тип</span><span class="sxs-lookup"><span data-stu-id="0bba7-128">Type</span></span> | <span data-ttu-id="0bba7-129">Описание</span><span class="sxs-lookup"><span data-stu-id="0bba7-129">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="0bba7-130">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="0bba7-130">keyId</span></span>     | <span data-ttu-id="0bba7-131">GUID</span><span class="sxs-lookup"><span data-stu-id="0bba7-131">GUID</span></span> | <span data-ttu-id="0bba7-132">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="0bba7-132">The unique identifier for the password.</span></span> <span data-ttu-id="0bba7-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0bba7-133">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0bba7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bba7-134">Response</span></span>

<span data-ttu-id="0bba7-135">В случае успешного выполнения этот метод возвращает код отклика `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="0bba7-135">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0bba7-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="0bba7-136">Examples</span></span>

<span data-ttu-id="0bba7-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="0bba7-137">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="0bba7-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bba7-138">Request</span></span>

<span data-ttu-id="0bba7-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0bba7-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0bba7-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="0bba7-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="0bba7-141">C#</span><span class="sxs-lookup"><span data-stu-id="0bba7-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0bba7-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0bba7-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0bba7-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0bba7-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0bba7-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bba7-144">Response</span></span>

<span data-ttu-id="0bba7-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0bba7-145">The following is an example of the response.</span></span>

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
