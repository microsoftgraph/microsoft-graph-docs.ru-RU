---
title: Добавление владельца
description: Используйте этот API, чтобы добавить владельца в приложение.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 95642607e2a43797683f494807fb47a147216c28
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048080"
---
# <a name="add-owner"></a><span data-ttu-id="1c6d0-103">Добавление владельца</span><span class="sxs-lookup"><span data-stu-id="1c6d0-103">Add owner</span></span>

<span data-ttu-id="1c6d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c6d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c6d0-105">Используйте этот API, чтобы добавить владельца в приложение, разместив его в коллекции владельцев.</span><span class="sxs-lookup"><span data-stu-id="1c6d0-105">Use this API to add an owner to an application by posting to the owners collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c6d0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c6d0-106">Permissions</span></span>
<span data-ttu-id="1c6d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c6d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c6d0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c6d0-109">Permission type</span></span>      | <span data-ttu-id="1c6d0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c6d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c6d0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c6d0-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="1c6d0-112">Application.ReadWrite.All и Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1c6d0-112">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1c6d0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c6d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c6d0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c6d0-114">Not supported.</span></span>    |
|<span data-ttu-id="1c6d0-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1c6d0-115">Application</span></span> | <span data-ttu-id="1c6d0-116">Application.ReadWrite.OwnedBy и Directory.Read.All, Application.ReadWrite.All и Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c6d0-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c6d0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c6d0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="1c6d0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c6d0-118">Request headers</span></span>
| <span data-ttu-id="1c6d0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1c6d0-119">Name</span></span> | <span data-ttu-id="1c6d0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1c6d0-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="1c6d0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c6d0-121">Authorization</span></span> | <span data-ttu-id="1c6d0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c6d0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1c6d0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c6d0-124">Request body</span></span>
<span data-ttu-id="1c6d0-125">В теле запроса укажи идентификатор объекта каталога, назначенного в качестве владельца.</span><span class="sxs-lookup"><span data-stu-id="1c6d0-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="1c6d0-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c6d0-126">Response</span></span>

<span data-ttu-id="1c6d0-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1c6d0-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1c6d0-128">Пример</span><span class="sxs-lookup"><span data-stu-id="1c6d0-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c6d0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c6d0-129">Request</span></span>
<span data-ttu-id="1c6d0-130">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c6d0-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c6d0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c6d0-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
"@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}

```
# <a name="javascript"></a>[<span data-ttu-id="1c6d0-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c6d0-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="1c6d0-133">C#</span><span class="sxs-lookup"><span data-stu-id="1c6d0-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c6d0-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c6d0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c6d0-135">Java</span><span class="sxs-lookup"><span data-stu-id="1c6d0-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="1c6d0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c6d0-136">Response</span></span>

<span data-ttu-id="1c6d0-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1c6d0-137">The following is an example of the response.</span></span>

><span data-ttu-id="1c6d0-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1c6d0-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



