---
title: Список registeredDevices
description: Получение списка зарегистрированных устройств пользователя.
localization_priority: Normal
ms.openlocfilehash: 2447a58e89fe6c94ab5b3cf6d23b2621f757709c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866369"
---
# <a name="list-registereddevices"></a><span data-ttu-id="f0570-103">Список registeredDevices</span><span class="sxs-lookup"><span data-stu-id="f0570-103">List registeredDevices</span></span>

> <span data-ttu-id="f0570-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f0570-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0570-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0570-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0570-106">Получение списка зарегистрированных устройств пользователя.</span><span class="sxs-lookup"><span data-stu-id="f0570-106">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="f0570-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0570-107">Permissions</span></span>
<span data-ttu-id="f0570-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0570-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0570-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0570-110">Permission type</span></span>      | <span data-ttu-id="f0570-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0570-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0570-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0570-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f0570-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f0570-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f0570-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0570-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0570-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0570-115">Not supported.</span></span>    |
|<span data-ttu-id="f0570-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0570-116">Application</span></span> | <span data-ttu-id="f0570-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0570-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0570-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0570-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f0570-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f0570-119">Optional query parameters</span></span>
<span data-ttu-id="f0570-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f0570-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f0570-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0570-121">Request headers</span></span>
| <span data-ttu-id="f0570-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0570-122">Header</span></span>       | <span data-ttu-id="f0570-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f0570-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f0570-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0570-124">Authorization</span></span>  | <span data-ttu-id="f0570-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0570-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f0570-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f0570-127">Accept</span></span>  | <span data-ttu-id="f0570-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f0570-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0570-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f0570-129">Request body</span></span>
<span data-ttu-id="f0570-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0570-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0570-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0570-131">Response</span></span>

<span data-ttu-id="f0570-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0570-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0570-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f0570-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0570-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0570-134">Request</span></span>
<span data-ttu-id="f0570-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0570-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```http
GET https://graph.microsoft.com/beta/me/registeredDevices
```
##### <a name="response"></a><span data-ttu-id="f0570-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0570-136">Response</span></span>
<span data-ttu-id="f0570-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f0570-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
