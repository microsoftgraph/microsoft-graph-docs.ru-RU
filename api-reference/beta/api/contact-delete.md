---
title: Удаление контакта
description: Удаление контакта.
author: angelgolfer-ms
ms.openlocfilehash: a8f1ea8c1ee0f202e60d4efb05f65022a9269c01
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319273"
---
# <a name="delete-contact"></a><span data-ttu-id="34c27-103">Удаление контакта</span><span class="sxs-lookup"><span data-stu-id="34c27-103">Delete contact</span></span>

> <span data-ttu-id="34c27-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="34c27-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34c27-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34c27-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34c27-106">Удаление контакта.</span><span class="sxs-lookup"><span data-stu-id="34c27-106">Delete contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="34c27-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34c27-107">Permissions</span></span>
<span data-ttu-id="34c27-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34c27-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34c27-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34c27-110">Permission type</span></span>      | <span data-ttu-id="34c27-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34c27-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34c27-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34c27-112">Delegated (work or school account)</span></span> | <span data-ttu-id="34c27-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c27-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="34c27-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34c27-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34c27-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c27-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="34c27-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34c27-116">Application</span></span> | <span data-ttu-id="34c27-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34c27-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="34c27-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34c27-118">HTTP request</span></span>
<span data-ttu-id="34c27-119"><!-- { "blockType": "ignored" } -->[Обратитесь](../resources/contact.md) в пользователя по умолчанию [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="34c27-119"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="34c27-120">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="34c27-120">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="34c27-121">[Обратитесь](../resources/contact.md) в дочерней папкой [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="34c27-121">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="34c27-122">В приведенном ниже примере показана один уровень вложения, но контакт может быть найдена в дочерних дочернего и т. д.</span><span class="sxs-lookup"><span data-stu-id="34c27-122">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="34c27-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34c27-123">Request headers</span></span>
| <span data-ttu-id="34c27-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34c27-124">Header</span></span>       | <span data-ttu-id="34c27-125">Значение</span><span class="sxs-lookup"><span data-stu-id="34c27-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="34c27-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34c27-126">Authorization</span></span>  | <span data-ttu-id="34c27-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34c27-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="34c27-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34c27-129">Request body</span></span>
<span data-ttu-id="34c27-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34c27-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34c27-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="34c27-131">Response</span></span>

<span data-ttu-id="34c27-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="34c27-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34c27-134">Пример</span><span class="sxs-lookup"><span data-stu-id="34c27-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34c27-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="34c27-135">Request</span></span>
<span data-ttu-id="34c27-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34c27-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="34c27-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="34c27-137">Response</span></span>
<span data-ttu-id="34c27-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="34c27-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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