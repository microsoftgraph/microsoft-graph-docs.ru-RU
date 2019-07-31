---
title: Удаление schemaExtension
description: Удаление определения расширения схемы.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 3125ae80680e1d9f7b6f7ea5f3732332786283b8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978075"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="8ab94-103">Удаление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="8ab94-103">Delete schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ab94-104">Удаление определения [расширения схемы](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="8ab94-104">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="8ab94-p101">Только приложение, которое создало расширение схемы (приложение-владелец), может удалить определение расширения схемы, причем только тогда, когда расширение находится в состоянии **InDevelopment**. Удаление определения расширения схемы не влияет на доступ к пользовательским данным, добавленным в ресурс на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="8ab94-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="8ab94-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ab94-107">Permissions</span></span>
<span data-ttu-id="8ab94-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ab94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8ab94-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ab94-110">Permission type</span></span>      | <span data-ttu-id="8ab94-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ab94-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ab94-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ab94-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8ab94-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8ab94-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8ab94-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ab94-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ab94-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ab94-115">Not supported.</span></span>    |
|<span data-ttu-id="8ab94-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ab94-116">Application</span></span> | <span data-ttu-id="8ab94-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ab94-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ab94-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ab94-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8ab94-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ab94-119">Request headers</span></span>
| <span data-ttu-id="8ab94-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8ab94-120">Name</span></span>      |<span data-ttu-id="8ab94-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8ab94-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8ab94-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ab94-122">Authorization</span></span>  | <span data-ttu-id="8ab94-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ab94-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ab94-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ab94-125">Request body</span></span>
<span data-ttu-id="8ab94-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ab94-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ab94-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ab94-127">Response</span></span>

<span data-ttu-id="8ab94-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8ab94-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ab94-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8ab94-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ab94-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ab94-131">Request</span></span>
<span data-ttu-id="8ab94-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ab94-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8ab94-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ab94-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ab94-134">C#</span><span class="sxs-lookup"><span data-stu-id="8ab94-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ab94-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="8ab94-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ab94-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8ab94-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8ab94-137">Java</span><span class="sxs-lookup"><span data-stu-id="8ab94-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8ab94-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ab94-138">Response</span></span>
<span data-ttu-id="8ab94-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8ab94-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="8ab94-140">См. также</span><span class="sxs-lookup"><span data-stu-id="8ab94-140">See also</span></span>

- [<span data-ttu-id="8ab94-141">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="8ab94-141">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="8ab94-142">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="8ab94-142">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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
