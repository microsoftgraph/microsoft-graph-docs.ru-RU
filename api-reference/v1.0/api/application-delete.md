---
title: Удаление приложения
description: Удаление объекта Application.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b6780ab734373d82690e60137966cb10b93d8165
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992498"
---
# <a name="delete-application"></a><span data-ttu-id="40822-103">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="40822-103">Delete application</span></span>

<span data-ttu-id="40822-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40822-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40822-105">Удаление объекта [Application](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="40822-105">Delete an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40822-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40822-106">Permissions</span></span>
<span data-ttu-id="40822-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40822-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40822-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40822-109">Permission type</span></span>      | <span data-ttu-id="40822-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40822-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40822-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40822-111">Delegated (work or school account)</span></span> | <span data-ttu-id="40822-112">Application. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="40822-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="40822-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40822-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40822-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40822-114">Not supported.</span></span>    |
|<span data-ttu-id="40822-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40822-115">Application</span></span> | <span data-ttu-id="40822-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40822-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="40822-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40822-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="40822-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40822-118">Request headers</span></span>
| <span data-ttu-id="40822-119">Имя</span><span class="sxs-lookup"><span data-stu-id="40822-119">Name</span></span>       | <span data-ttu-id="40822-120">Описание</span><span class="sxs-lookup"><span data-stu-id="40822-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="40822-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40822-121">Authorization</span></span> | <span data-ttu-id="40822-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40822-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="40822-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="40822-124">Request body</span></span>
<span data-ttu-id="40822-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40822-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40822-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="40822-126">Response</span></span>

<span data-ttu-id="40822-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="40822-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40822-129">Пример</span><span class="sxs-lookup"><span data-stu-id="40822-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40822-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="40822-130">Request</span></span>
<span data-ttu-id="40822-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40822-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="40822-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="40822-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="40822-133">C#</span><span class="sxs-lookup"><span data-stu-id="40822-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40822-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40822-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40822-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40822-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40822-136">Java</span><span class="sxs-lookup"><span data-stu-id="40822-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="40822-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="40822-137">Response</span></span>
<span data-ttu-id="40822-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="40822-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

