---
title: Получение руководителя
description: Получение руководителя пользователя. Возвращает пользователя или контакт, назначенный руководителем пользователя.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ae243f0fa4c8212cecebedc39ebfc2d5713d5689
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980568"
---
# <a name="list-manager"></a><span data-ttu-id="2f948-104">Получение руководителя</span><span class="sxs-lookup"><span data-stu-id="2f948-104">List manager</span></span>

<span data-ttu-id="2f948-p102">Получение руководителя пользователя. Возвращает пользователя или контакт, назначенный руководителем пользователя.</span><span class="sxs-lookup"><span data-stu-id="2f948-p102">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="2f948-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f948-107">Permissions</span></span>
<span data-ttu-id="2f948-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f948-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f948-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f948-110">Permission type</span></span>      | <span data-ttu-id="2f948-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f948-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f948-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f948-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2f948-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2f948-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2f948-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f948-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f948-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f948-115">Not supported.</span></span>    |
|<span data-ttu-id="2f948-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f948-116">Application</span></span> | <span data-ttu-id="2f948-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f948-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f948-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f948-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2f948-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2f948-119">Optional query parameters</span></span>
<span data-ttu-id="2f948-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2f948-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2f948-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f948-121">Request headers</span></span>
| <span data-ttu-id="2f948-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f948-122">Header</span></span>       | <span data-ttu-id="2f948-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2f948-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="2f948-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f948-124">Authorization</span></span>  | <span data-ttu-id="2f948-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f948-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2f948-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f948-127">Content-Type</span></span>   | <span data-ttu-id="2f948-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2f948-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f948-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2f948-129">Request body</span></span>
<span data-ttu-id="2f948-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f948-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f948-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f948-131">Response</span></span>

<span data-ttu-id="2f948-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f948-132">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2f948-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2f948-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f948-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f948-134">Request</span></span>
<span data-ttu-id="2f948-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f948-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="2f948-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f948-136">Response</span></span>
<span data-ttu-id="2f948-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2f948-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
