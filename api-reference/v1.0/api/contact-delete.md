---
title: Удаление контакта
description: Удаление контакта.
author: angelgolfer-ms
ms.openlocfilehash: 17c82b895b1e2011c8efbd15fa9394cf6434fbd8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354224"
---
# <a name="delete-contact"></a><span data-ttu-id="de6b5-103">Удаление контакта</span><span class="sxs-lookup"><span data-stu-id="de6b5-103">Delete contact</span></span>

<span data-ttu-id="de6b5-104">Удаление контакта.</span><span class="sxs-lookup"><span data-stu-id="de6b5-104">Delete a contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="de6b5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de6b5-105">Permissions</span></span>
<span data-ttu-id="de6b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de6b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de6b5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de6b5-108">Permission type</span></span>      | <span data-ttu-id="de6b5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de6b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de6b5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de6b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="de6b5-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de6b5-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="de6b5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de6b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de6b5-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de6b5-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="de6b5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de6b5-114">Application</span></span> | <span data-ttu-id="de6b5-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de6b5-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="de6b5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de6b5-116">HTTP request</span></span>
<span data-ttu-id="de6b5-117"><!-- { "blockType": "ignored" } -->[Обратитесь](../resources/contact.md) в пользователя по умолчанию [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="de6b5-117"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="de6b5-118">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="de6b5-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="de6b5-p102">Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md). Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="de6b5-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="de6b5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de6b5-121">Request headers</span></span>
| <span data-ttu-id="de6b5-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de6b5-122">Header</span></span>       | <span data-ttu-id="de6b5-123">Значение</span><span class="sxs-lookup"><span data-stu-id="de6b5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de6b5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de6b5-124">Authorization</span></span>  | <span data-ttu-id="de6b5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de6b5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de6b5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de6b5-127">Request body</span></span>
<span data-ttu-id="de6b5-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de6b5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de6b5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="de6b5-129">Response</span></span>

<span data-ttu-id="de6b5-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="de6b5-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de6b5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="de6b5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de6b5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="de6b5-133">Request</span></span>
<span data-ttu-id="de6b5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de6b5-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="de6b5-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="de6b5-135">Response</span></span>
<span data-ttu-id="de6b5-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="de6b5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
