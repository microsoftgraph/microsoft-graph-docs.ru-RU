---
title: Перечисление пользователей
description: Получение списка объектов user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 00cf39a3e50c6c9911471f60a1cc7def1ee4563b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544199"
---
# <a name="list-users"></a><span data-ttu-id="0eb52-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="0eb52-103">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0eb52-104">Получение списка объектов user.</span><span class="sxs-lookup"><span data-stu-id="0eb52-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0eb52-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0eb52-105">Permissions</span></span>

<span data-ttu-id="0eb52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0eb52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0eb52-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0eb52-108">Permission type</span></span>      | <span data-ttu-id="0eb52-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0eb52-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0eb52-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0eb52-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0eb52-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0eb52-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0eb52-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0eb52-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0eb52-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0eb52-113">Not supported.</span></span>    |
|<span data-ttu-id="0eb52-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0eb52-114">Application</span></span> | <span data-ttu-id="0eb52-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eb52-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0eb52-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0eb52-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0eb52-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0eb52-117">Optional query parameters</span></span>

<span data-ttu-id="0eb52-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0eb52-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0eb52-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0eb52-119">Request headers</span></span>
| <span data-ttu-id="0eb52-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0eb52-120">Header</span></span>        | <span data-ttu-id="0eb52-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0eb52-121">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="0eb52-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0eb52-122">Authorization</span></span> | <span data-ttu-id="0eb52-123">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="0eb52-123">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="0eb52-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0eb52-124">Content-Type</span></span>  | <span data-ttu-id="0eb52-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0eb52-125">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="0eb52-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0eb52-126">Request body</span></span>

<span data-ttu-id="0eb52-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0eb52-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0eb52-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eb52-128">Response</span></span>

<span data-ttu-id="0eb52-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0eb52-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0eb52-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0eb52-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0eb52-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0eb52-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/users
```

##### <a name="response"></a><span data-ttu-id="0eb52-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0eb52-132">Response</span></span>

<span data-ttu-id="0eb52-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0eb52-133">Here is an example of the response.</span></span> <span data-ttu-id="0eb52-134">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="0eb52-134">Note: The response object shown here may be truncated for brevity.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
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
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
