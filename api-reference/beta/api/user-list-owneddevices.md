---
title: Список ownedDevices
description: Получение списка устройств, принадлежащих пользователю.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 77a253906626c7655a85769a08fee12b8c38b6a1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968570"
---
# <a name="list-owneddevices"></a><span data-ttu-id="cdd7d-103">Список ownedDevices</span><span class="sxs-lookup"><span data-stu-id="cdd7d-103">List ownedDevices</span></span>

> <span data-ttu-id="cdd7d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cdd7d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cdd7d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdd7d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cdd7d-106">Получение списка устройств, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="cdd7d-106">Get the list of devices that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="cdd7d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cdd7d-107">Permissions</span></span>
<span data-ttu-id="cdd7d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdd7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdd7d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdd7d-110">Permission type</span></span>      | <span data-ttu-id="cdd7d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdd7d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdd7d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdd7d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cdd7d-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cdd7d-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cdd7d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdd7d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdd7d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdd7d-115">Not supported.</span></span>    |
|<span data-ttu-id="cdd7d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdd7d-116">Application</span></span> | <span data-ttu-id="cdd7d-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdd7d-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdd7d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdd7d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cdd7d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cdd7d-119">Optional query parameters</span></span>
<span data-ttu-id="cdd7d-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cdd7d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cdd7d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdd7d-121">Request headers</span></span>
| <span data-ttu-id="cdd7d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cdd7d-122">Header</span></span>       | <span data-ttu-id="cdd7d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cdd7d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cdd7d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdd7d-124">Authorization</span></span>  | <span data-ttu-id="cdd7d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdd7d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cdd7d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="cdd7d-127">Accept</span></span>  | <span data-ttu-id="cdd7d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cdd7d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdd7d-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cdd7d-129">Request body</span></span>
<span data-ttu-id="cdd7d-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cdd7d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdd7d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdd7d-131">Response</span></span>

<span data-ttu-id="cdd7d-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cdd7d-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cdd7d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cdd7d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdd7d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdd7d-134">Request</span></span>
<span data-ttu-id="cdd7d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdd7d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owneddevices"
}-->
```http
GET https://graph.microsoft.com/beta/me/ownedDevices
```
##### <a name="response"></a><span data-ttu-id="cdd7d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="cdd7d-136">Response</span></span>
<span data-ttu-id="cdd7d-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cdd7d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List ownedDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
