---
title: Удаление владельца
description: Удаление владельца приложения.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 034e8299ec1a5a05f1fa307f0196aed2113aebbc
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786077"
---
# <a name="remove-owner"></a><span data-ttu-id="f4606-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="f4606-103">Remove owner</span></span>

<span data-ttu-id="f4606-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4606-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4606-105">Удаление владельца из [приложения.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="f4606-105">Remove an owner from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f4606-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4606-106">Permissions</span></span>
<span data-ttu-id="f4606-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4606-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4606-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4606-109">Permission type</span></span>      | <span data-ttu-id="f4606-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4606-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4606-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4606-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f4606-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f4606-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f4606-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4606-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4606-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4606-114">Not supported.</span></span>    |
|<span data-ttu-id="f4606-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4606-115">Application</span></span> | <span data-ttu-id="f4606-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4606-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4606-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4606-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}/owners/{id}/$ref

```
## <a name="request-headers"></a><span data-ttu-id="f4606-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4606-118">Request headers</span></span>
| <span data-ttu-id="f4606-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f4606-119">Name</span></span> | <span data-ttu-id="f4606-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f4606-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="f4606-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4606-121">Authorization</span></span> | <span data-ttu-id="f4606-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4606-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f4606-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f4606-124">Request body</span></span>
<span data-ttu-id="f4606-125">В теле запроса укажи идентификатор объекта каталога, назначенного в качестве владельца.</span><span class="sxs-lookup"><span data-stu-id="f4606-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="f4606-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4606-126">Response</span></span>

<span data-ttu-id="f4606-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f4606-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f4606-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f4606-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4606-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4606-129">Request</span></span>

<span data-ttu-id="f4606-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4606-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f4606-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4606-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delete_owners"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="f4606-132">C#</span><span class="sxs-lookup"><span data-stu-id="f4606-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delete-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4606-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4606-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delete-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4606-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4606-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delete-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4606-135">Java</span><span class="sxs-lookup"><span data-stu-id="f4606-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delete-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f4606-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4606-136">Response</span></span>

<span data-ttu-id="f4606-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f4606-137">The following is an example of the response.</span></span>

><span data-ttu-id="f4606-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f4606-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

