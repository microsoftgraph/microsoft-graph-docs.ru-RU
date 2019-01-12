---
title: Получение руководителя
description: Получение руководителя пользователя. Возвращает пользователя или контакт, назначенный руководителем пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3818d72ea024ff06697f123d9a1fb5b3d534152d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933775"
---
# <a name="list-manager"></a><span data-ttu-id="97dd7-104">Получение руководителя</span><span class="sxs-lookup"><span data-stu-id="97dd7-104">List manager</span></span>

> <span data-ttu-id="97dd7-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="97dd7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97dd7-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97dd7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97dd7-p103">Получение руководителя пользователя. Возвращает пользователя или контакт, назначенный руководителем пользователя.</span><span class="sxs-lookup"><span data-stu-id="97dd7-p103">Get user's manager. Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="97dd7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97dd7-109">Permissions</span></span>
<span data-ttu-id="97dd7-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97dd7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97dd7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97dd7-112">Permission type</span></span>      | <span data-ttu-id="97dd7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97dd7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97dd7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97dd7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="97dd7-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="97dd7-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="97dd7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97dd7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97dd7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97dd7-117">Not supported.</span></span>    |
|<span data-ttu-id="97dd7-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97dd7-118">Application</span></span> | <span data-ttu-id="97dd7-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97dd7-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97dd7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97dd7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="97dd7-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="97dd7-121">Optional query parameters</span></span>
<span data-ttu-id="97dd7-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="97dd7-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="97dd7-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97dd7-123">Request headers</span></span>
| <span data-ttu-id="97dd7-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97dd7-124">Header</span></span>       | <span data-ttu-id="97dd7-125">Значение</span><span class="sxs-lookup"><span data-stu-id="97dd7-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="97dd7-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97dd7-126">Authorization</span></span>  | <span data-ttu-id="97dd7-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97dd7-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="97dd7-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97dd7-129">Content-Type</span></span>   | <span data-ttu-id="97dd7-130">application/json</span><span class="sxs-lookup"><span data-stu-id="97dd7-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97dd7-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="97dd7-131">Request body</span></span>
<span data-ttu-id="97dd7-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97dd7-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97dd7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="97dd7-133">Response</span></span>

<span data-ttu-id="97dd7-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="97dd7-134">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97dd7-135">Пример</span><span class="sxs-lookup"><span data-stu-id="97dd7-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97dd7-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="97dd7-136">Request</span></span>
<span data-ttu-id="97dd7-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97dd7-137">Here is an example of the request.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="97dd7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="97dd7-138">Response</span></span>
<span data-ttu-id="97dd7-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="97dd7-139">Here is an example of the response.</span></span>
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
