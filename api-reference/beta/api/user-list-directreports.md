---
title: Список directReports
description: Получение подчиненных пользователя. Возвращает пользователей и контакты, для которых данный пользователь назначен руководителем.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d56b8dc4579f40156e30a46b00af0f5bfcd82b97
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520349"
---
# <a name="list-directreports"></a><span data-ttu-id="dfa4f-104">Список directReports</span><span class="sxs-lookup"><span data-stu-id="dfa4f-104">List directReports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfa4f-p102">Получение подчиненных пользователя. Возвращает пользователей и контакты, для которых данный пользователь назначен руководителем.</span><span class="sxs-lookup"><span data-stu-id="dfa4f-p102">Get user's direct reports. Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="dfa4f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfa4f-107">Permissions</span></span>
<span data-ttu-id="dfa4f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfa4f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfa4f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfa4f-110">Permission type</span></span>      | <span data-ttu-id="dfa4f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfa4f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfa4f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfa4f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dfa4f-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dfa4f-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dfa4f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfa4f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfa4f-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfa4f-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="dfa4f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfa4f-116">Application</span></span> | <span data-ttu-id="dfa4f-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfa4f-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfa4f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfa4f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dfa4f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dfa4f-119">Optional query parameters</span></span>
<span data-ttu-id="dfa4f-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dfa4f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dfa4f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfa4f-121">Request headers</span></span>
| <span data-ttu-id="dfa4f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dfa4f-122">Header</span></span>       | <span data-ttu-id="dfa4f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="dfa4f-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="dfa4f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfa4f-124">Authorization</span></span>  | <span data-ttu-id="dfa4f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfa4f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="dfa4f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dfa4f-127">Content-Type</span></span>   | <span data-ttu-id="dfa4f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dfa4f-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dfa4f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dfa4f-129">Request body</span></span>
<span data-ttu-id="dfa4f-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dfa4f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfa4f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfa4f-131">Response</span></span>

<span data-ttu-id="dfa4f-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dfa4f-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dfa4f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="dfa4f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dfa4f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfa4f-134">Request</span></span>
<span data-ttu-id="dfa4f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfa4f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/beta/me/directReports
```
##### <a name="response"></a><span data-ttu-id="dfa4f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="dfa4f-136">Response</span></span>
<span data-ttu-id="dfa4f-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="dfa4f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-directreports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
