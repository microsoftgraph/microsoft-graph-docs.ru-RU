---
title: Удаление контакта
description: Удаление контакта.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 795a3bc5526f3276cc04cae294a886c5966160b5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053267"
---
# <a name="delete-contact"></a><span data-ttu-id="85bc5-103">Удаление контакта</span><span class="sxs-lookup"><span data-stu-id="85bc5-103">Delete contact</span></span>

<span data-ttu-id="85bc5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85bc5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85bc5-105">Удаление контакта.</span><span class="sxs-lookup"><span data-stu-id="85bc5-105">Delete a contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="85bc5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85bc5-106">Permissions</span></span>
<span data-ttu-id="85bc5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85bc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85bc5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85bc5-109">Permission type</span></span>      | <span data-ttu-id="85bc5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85bc5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85bc5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85bc5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="85bc5-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85bc5-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="85bc5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85bc5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85bc5-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85bc5-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="85bc5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85bc5-115">Application</span></span> | <span data-ttu-id="85bc5-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85bc5-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="85bc5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85bc5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="85bc5-118">Объект [contact](../resources/contact.md) из стандартной пользовательской папки [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="85bc5-118">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="85bc5-119">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="85bc5-119">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="85bc5-p102">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md). Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="85bc5-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="85bc5-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85bc5-122">Request headers</span></span>
| <span data-ttu-id="85bc5-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85bc5-123">Header</span></span>       | <span data-ttu-id="85bc5-124">Значение</span><span class="sxs-lookup"><span data-stu-id="85bc5-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="85bc5-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85bc5-125">Authorization</span></span>  | <span data-ttu-id="85bc5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85bc5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="85bc5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85bc5-128">Request body</span></span>
<span data-ttu-id="85bc5-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85bc5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85bc5-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="85bc5-130">Response</span></span>

<span data-ttu-id="85bc5-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="85bc5-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85bc5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="85bc5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85bc5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="85bc5-134">Request</span></span>
<span data-ttu-id="85bc5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85bc5-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85bc5-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="85bc5-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="85bc5-137">C#</span><span class="sxs-lookup"><span data-stu-id="85bc5-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85bc5-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85bc5-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85bc5-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85bc5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85bc5-140">Java</span><span class="sxs-lookup"><span data-stu-id="85bc5-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="85bc5-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="85bc5-141">Response</span></span>
<span data-ttu-id="85bc5-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="85bc5-142">Here is an example of the response.</span></span> <span data-ttu-id="85bc5-143">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="85bc5-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

