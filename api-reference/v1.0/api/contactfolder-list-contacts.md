---
title: Список контактов
description: Получение коллекции контактов из папки контактов по умолчанию для вошедшего пользователя (`.../me/contacts`) или из указанной папки контактов.
ms.openlocfilehash: f70ea5000a5d0228f49b8bfa6179a97cb5899c3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026077"
---
# <a name="list-contacts"></a><span data-ttu-id="f6932-103">Список контактов</span><span class="sxs-lookup"><span data-stu-id="f6932-103">List contacts</span></span>

<span data-ttu-id="f6932-104">Получение коллекции контактов из папки контактов по умолчанию для вошедшего пользователя (`.../me/contacts`) или из указанной папки контактов.</span><span class="sxs-lookup"><span data-stu-id="f6932-104">Get a contact collection from the default Contacts folder of the signed-in user (`.../me/contacts`), or from the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="f6932-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6932-105">Permissions</span></span>
<span data-ttu-id="f6932-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6932-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6932-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6932-108">Permission type</span></span>      | <span data-ttu-id="f6932-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6932-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6932-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6932-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f6932-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6932-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f6932-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6932-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6932-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6932-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f6932-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6932-114">Application</span></span> | <span data-ttu-id="f6932-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6932-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6932-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6932-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f6932-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6932-117">Optional query parameters</span></span>
<span data-ttu-id="f6932-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f6932-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f6932-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6932-119">Request headers</span></span>
| <span data-ttu-id="f6932-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f6932-120">Name</span></span>       | <span data-ttu-id="f6932-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f6932-121">Type</span></span> | <span data-ttu-id="f6932-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f6932-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f6932-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6932-123">Authorization</span></span>  | <span data-ttu-id="f6932-124">string</span><span class="sxs-lookup"><span data-stu-id="f6932-124">string</span></span>  | <span data-ttu-id="f6932-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6932-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6932-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f6932-127">Request body</span></span>
<span data-ttu-id="f6932-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6932-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6932-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6932-129">Response</span></span>

<span data-ttu-id="f6932-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6932-130">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f6932-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f6932-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6932-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6932-132">Request</span></span>
<span data-ttu-id="f6932-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6932-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="f6932-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6932-134">Response</span></span>
<span data-ttu-id="f6932-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f6932-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "birthday": "datetime-value",
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
