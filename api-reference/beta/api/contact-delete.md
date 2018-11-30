---
title: Удаление контакта
description: Удаление контакта.
ms.openlocfilehash: fec4ec30430114f023577043b0351683fc25189e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076238"
---
# <a name="delete-contact"></a><span data-ttu-id="6731d-103">Удаление контакта</span><span class="sxs-lookup"><span data-stu-id="6731d-103">Delete contact</span></span>

> <span data-ttu-id="6731d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6731d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6731d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6731d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6731d-106">Удаление контакта.</span><span class="sxs-lookup"><span data-stu-id="6731d-106">Delete contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="6731d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6731d-107">Permissions</span></span>
<span data-ttu-id="6731d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6731d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6731d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6731d-110">Permission type</span></span>      | <span data-ttu-id="6731d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6731d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6731d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6731d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6731d-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6731d-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6731d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6731d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6731d-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6731d-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6731d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6731d-116">Application</span></span> | <span data-ttu-id="6731d-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6731d-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6731d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6731d-118">HTTP request</span></span>
<span data-ttu-id="6731d-119"><!-- { "blockType": "ignored" } -->[Обратитесь](../resources/contact.md) в пользователя по умолчанию [contactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="6731d-119"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="6731d-120">Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="6731d-120">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="6731d-121">[Обратитесь](../resources/contact.md) в дочерней папкой [contactFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="6731d-121">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="6731d-122">В приведенном ниже примере показана один уровень вложения, но контакт может быть найдена в дочерних дочернего и т. д.</span><span class="sxs-lookup"><span data-stu-id="6731d-122">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6731d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6731d-123">Request headers</span></span>
| <span data-ttu-id="6731d-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6731d-124">Header</span></span>       | <span data-ttu-id="6731d-125">Значение</span><span class="sxs-lookup"><span data-stu-id="6731d-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6731d-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6731d-126">Authorization</span></span>  | <span data-ttu-id="6731d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6731d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6731d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6731d-129">Request body</span></span>
<span data-ttu-id="6731d-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6731d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6731d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6731d-131">Response</span></span>

<span data-ttu-id="6731d-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6731d-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6731d-134">Пример</span><span class="sxs-lookup"><span data-stu-id="6731d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6731d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="6731d-135">Request</span></span>
<span data-ttu-id="6731d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6731d-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="6731d-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="6731d-137">Response</span></span>
<span data-ttu-id="6731d-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6731d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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