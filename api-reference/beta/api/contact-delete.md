---
title: Удаление контакта
description: Удаление контакта.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9f3e0a56d3c9f4b1a1858dc350e264eb18a11056
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591753"
---
# <a name="delete-contact"></a><span data-ttu-id="a8474-103">Удаление контакта</span><span class="sxs-lookup"><span data-stu-id="a8474-103">Delete contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8474-104">Удаление контакта.</span><span class="sxs-lookup"><span data-stu-id="a8474-104">Delete contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="a8474-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8474-105">Permissions</span></span>
<span data-ttu-id="a8474-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8474-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8474-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8474-108">Permission type</span></span>      | <span data-ttu-id="a8474-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8474-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8474-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8474-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a8474-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8474-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a8474-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8474-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8474-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8474-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a8474-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8474-114">Application</span></span> | <span data-ttu-id="a8474-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a8474-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8474-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8474-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a8474-117">[Контакт](../resources/contact.md) от [contactFolder](../resources/contactfolder.md)пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a8474-117">A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="a8474-118">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="a8474-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="a8474-119">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a8474-119">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="a8474-120">Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="a8474-120">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a8474-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8474-121">Request headers</span></span>
| <span data-ttu-id="a8474-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8474-122">Header</span></span>       | <span data-ttu-id="a8474-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a8474-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a8474-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8474-124">Authorization</span></span>  | <span data-ttu-id="a8474-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8474-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a8474-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8474-127">Request body</span></span>
<span data-ttu-id="a8474-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8474-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8474-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8474-129">Response</span></span>

<span data-ttu-id="a8474-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a8474-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8474-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a8474-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8474-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8474-133">Request</span></span>
<span data-ttu-id="a8474-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8474-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="a8474-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8474-135">Response</span></span>
<span data-ttu-id="a8474-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8474-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a8474-139">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="a8474-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a8474-140">Языках</span><span class="sxs-lookup"><span data-stu-id="a8474-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_contact-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8474-141">Язык</span><span class="sxs-lookup"><span data-stu-id="a8474-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_contact-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/contact-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/contact-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
