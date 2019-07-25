---
title: Удаление контакта
description: Удаление контакта.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 100ee24b18889484df103505a16f5f9844b72152
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863477"
---
# <a name="delete-contact"></a><span data-ttu-id="9ae6d-103">Удаление контакта</span><span class="sxs-lookup"><span data-stu-id="9ae6d-103">Delete contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ae6d-104">Удаление контакта.</span><span class="sxs-lookup"><span data-stu-id="9ae6d-104">Delete contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="9ae6d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ae6d-105">Permissions</span></span>
<span data-ttu-id="9ae6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ae6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ae6d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ae6d-108">Permission type</span></span>      | <span data-ttu-id="9ae6d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ae6d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ae6d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ae6d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9ae6d-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ae6d-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9ae6d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ae6d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ae6d-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ae6d-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9ae6d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ae6d-114">Application</span></span> | <span data-ttu-id="9ae6d-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ae6d-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ae6d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ae6d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="9ae6d-117">[Контакт](../resources/contact.md) от [contactFolder](../resources/contactfolder.md)пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9ae6d-117">A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="9ae6d-118">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="9ae6d-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="9ae6d-119">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="9ae6d-119">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="9ae6d-120">Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="9ae6d-120">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9ae6d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ae6d-121">Request headers</span></span>
| <span data-ttu-id="9ae6d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ae6d-122">Header</span></span>       | <span data-ttu-id="9ae6d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9ae6d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ae6d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ae6d-124">Authorization</span></span>  | <span data-ttu-id="9ae6d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ae6d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9ae6d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9ae6d-127">Request body</span></span>
<span data-ttu-id="9ae6d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ae6d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ae6d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ae6d-129">Response</span></span>

<span data-ttu-id="9ae6d-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9ae6d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ae6d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9ae6d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ae6d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ae6d-133">Request</span></span>
<span data-ttu-id="9ae6d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ae6d-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9ae6d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ae6d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contacts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ae6d-136">C#</span><span class="sxs-lookup"><span data-stu-id="9ae6d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ae6d-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="9ae6d-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ae6d-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9ae6d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9ae6d-139">Java</span><span class="sxs-lookup"><span data-stu-id="9ae6d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9ae6d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ae6d-140">Response</span></span>
<span data-ttu-id="9ae6d-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ae6d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
