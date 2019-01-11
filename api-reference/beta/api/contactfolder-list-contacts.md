---
title: Список контактов
description: Получение всех контактов в почтовом ящике пользователь выполнил вход (.../me/contacts) или из указанной папки "Контакты".
localization_priority: Normal
ms.openlocfilehash: 304efe55a39d685ef5ce58281bfb407a43657a92
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892367"
---
# <a name="list-contacts"></a><span data-ttu-id="6523a-103">Список контактов</span><span class="sxs-lookup"><span data-stu-id="6523a-103">List contacts</span></span>

> <span data-ttu-id="6523a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6523a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6523a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6523a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6523a-106">Получение всех контактов в почтовом ящике пользователь выполнил вход (.../me/contacts) или из указанной папки "Контакты".</span><span class="sxs-lookup"><span data-stu-id="6523a-106">Get all the contacts in the signed-in user's mailbox (.../me/contacts), or from the specified contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="6523a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6523a-107">Permissions</span></span>
<span data-ttu-id="6523a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6523a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6523a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6523a-110">Permission type</span></span>      | <span data-ttu-id="6523a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6523a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6523a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6523a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6523a-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6523a-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6523a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6523a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6523a-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6523a-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6523a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6523a-116">Application</span></span> | <span data-ttu-id="6523a-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6523a-117">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6523a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6523a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6523a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6523a-119">Optional query parameters</span></span>
<span data-ttu-id="6523a-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6523a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6523a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6523a-121">Request headers</span></span>
| <span data-ttu-id="6523a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6523a-122">Name</span></span>       | <span data-ttu-id="6523a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="6523a-123">Type</span></span> | <span data-ttu-id="6523a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6523a-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6523a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6523a-125">Authorization</span></span>  | <span data-ttu-id="6523a-126">string</span><span class="sxs-lookup"><span data-stu-id="6523a-126">string</span></span>  | <span data-ttu-id="6523a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6523a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6523a-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6523a-129">Request body</span></span>
<span data-ttu-id="6523a-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6523a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6523a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6523a-131">Response</span></span>

<span data-ttu-id="6523a-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6523a-132">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6523a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6523a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6523a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6523a-134">Request</span></span>
<span data-ttu-id="6523a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6523a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="6523a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="6523a-136">Response</span></span>
<span data-ttu-id="6523a-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6523a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "2016-10-19T10:37:00Z",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
