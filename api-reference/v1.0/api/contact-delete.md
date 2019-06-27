---
title: Удаление контакта
description: Удаление контакта.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3235e460c43aa2c4062ffbbbcb798d2e6a6043fe
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277527"
---
# <a name="delete-contact"></a><span data-ttu-id="0d42a-103">Удаление контакта</span><span class="sxs-lookup"><span data-stu-id="0d42a-103">Delete contact</span></span>

<span data-ttu-id="0d42a-104">Удаление контакта.</span><span class="sxs-lookup"><span data-stu-id="0d42a-104">Delete a contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="0d42a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d42a-105">Permissions</span></span>
<span data-ttu-id="0d42a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d42a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d42a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d42a-108">Permission type</span></span>      | <span data-ttu-id="0d42a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d42a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d42a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d42a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0d42a-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d42a-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0d42a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d42a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d42a-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d42a-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0d42a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d42a-114">Application</span></span> | <span data-ttu-id="0d42a-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d42a-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d42a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d42a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="0d42a-117">Объект [contact](../resources/contact.md) из стандартной пользовательской папки [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="0d42a-117">A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="0d42a-118">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="0d42a-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="0d42a-p102">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md). Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="0d42a-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0d42a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d42a-121">Request headers</span></span>
| <span data-ttu-id="0d42a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d42a-122">Header</span></span>       | <span data-ttu-id="0d42a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0d42a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0d42a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d42a-124">Authorization</span></span>  | <span data-ttu-id="0d42a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d42a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0d42a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0d42a-127">Request body</span></span>
<span data-ttu-id="0d42a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0d42a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d42a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d42a-129">Response</span></span>

<span data-ttu-id="0d42a-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0d42a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d42a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0d42a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d42a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d42a-133">Request</span></span>
<span data-ttu-id="0d42a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d42a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="0d42a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d42a-135">Response</span></span>
<span data-ttu-id="0d42a-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d42a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0d42a-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="0d42a-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0d42a-140">C#</span><span class="sxs-lookup"><span data-stu-id="0d42a-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_contact-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d42a-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="0d42a-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_contact-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0d42a-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0d42a-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_contact-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/contact-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/contact-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/contact-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
