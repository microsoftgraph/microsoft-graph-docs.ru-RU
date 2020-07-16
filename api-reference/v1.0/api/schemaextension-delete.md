---
title: Удаление schemaExtension
description: Удаление определения расширения схемы.
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: b8bbdd60e979a7102f7f73e224d654eb4f1e2c56
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863153"
---
# <a name="delete-schemaextension"></a><span data-ttu-id="a5d04-103">Удаление schemaExtension</span><span class="sxs-lookup"><span data-stu-id="a5d04-103">Delete schemaExtension</span></span>

<span data-ttu-id="a5d04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5d04-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5d04-105">Удаление определения [расширения схемы](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="a5d04-105">Delete the definition of a [schema extension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="a5d04-p101">Только приложение, которое создало расширение схемы (приложение-владелец), может удалить определение расширения схемы, причем только тогда, когда расширение находится в состоянии **InDevelopment**. Удаление определения расширения схемы не влияет на доступ к пользовательским данным, добавленным в ресурс на основе этого определения.</span><span class="sxs-lookup"><span data-stu-id="a5d04-p101">Only the app that created the schema extension (owner app) can delete the schema extension definition, and only when the extension is in the **InDevelopment** state. Deleting a schema extension definition does not affect accessing custom data that has been added to resource instances based on that definition.</span></span>


## <a name="permissions"></a><span data-ttu-id="a5d04-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5d04-108">Permissions</span></span>
<span data-ttu-id="a5d04-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5d04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a5d04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5d04-111">Permission type</span></span>      | <span data-ttu-id="a5d04-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5d04-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5d04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5d04-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a5d04-114">Application. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="a5d04-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a5d04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5d04-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5d04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5d04-116">Not supported.</span></span>    |
|<span data-ttu-id="a5d04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5d04-117">Application</span></span> | <span data-ttu-id="a5d04-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5d04-118">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="a5d04-119">Кроме того, для делегированного процесса вошедшего в систему пользователя можно удалить только schemaExtensions, которыми они владеют (где свойство **owner** объекта schemaExtension — это `appId` приложение, которому принадлежит вошедшего пользователь).</span><span class="sxs-lookup"><span data-stu-id="a5d04-119">Additionally for the delegated flow, the signed-in user can only delete schemaExtensions they own (where the **owner** property of the schemaExtension is the `appId` of an application the signed-in user owns).</span></span>

## <a name="http-request"></a><span data-ttu-id="a5d04-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5d04-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a5d04-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5d04-121">Request headers</span></span>
| <span data-ttu-id="a5d04-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a5d04-122">Name</span></span>      |<span data-ttu-id="a5d04-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a5d04-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a5d04-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5d04-124">Authorization</span></span>  | <span data-ttu-id="a5d04-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5d04-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5d04-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5d04-127">Request body</span></span>
<span data-ttu-id="a5d04-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5d04-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5d04-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5d04-129">Response</span></span>

<span data-ttu-id="a5d04-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a5d04-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5d04-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a5d04-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5d04-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5d04-133">Request</span></span>
<span data-ttu-id="a5d04-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5d04-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5d04-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5d04-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/schemaExtensions/{id}
```
# <a name="c"></a>[<span data-ttu-id="a5d04-136">C#</span><span class="sxs-lookup"><span data-stu-id="a5d04-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5d04-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5d04-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5d04-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5d04-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5d04-139">Java</span><span class="sxs-lookup"><span data-stu-id="a5d04-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a5d04-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5d04-140">Response</span></span>
<span data-ttu-id="a5d04-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a5d04-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="a5d04-142">См. также</span><span class="sxs-lookup"><span data-stu-id="a5d04-142">See also</span></span>

- [<span data-ttu-id="a5d04-143">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="a5d04-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a5d04-144">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="a5d04-144">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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
