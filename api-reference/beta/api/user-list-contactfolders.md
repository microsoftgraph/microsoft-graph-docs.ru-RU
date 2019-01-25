---
title: Список объектов contactFolder
description: Получение всех контактов папок в почтовом ящике пользователь выполнил вход.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f5f0a485c3c134b6627fce5d3b8f04c26dee503e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523283"
---
# <a name="list-contactfolders"></a><span data-ttu-id="541d5-103">Список объектов contactFolder</span><span class="sxs-lookup"><span data-stu-id="541d5-103">List contactFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="541d5-104">Получение всех контактов папок в почтовом ящике пользователь выполнил вход.</span><span class="sxs-lookup"><span data-stu-id="541d5-104">Get all the contact folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="541d5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="541d5-105">Permissions</span></span>
<span data-ttu-id="541d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="541d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="541d5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="541d5-108">Permission type</span></span>      | <span data-ttu-id="541d5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="541d5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="541d5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="541d5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="541d5-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="541d5-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="541d5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="541d5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="541d5-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="541d5-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="541d5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="541d5-114">Application</span></span> | <span data-ttu-id="541d5-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="541d5-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="541d5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="541d5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="541d5-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="541d5-117">Optional query parameters</span></span>
<span data-ttu-id="541d5-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="541d5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="541d5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="541d5-119">Request headers</span></span>
| <span data-ttu-id="541d5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="541d5-120">Header</span></span>       | <span data-ttu-id="541d5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="541d5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="541d5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="541d5-122">Authorization</span></span>  | <span data-ttu-id="541d5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="541d5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="541d5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="541d5-125">Content-Type</span></span>   | <span data-ttu-id="541d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="541d5-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="541d5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="541d5-127">Request body</span></span>
<span data-ttu-id="541d5-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="541d5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="541d5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="541d5-129">Response</span></span>

<span data-ttu-id="541d5-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="541d5-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="541d5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="541d5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="541d5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="541d5-132">Request</span></span>
<span data-ttu-id="541d5-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="541d5-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders
```
##### <a name="response"></a><span data-ttu-id="541d5-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="541d5-134">Response</span></span>
<span data-ttu-id="541d5-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="541d5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "wellKnownName": "wellKnownName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-contactfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
