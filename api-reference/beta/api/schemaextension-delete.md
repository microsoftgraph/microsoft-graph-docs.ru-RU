---
title: Удаление schemaExtension
description: Удаление определения расширения схемы.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: ac09d3c34539ca2454fbe616fa1b9c9cd1decc00
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453788"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="8c8bf-103">Удаление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="8c8bf-103">Delete schemaExtension</span></span>

<span data-ttu-id="8c8bf-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8c8bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c8bf-105">Удаление определения [расширения схемы](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="8c8bf-105">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="8c8bf-p101">Только приложение, которое создало расширение схемы (приложение-владелец), может удалить определение расширения схемы, причем только тогда, когда расширение находится в состоянии **InDevelopment**. Удаление определения расширения схемы не влияет на доступ к пользовательским данным, добавленным в ресурс на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="8c8bf-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="8c8bf-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c8bf-108">Permissions</span></span>
<span data-ttu-id="8c8bf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c8bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8c8bf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c8bf-111">Permission type</span></span>      | <span data-ttu-id="8c8bf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c8bf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c8bf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c8bf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8c8bf-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8c8bf-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8c8bf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c8bf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c8bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c8bf-116">Not supported.</span></span>    |
|<span data-ttu-id="8c8bf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c8bf-117">Application</span></span> | <span data-ttu-id="8c8bf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c8bf-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c8bf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c8bf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8c8bf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c8bf-120">Request headers</span></span>
| <span data-ttu-id="8c8bf-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8c8bf-121">Name</span></span>      |<span data-ttu-id="8c8bf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8c8bf-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c8bf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c8bf-123">Authorization</span></span>  | <span data-ttu-id="8c8bf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c8bf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c8bf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c8bf-126">Request body</span></span>
<span data-ttu-id="8c8bf-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c8bf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c8bf-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c8bf-128">Response</span></span>

<span data-ttu-id="8c8bf-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8c8bf-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c8bf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8c8bf-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c8bf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c8bf-132">Request</span></span>
<span data-ttu-id="8c8bf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c8bf-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8c8bf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c8bf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
# <a name="c"></a>[<span data-ttu-id="8c8bf-135">C#</span><span class="sxs-lookup"><span data-stu-id="8c8bf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c8bf-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c8bf-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c8bf-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c8bf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8c8bf-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c8bf-138">Response</span></span>
<span data-ttu-id="8c8bf-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c8bf-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="8c8bf-140">См. также</span><span class="sxs-lookup"><span data-stu-id="8c8bf-140">See also</span></span>

- [<span data-ttu-id="8c8bf-141">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="8c8bf-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="8c8bf-142">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="8c8bf-142">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
