---
title: Удаление владельца
description: Удаление владельца приложения.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 84728c7c4e7c37eb49b4f0cd02087e80b77dbf00
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "37999094"
---
# <a name="remove-owner"></a><span data-ttu-id="17aba-103">Удаление владельца</span><span class="sxs-lookup"><span data-stu-id="17aba-103">Remove owner</span></span>

<span data-ttu-id="17aba-104">Удаление владельца из [приложения](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="17aba-104">Remove an owner from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="17aba-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="17aba-105">Permissions</span></span>
<span data-ttu-id="17aba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17aba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17aba-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17aba-108">Permission type</span></span>      | <span data-ttu-id="17aba-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17aba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17aba-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17aba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="17aba-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="17aba-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="17aba-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17aba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17aba-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17aba-113">Not supported.</span></span>    |
|<span data-ttu-id="17aba-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17aba-114">Application</span></span> | <span data-ttu-id="17aba-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17aba-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17aba-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17aba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/{id}/$ref

```
## <a name="request-headers"></a><span data-ttu-id="17aba-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17aba-117">Request headers</span></span>
| <span data-ttu-id="17aba-118">Имя</span><span class="sxs-lookup"><span data-stu-id="17aba-118">Name</span></span> | <span data-ttu-id="17aba-119">Описание</span><span class="sxs-lookup"><span data-stu-id="17aba-119">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="17aba-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17aba-120">Authorization</span></span> | <span data-ttu-id="17aba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17aba-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="17aba-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17aba-123">Request body</span></span>
<span data-ttu-id="17aba-124">В тексте запроса укажите идентификатор объекта каталога, который необходимо назначить владельцем.</span><span class="sxs-lookup"><span data-stu-id="17aba-124">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="17aba-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="17aba-125">Response</span></span>

<span data-ttu-id="17aba-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="17aba-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="17aba-127">Пример</span><span class="sxs-lookup"><span data-stu-id="17aba-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="17aba-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="17aba-128">Request</span></span>

<span data-ttu-id="17aba-129">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17aba-129">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="17aba-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="17aba-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_delete_owners"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/owners/{id}/$ref
Content-type: application/json
Content-length: 30

{
"@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="17aba-131">C#</span><span class="sxs-lookup"><span data-stu-id="17aba-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-delete-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="17aba-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17aba-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-delete-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="17aba-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17aba-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-delete-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="17aba-134">Java</span><span class="sxs-lookup"><span data-stu-id="17aba-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-delete-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="17aba-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="17aba-135">Response</span></span>

<span data-ttu-id="17aba-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="17aba-136">The following is an example of the response.</span></span>

><span data-ttu-id="17aba-137">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="17aba-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="17aba-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17aba-138">All the properties will be returned from an actual call.</span></span>

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
