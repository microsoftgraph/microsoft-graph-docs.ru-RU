---
title: Создание объекта Contact
description: Добавление контакта в корневую папку контактов или в конечную точку `contacts` другой папки контактов.
ms.openlocfilehash: a770569f15676317479571afb1dbe46268c926d7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075964"
---
# <a name="create-contact"></a><span data-ttu-id="cf7a7-103">Создание объекта Contact</span><span class="sxs-lookup"><span data-stu-id="cf7a7-103">Create Contact</span></span>

> <span data-ttu-id="cf7a7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cf7a7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf7a7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf7a7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cf7a7-106">Добавление контакта в корневую папку с контактами или конечную точку `contacts` другой папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="cf7a7-106">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="cf7a7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf7a7-107">Permissions</span></span>
<span data-ttu-id="cf7a7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf7a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf7a7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf7a7-110">Permission type</span></span>      | <span data-ttu-id="cf7a7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf7a7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf7a7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf7a7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cf7a7-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf7a7-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cf7a7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf7a7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf7a7-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf7a7-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cf7a7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf7a7-116">Application</span></span> | <span data-ttu-id="cf7a7-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cf7a7-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf7a7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf7a7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="cf7a7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf7a7-119">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="cf7a7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf7a7-120">Request headers</span></span>
| <span data-ttu-id="cf7a7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf7a7-121">Header</span></span>       | <span data-ttu-id="cf7a7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cf7a7-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cf7a7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf7a7-123">Authorization</span></span>  | <span data-ttu-id="cf7a7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf7a7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cf7a7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cf7a7-126">Content-Type</span></span>  | <span data-ttu-id="cf7a7-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf7a7-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf7a7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf7a7-129">Request body</span></span>
<span data-ttu-id="cf7a7-130">Предоставьте в тексте запроса описание объекта [Contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf7a7-130">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cf7a7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf7a7-131">Response</span></span>

<span data-ttu-id="cf7a7-132">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cf7a7-132">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf7a7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cf7a7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf7a7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf7a7-134">Request</span></span>
<span data-ttu-id="cf7a7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf7a7-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
<span data-ttu-id="cf7a7-136">Предоставьте в тексте запроса описание объекта [contact](../resources/contact.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf7a7-136">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cf7a7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf7a7-137">Response</span></span>
<span data-ttu-id="cf7a7-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cf7a7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->