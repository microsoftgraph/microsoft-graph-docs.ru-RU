---
title: Удаление приложения
description: Удаление объекта приложения.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: da60fd5c6a3a97a3924fc45448c00f9665748752
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131784"
---
# <a name="delete-application"></a><span data-ttu-id="ead2c-103">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="ead2c-103">Delete application</span></span>

<span data-ttu-id="ead2c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ead2c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ead2c-105">Удаление [объекта](../resources/application.md) приложения.</span><span class="sxs-lookup"><span data-stu-id="ead2c-105">Delete an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ead2c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ead2c-106">Permissions</span></span>
<span data-ttu-id="ead2c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ead2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ead2c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ead2c-109">Permission type</span></span>      | <span data-ttu-id="ead2c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ead2c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ead2c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ead2c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ead2c-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ead2c-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ead2c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ead2c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ead2c-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ead2c-114">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="ead2c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ead2c-115">Application</span></span> | <span data-ttu-id="ead2c-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ead2c-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ead2c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ead2c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ead2c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ead2c-118">Request headers</span></span>
| <span data-ttu-id="ead2c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ead2c-119">Name</span></span>       | <span data-ttu-id="ead2c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ead2c-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="ead2c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ead2c-121">Authorization</span></span> | <span data-ttu-id="ead2c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ead2c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ead2c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ead2c-124">Request body</span></span>
<span data-ttu-id="ead2c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ead2c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ead2c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="ead2c-126">Response</span></span>

<span data-ttu-id="ead2c-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ead2c-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ead2c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ead2c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ead2c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ead2c-130">Request</span></span>
<span data-ttu-id="ead2c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ead2c-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ead2c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ead2c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}
```
# <a name="c"></a>[<span data-ttu-id="ead2c-133">C#</span><span class="sxs-lookup"><span data-stu-id="ead2c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ead2c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ead2c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ead2c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ead2c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ead2c-136">Java</span><span class="sxs-lookup"><span data-stu-id="ead2c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ead2c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ead2c-137">Response</span></span>
<span data-ttu-id="ead2c-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ead2c-138">Here is an example of the response.</span></span> 
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

