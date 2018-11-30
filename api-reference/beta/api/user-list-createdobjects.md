---
title: Список createdObjects
description: Получение списка созданных пользователем объектов каталога.
ms.openlocfilehash: 030de28bdd402720f2b5c62e9b276a080583f687
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078816"
---
# <a name="list-createdobjects"></a><span data-ttu-id="7aac0-103">Список createdObjects</span><span class="sxs-lookup"><span data-stu-id="7aac0-103">List createdObjects</span></span>

> <span data-ttu-id="7aac0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7aac0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7aac0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7aac0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7aac0-106">Получение списка созданных пользователем объектов каталога.</span><span class="sxs-lookup"><span data-stu-id="7aac0-106">Get a list of directory objects that were created by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="7aac0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7aac0-107">Permissions</span></span>
<span data-ttu-id="7aac0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aac0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aac0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7aac0-110">Permission type</span></span>      | <span data-ttu-id="7aac0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7aac0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7aac0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7aac0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7aac0-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7aac0-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7aac0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7aac0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aac0-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7aac0-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="7aac0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7aac0-116">Application</span></span> | <span data-ttu-id="7aac0-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aac0-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7aac0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7aac0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7aac0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7aac0-119">Optional query parameters</span></span>
<span data-ttu-id="7aac0-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7aac0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7aac0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7aac0-121">Request headers</span></span>
| <span data-ttu-id="7aac0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7aac0-122">Header</span></span>       | <span data-ttu-id="7aac0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7aac0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7aac0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7aac0-124">Authorization</span></span>  | <span data-ttu-id="7aac0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7aac0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7aac0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7aac0-127">Content-Type</span></span>  | <span data-ttu-id="7aac0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7aac0-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7aac0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7aac0-129">Request body</span></span>
<span data-ttu-id="7aac0-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7aac0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7aac0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7aac0-131">Response</span></span>

<span data-ttu-id="7aac0-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7aac0-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7aac0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7aac0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7aac0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7aac0-134">Request</span></span>
<span data-ttu-id="7aac0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7aac0-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```http
GET https://graph.microsoft.com/beta/me/createdObjects
```
##### <a name="response"></a><span data-ttu-id="7aac0-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7aac0-136">Response</span></span>
<span data-ttu-id="7aac0-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="7aac0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->