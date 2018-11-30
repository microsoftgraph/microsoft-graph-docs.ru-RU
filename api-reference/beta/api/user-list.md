---
title: Список пользователей
description: Получение списка объектов user.
ms.openlocfilehash: 13c9b2847e7acc1999f3ab23fadfea371036caf3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081257"
---
# <a name="list-users"></a><span data-ttu-id="d7a11-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="d7a11-103">List users</span></span>

> <span data-ttu-id="d7a11-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d7a11-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7a11-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7a11-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7a11-106">Получение списка объектов user.</span><span class="sxs-lookup"><span data-stu-id="d7a11-106">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7a11-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7a11-107">Permissions</span></span>

<span data-ttu-id="d7a11-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7a11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7a11-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7a11-110">Permission type</span></span>      | <span data-ttu-id="d7a11-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7a11-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7a11-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7a11-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d7a11-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d7a11-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d7a11-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7a11-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7a11-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7a11-115">Not supported.</span></span>    |
|<span data-ttu-id="d7a11-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7a11-116">Application</span></span> | <span data-ttu-id="d7a11-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7a11-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7a11-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7a11-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d7a11-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d7a11-119">Optional query parameters</span></span>

<span data-ttu-id="d7a11-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d7a11-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7a11-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7a11-121">Request headers</span></span>
| <span data-ttu-id="d7a11-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7a11-122">Header</span></span>        | <span data-ttu-id="d7a11-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d7a11-123">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="d7a11-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7a11-124">Authorization</span></span> | <span data-ttu-id="d7a11-125">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="d7a11-125">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="d7a11-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7a11-126">Content-Type</span></span>  | <span data-ttu-id="d7a11-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d7a11-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="d7a11-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7a11-128">Request body</span></span>

<span data-ttu-id="d7a11-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7a11-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7a11-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7a11-130">Response</span></span>

<span data-ttu-id="d7a11-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d7a11-131">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7a11-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d7a11-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d7a11-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7a11-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/users
```

##### <a name="response"></a><span data-ttu-id="d7a11-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7a11-134">Response</span></span>

<span data-ttu-id="d7a11-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d7a11-135">Here is an example of the response.</span></span> <span data-ttu-id="d7a11-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="d7a11-136">Note: The response object shown here may be truncated for brevity.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
