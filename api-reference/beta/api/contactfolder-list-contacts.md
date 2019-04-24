---
title: Список контактов
description: Получение всех контактов в почтовом ящике вошедшего пользователя (. ../ме/контактс) или из указанной папки контактов.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b3e5ee2ad13e454c0ab118b1a5b14509c9b33fbd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455704"
---
# <a name="list-contacts"></a><span data-ttu-id="0ed8d-103">Список контактов</span><span class="sxs-lookup"><span data-stu-id="0ed8d-103">List contacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ed8d-104">Получение всех контактов в почтовом ящике вошедшего пользователя (. ../ме/контактс) или из указанной папки контактов.</span><span class="sxs-lookup"><span data-stu-id="0ed8d-104">Get all the contacts in the signed-in user's mailbox (.../me/contacts), or from the specified contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ed8d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ed8d-105">Permissions</span></span>
<span data-ttu-id="0ed8d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ed8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ed8d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ed8d-108">Permission type</span></span>      | <span data-ttu-id="0ed8d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ed8d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ed8d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ed8d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ed8d-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ed8d-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0ed8d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ed8d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ed8d-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ed8d-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="0ed8d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ed8d-114">Application</span></span> | <span data-ttu-id="0ed8d-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ed8d-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ed8d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ed8d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts

GET /me/contactFolders/{id}/contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0ed8d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0ed8d-117">Optional query parameters</span></span>
<span data-ttu-id="0ed8d-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0ed8d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0ed8d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ed8d-119">Request headers</span></span>
| <span data-ttu-id="0ed8d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0ed8d-120">Name</span></span>       | <span data-ttu-id="0ed8d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0ed8d-121">Type</span></span> | <span data-ttu-id="0ed8d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0ed8d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0ed8d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ed8d-123">Authorization</span></span>  | <span data-ttu-id="0ed8d-124">string</span><span class="sxs-lookup"><span data-stu-id="0ed8d-124">string</span></span>  | <span data-ttu-id="0ed8d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ed8d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ed8d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ed8d-127">Request body</span></span>
<span data-ttu-id="0ed8d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ed8d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ed8d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ed8d-129">Response</span></span>

<span data-ttu-id="0ed8d-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contact](../resources/contact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ed8d-130">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ed8d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0ed8d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ed8d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ed8d-132">Request</span></span>
<span data-ttu-id="0ed8d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ed8d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
```
##### <a name="response"></a><span data-ttu-id="0ed8d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ed8d-134">Response</span></span>
<span data-ttu-id="0ed8d-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ed8d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-list-contacts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
