---
title: Список объектов contactFolder
description: Получение всех папок контактов в почтовом ящике вошедшего пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4aca24e167f1d9f1bfe3529e44665347a5e1cdbd
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869269"
---
# <a name="list-contactfolders"></a><span data-ttu-id="639cc-103">Список объектов contactFolder</span><span class="sxs-lookup"><span data-stu-id="639cc-103">List contactFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="639cc-104">Получение всех папок контактов в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="639cc-104">Get all the contact folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="639cc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="639cc-105">Permissions</span></span>
<span data-ttu-id="639cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="639cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="639cc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="639cc-108">Permission type</span></span>      | <span data-ttu-id="639cc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="639cc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="639cc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="639cc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="639cc-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="639cc-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="639cc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="639cc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="639cc-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="639cc-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="639cc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="639cc-114">Application</span></span> | <span data-ttu-id="639cc-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="639cc-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="639cc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="639cc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="639cc-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="639cc-117">Optional query parameters</span></span>
<span data-ttu-id="639cc-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="639cc-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="639cc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="639cc-119">Request headers</span></span>
| <span data-ttu-id="639cc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="639cc-120">Header</span></span>       | <span data-ttu-id="639cc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="639cc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="639cc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="639cc-122">Authorization</span></span>  | <span data-ttu-id="639cc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="639cc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="639cc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="639cc-125">Content-Type</span></span>   | <span data-ttu-id="639cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="639cc-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="639cc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="639cc-127">Request body</span></span>
<span data-ttu-id="639cc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="639cc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="639cc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="639cc-129">Response</span></span>

<span data-ttu-id="639cc-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="639cc-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="639cc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="639cc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="639cc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="639cc-132">Request</span></span>
<span data-ttu-id="639cc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="639cc-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders
```
##### <a name="response"></a><span data-ttu-id="639cc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="639cc-134">Response</span></span>
<span data-ttu-id="639cc-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="639cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
