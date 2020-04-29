---
title: Удаление schemaExtension
description: Удаление определения расширения схемы.
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 830e64db27980a8194097e3ef7be3d1da3f43d09
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509971"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="955a7-103">Удаление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="955a7-103">Delete schemaExtension</span></span>

<span data-ttu-id="955a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="955a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="955a7-105">Удаление определения [расширения схемы](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="955a7-105">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="955a7-p101">Только приложение, которое создало расширение схемы (приложение-владелец), может удалить определение расширения схемы, причем только тогда, когда расширение находится в состоянии **InDevelopment**. Удаление определения расширения схемы не влияет на доступ к пользовательским данным, добавленным в ресурс на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="955a7-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="955a7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="955a7-108">Permissions</span></span>
<span data-ttu-id="955a7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="955a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="955a7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="955a7-111">Permission type</span></span>      | <span data-ttu-id="955a7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="955a7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="955a7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="955a7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="955a7-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="955a7-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="955a7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="955a7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="955a7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="955a7-116">Not supported.</span></span>    |
|<span data-ttu-id="955a7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="955a7-117">Application</span></span> | <span data-ttu-id="955a7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="955a7-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="955a7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="955a7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="955a7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="955a7-120">Request headers</span></span>
| <span data-ttu-id="955a7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="955a7-121">Name</span></span>      |<span data-ttu-id="955a7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="955a7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="955a7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="955a7-123">Authorization</span></span>  | <span data-ttu-id="955a7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="955a7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="955a7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="955a7-126">Request body</span></span>
<span data-ttu-id="955a7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="955a7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="955a7-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="955a7-128">Response</span></span>

<span data-ttu-id="955a7-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="955a7-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="955a7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="955a7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="955a7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="955a7-132">Request</span></span>
<span data-ttu-id="955a7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="955a7-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="955a7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="955a7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/schemaExtensions/{id}
```
# <a name="c"></a>[<span data-ttu-id="955a7-135">C#</span><span class="sxs-lookup"><span data-stu-id="955a7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="955a7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="955a7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="955a7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="955a7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="955a7-138">Java</span><span class="sxs-lookup"><span data-stu-id="955a7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="955a7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="955a7-139">Response</span></span>
<span data-ttu-id="955a7-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="955a7-140">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="955a7-141">См. также</span><span class="sxs-lookup"><span data-stu-id="955a7-141">See also</span></span>

- [<span data-ttu-id="955a7-142">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="955a7-142">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="955a7-143">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="955a7-143">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
