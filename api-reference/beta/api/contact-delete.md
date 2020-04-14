---
title: Удаление контакта
description: Удаление контакта.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 909e0d8e3b0e3e811035db29c071c476b562487a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43382086"
---
# <a name="delete-contact"></a><span data-ttu-id="88fdd-103">Удаление контакта</span><span class="sxs-lookup"><span data-stu-id="88fdd-103">Delete contact</span></span>

<span data-ttu-id="88fdd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88fdd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88fdd-105">Удаление контакта.</span><span class="sxs-lookup"><span data-stu-id="88fdd-105">Delete contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="88fdd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="88fdd-106">Permissions</span></span>
<span data-ttu-id="88fdd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88fdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88fdd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88fdd-109">Permission type</span></span>      | <span data-ttu-id="88fdd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="88fdd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88fdd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88fdd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="88fdd-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88fdd-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="88fdd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88fdd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88fdd-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88fdd-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="88fdd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88fdd-115">Application</span></span> | <span data-ttu-id="88fdd-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="88fdd-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="88fdd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88fdd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="88fdd-118">[Контакт](../resources/contact.md) от [contactFolder](../resources/contactfolder.md)пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="88fdd-118">A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="88fdd-119">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="88fdd-119">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="88fdd-120">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="88fdd-120">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="88fdd-121">Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="88fdd-121">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="88fdd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88fdd-122">Request headers</span></span>
| <span data-ttu-id="88fdd-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88fdd-123">Header</span></span>       | <span data-ttu-id="88fdd-124">Значение</span><span class="sxs-lookup"><span data-stu-id="88fdd-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="88fdd-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88fdd-125">Authorization</span></span>  | <span data-ttu-id="88fdd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88fdd-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="88fdd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="88fdd-128">Request body</span></span>
<span data-ttu-id="88fdd-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88fdd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88fdd-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="88fdd-130">Response</span></span>

<span data-ttu-id="88fdd-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="88fdd-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88fdd-133">Пример</span><span class="sxs-lookup"><span data-stu-id="88fdd-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="88fdd-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="88fdd-134">Request</span></span>
<span data-ttu-id="88fdd-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88fdd-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="88fdd-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="88fdd-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="88fdd-137">C#</span><span class="sxs-lookup"><span data-stu-id="88fdd-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88fdd-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88fdd-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88fdd-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88fdd-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="88fdd-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="88fdd-140">Response</span></span>
<span data-ttu-id="88fdd-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88fdd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
