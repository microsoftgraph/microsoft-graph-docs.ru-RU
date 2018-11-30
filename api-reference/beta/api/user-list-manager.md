---
title: Получение руководителя
description: Получение руководителя пользователя. Возвращает пользователя или контакт, назначенный руководителем пользователя.
ms.openlocfilehash: 3601b7c13eb97b288cc65e927432bd420105970a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077462"
---
# <a name="list-manager"></a><span data-ttu-id="a38cf-104">Получение руководителя</span><span class="sxs-lookup"><span data-stu-id="a38cf-104">List manager</span></span>

> <span data-ttu-id="a38cf-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a38cf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a38cf-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a38cf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a38cf-p103">Получение руководителя пользователя. Возвращает пользователя или контакт, назначенный руководителем пользователя.</span><span class="sxs-lookup"><span data-stu-id="a38cf-p103">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="a38cf-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a38cf-109">Permissions</span></span>
<span data-ttu-id="a38cf-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a38cf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a38cf-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a38cf-112">Permission type</span></span>      | <span data-ttu-id="a38cf-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a38cf-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a38cf-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a38cf-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a38cf-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a38cf-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a38cf-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a38cf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a38cf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a38cf-117">Not supported.</span></span>    |
|<span data-ttu-id="a38cf-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a38cf-118">Application</span></span> | <span data-ttu-id="a38cf-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a38cf-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a38cf-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a38cf-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a38cf-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a38cf-121">Optional query parameters</span></span>
<span data-ttu-id="a38cf-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a38cf-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a38cf-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a38cf-123">Request headers</span></span>
| <span data-ttu-id="a38cf-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a38cf-124">Header</span></span>       | <span data-ttu-id="a38cf-125">Значение</span><span class="sxs-lookup"><span data-stu-id="a38cf-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="a38cf-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a38cf-126">Authorization</span></span>  | <span data-ttu-id="a38cf-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a38cf-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a38cf-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a38cf-129">Content-Type</span></span>   | <span data-ttu-id="a38cf-130">application/json</span><span class="sxs-lookup"><span data-stu-id="a38cf-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a38cf-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a38cf-131">Request body</span></span>
<span data-ttu-id="a38cf-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a38cf-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a38cf-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a38cf-133">Response</span></span>

<span data-ttu-id="a38cf-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a38cf-134">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a38cf-135">Пример</span><span class="sxs-lookup"><span data-stu-id="a38cf-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a38cf-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a38cf-136">Request</span></span>
<span data-ttu-id="a38cf-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a38cf-137">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="a38cf-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="a38cf-138">Response</span></span>
<span data-ttu-id="a38cf-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a38cf-139">Here is an example of the response.</span></span>
<!-- { "blockType": "ignored" } -->
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
