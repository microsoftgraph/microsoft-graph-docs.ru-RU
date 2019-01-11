---
title: Список directReports
description: Получение подчиненных пользователя. Возвращает пользователей и контакты, для которых данный пользователь назначен руководителем.
localization_priority: Normal
ms.openlocfilehash: 9a5a76b98dfd47d9a0d1d4daceeb6a93c4dc5163
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863436"
---
# <a name="list-directreports"></a><span data-ttu-id="18496-104">Список directReports</span><span class="sxs-lookup"><span data-stu-id="18496-104">List directReports</span></span>

> <span data-ttu-id="18496-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="18496-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18496-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18496-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18496-p103">Получение подчиненных пользователя. Возвращает пользователей и контакты, для которых данный пользователь назначен руководителем.</span><span class="sxs-lookup"><span data-stu-id="18496-p103">Get user's direct reports. Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="18496-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18496-109">Permissions</span></span>
<span data-ttu-id="18496-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18496-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18496-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18496-112">Permission type</span></span>      | <span data-ttu-id="18496-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18496-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18496-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18496-114">Delegated (work or school account)</span></span> | <span data-ttu-id="18496-115">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="18496-115">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="18496-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18496-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18496-117">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18496-117">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="18496-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18496-118">Application</span></span> | <span data-ttu-id="18496-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18496-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18496-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18496-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="18496-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="18496-121">Optional query parameters</span></span>
<span data-ttu-id="18496-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="18496-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="18496-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18496-123">Request headers</span></span>
| <span data-ttu-id="18496-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18496-124">Header</span></span>       | <span data-ttu-id="18496-125">Значение</span><span class="sxs-lookup"><span data-stu-id="18496-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="18496-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18496-126">Authorization</span></span>  | <span data-ttu-id="18496-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18496-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="18496-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18496-129">Content-Type</span></span>   | <span data-ttu-id="18496-130">application/json</span><span class="sxs-lookup"><span data-stu-id="18496-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18496-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="18496-131">Request body</span></span>
<span data-ttu-id="18496-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18496-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18496-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="18496-133">Response</span></span>

<span data-ttu-id="18496-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18496-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18496-135">Пример</span><span class="sxs-lookup"><span data-stu-id="18496-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18496-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="18496-136">Request</span></span>
<span data-ttu-id="18496-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18496-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/beta/me/directReports
```
##### <a name="response"></a><span data-ttu-id="18496-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="18496-138">Response</span></span>
<span data-ttu-id="18496-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="18496-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
