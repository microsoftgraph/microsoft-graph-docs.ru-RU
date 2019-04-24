---
title: Список createdObjects
description: Получение списка созданных пользователем объектов каталога.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 33b3f7ded23a7bd72274dff159a824acb03e6bb5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522596"
---
# <a name="list-createdobjects"></a><span data-ttu-id="2201d-103">Список createdObjects</span><span class="sxs-lookup"><span data-stu-id="2201d-103">List createdObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2201d-104">Получение списка созданных пользователем объектов каталога.</span><span class="sxs-lookup"><span data-stu-id="2201d-104">Get a list of directory objects that were created by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="2201d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2201d-105">Permissions</span></span>
<span data-ttu-id="2201d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2201d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2201d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2201d-108">Permission type</span></span>      | <span data-ttu-id="2201d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2201d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2201d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2201d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2201d-111">User. Read, User. ReadWrite, User. Read. ALL, User. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="2201d-111">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2201d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2201d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2201d-113">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2201d-113">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="2201d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2201d-114">Application</span></span> | <span data-ttu-id="2201d-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2201d-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2201d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2201d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2201d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2201d-117">Optional query parameters</span></span>
<span data-ttu-id="2201d-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2201d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2201d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2201d-119">Request headers</span></span>
| <span data-ttu-id="2201d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2201d-120">Header</span></span>       | <span data-ttu-id="2201d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2201d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2201d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2201d-122">Authorization</span></span>  | <span data-ttu-id="2201d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2201d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2201d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2201d-125">Content-Type</span></span>  | <span data-ttu-id="2201d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2201d-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2201d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2201d-127">Request body</span></span>
<span data-ttu-id="2201d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2201d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2201d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2201d-129">Response</span></span>

<span data-ttu-id="2201d-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2201d-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2201d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2201d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2201d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2201d-132">Request</span></span>
<span data-ttu-id="2201d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2201d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```http
GET https://graph.microsoft.com/beta/me/createdObjects
```
##### <a name="response"></a><span data-ttu-id="2201d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2201d-134">Response</span></span>
<span data-ttu-id="2201d-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2201d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
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
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-createdobjects.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
