---
title: 'Приложение: Ремовепассворд'
description: Удаление пароля из приложения
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bac7ed6bd5ee15cd917c8467d3b12ef696bbdf51
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441447"
---
# <a name="application-removepassword"></a><span data-ttu-id="d2380-103">Приложение: Ремовепассворд</span><span class="sxs-lookup"><span data-stu-id="d2380-103">application: removePassword</span></span>

<span data-ttu-id="d2380-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d2380-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2380-105">Удаляет пароль из [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="d2380-105">Removes a password from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d2380-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2380-106">Permissions</span></span>

<span data-ttu-id="d2380-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2380-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2380-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2380-109">Permission type</span></span>                        | <span data-ttu-id="d2380-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2380-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d2380-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2380-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2380-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d2380-112">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="d2380-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2380-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2380-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2380-114">Not supported.</span></span> |
| <span data-ttu-id="d2380-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2380-115">Application</span></span>                            | <span data-ttu-id="d2380-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2380-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2380-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2380-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="d2380-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2380-118">Request headers</span></span>

| <span data-ttu-id="d2380-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d2380-119">Name</span></span>           | <span data-ttu-id="d2380-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d2380-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="d2380-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2380-121">Authorization</span></span>  | <span data-ttu-id="d2380-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2380-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d2380-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2380-124">Content-type</span></span>   | <span data-ttu-id="d2380-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2380-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2380-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2380-127">Request body</span></span>

| <span data-ttu-id="d2380-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2380-128">Property</span></span>  | <span data-ttu-id="d2380-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d2380-129">Type</span></span> | <span data-ttu-id="d2380-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d2380-130">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="d2380-131">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="d2380-131">keyId</span></span>     | <span data-ttu-id="d2380-132">GUID</span><span class="sxs-lookup"><span data-stu-id="d2380-132">GUID</span></span> | <span data-ttu-id="d2380-133">Уникальный идентификатор пароля.</span><span class="sxs-lookup"><span data-stu-id="d2380-133">The unique identifier for the password.</span></span> <span data-ttu-id="d2380-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2380-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d2380-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2380-135">Response</span></span>

<span data-ttu-id="d2380-136">В случае успешного выполнения этот метод возвращает код отклика `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="d2380-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d2380-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="d2380-137">Examples</span></span>

<span data-ttu-id="d2380-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="d2380-138">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d2380-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2380-139">Request</span></span>

<span data-ttu-id="d2380-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2380-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2380-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2380-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d2380-142">C#</span><span class="sxs-lookup"><span data-stu-id="d2380-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2380-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2380-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2380-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2380-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d2380-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2380-145">Response</span></span>

<span data-ttu-id="d2380-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d2380-146">The following is an example of the response.</span></span>

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
