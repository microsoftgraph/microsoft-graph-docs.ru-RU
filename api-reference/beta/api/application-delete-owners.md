---
title: Удаление владельца
description: Удаление владельца приложения.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 9bb43da4007e56cfae7d3b881ca3fd53f3bbf679
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048164"
---
# <a name="remove-owner"></a><span data-ttu-id="f23b3-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="f23b3-103">Remove owner</span></span>

<span data-ttu-id="f23b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f23b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f23b3-105">Удаление владельца из [приложения.](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="f23b3-105">Remove an owner from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f23b3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f23b3-106">Permissions</span></span>
<span data-ttu-id="f23b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f23b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f23b3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f23b3-109">Permission type</span></span>      | <span data-ttu-id="f23b3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f23b3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f23b3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f23b3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f23b3-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f23b3-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f23b3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f23b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f23b3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f23b3-114">Not supported.</span></span>    |
|<span data-ttu-id="f23b3-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f23b3-115">Application</span></span> | <span data-ttu-id="f23b3-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f23b3-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f23b3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f23b3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}/owners/{id}/$ref

```
## <a name="request-headers"></a><span data-ttu-id="f23b3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f23b3-118">Request headers</span></span>
| <span data-ttu-id="f23b3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f23b3-119">Name</span></span> | <span data-ttu-id="f23b3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f23b3-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="f23b3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f23b3-121">Authorization</span></span> | <span data-ttu-id="f23b3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f23b3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f23b3-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f23b3-124">Request body</span></span>
<span data-ttu-id="f23b3-125">В теле запроса укажи идентификатор объекта каталога, назначенного в качестве владельца.</span><span class="sxs-lookup"><span data-stu-id="f23b3-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="f23b3-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f23b3-126">Response</span></span>

<span data-ttu-id="f23b3-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f23b3-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f23b3-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f23b3-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="f23b3-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f23b3-129">Request</span></span>

<span data-ttu-id="f23b3-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f23b3-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f23b3-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f23b3-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delete_owners"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/owners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="f23b3-132">C#</span><span class="sxs-lookup"><span data-stu-id="f23b3-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delete-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f23b3-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f23b3-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delete-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f23b3-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f23b3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delete-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f23b3-135">Java</span><span class="sxs-lookup"><span data-stu-id="f23b3-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delete-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f23b3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f23b3-136">Response</span></span>

<span data-ttu-id="f23b3-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f23b3-137">The following is an example of the response.</span></span>

><span data-ttu-id="f23b3-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f23b3-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
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



