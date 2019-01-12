---
title: Список ownedDevices
description: Получение списка устройств, принадлежащих пользователю.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 275e2869763e8cc25728e24c8046506891d2005f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947458"
---
# <a name="list-owneddevices"></a><span data-ttu-id="bca8d-103">Список ownedDevices</span><span class="sxs-lookup"><span data-stu-id="bca8d-103">List ownedDevices</span></span>

<span data-ttu-id="bca8d-104">Получение списка устройств, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="bca8d-104">Get the list of devices that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="bca8d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bca8d-105">Permissions</span></span>
<span data-ttu-id="bca8d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bca8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bca8d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bca8d-108">Permission type</span></span>      | <span data-ttu-id="bca8d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bca8d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bca8d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bca8d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bca8d-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bca8d-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bca8d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bca8d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bca8d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bca8d-113">Not supported.</span></span>    |
|<span data-ttu-id="bca8d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bca8d-114">Application</span></span> | <span data-ttu-id="bca8d-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bca8d-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bca8d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bca8d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bca8d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bca8d-117">Optional query parameters</span></span>
<span data-ttu-id="bca8d-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bca8d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bca8d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bca8d-119">Request headers</span></span>
| <span data-ttu-id="bca8d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bca8d-120">Header</span></span>       | <span data-ttu-id="bca8d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bca8d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bca8d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bca8d-122">Authorization</span></span>  | <span data-ttu-id="bca8d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bca8d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bca8d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bca8d-125">Accept</span></span>  | <span data-ttu-id="bca8d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bca8d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bca8d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bca8d-127">Request body</span></span>
<span data-ttu-id="bca8d-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bca8d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bca8d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bca8d-129">Response</span></span>

<span data-ttu-id="bca8d-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bca8d-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bca8d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bca8d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bca8d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bca8d-132">Request</span></span>
<span data-ttu-id="bca8d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bca8d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owneddevices"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/ownedDevices
```
##### <a name="response"></a><span data-ttu-id="bca8d-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="bca8d-134">Response</span></span>
<span data-ttu-id="bca8d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bca8d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
