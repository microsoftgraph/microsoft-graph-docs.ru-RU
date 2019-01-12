---
title: Список registeredUsers
description: Получение списка пользователей, являющихся зарегистрированными пользователями устройства.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 14b7c3b31d2edfde093a0c5d8cd1ed48a25ba1cd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954220"
---
# <a name="list-registeredusers"></a><span data-ttu-id="1d503-103">Список registeredUsers</span><span class="sxs-lookup"><span data-stu-id="1d503-103">List registeredUsers</span></span>

<span data-ttu-id="1d503-104">Получение списка пользователей, являющихся зарегистрированными пользователями устройства.</span><span class="sxs-lookup"><span data-stu-id="1d503-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="1d503-105">В случае зарегистрированных личных устройств или устройств, присоединенных через облако, при регистрации для обычных пользователей задается то же значение, что и для владельцев.</span><span class="sxs-lookup"><span data-stu-id="1d503-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d503-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d503-106">Permissions</span></span>
<span data-ttu-id="1d503-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d503-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1d503-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d503-109">Permission type</span></span>      | <span data-ttu-id="1d503-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d503-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d503-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d503-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1d503-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1d503-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1d503-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d503-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d503-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d503-114">Not supported.</span></span>    |
|<span data-ttu-id="1d503-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1d503-115">Application</span></span> | <span data-ttu-id="1d503-116">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d503-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d503-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d503-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1d503-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1d503-118">Optional query parameters</span></span>
<span data-ttu-id="1d503-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1d503-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1d503-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d503-120">Request headers</span></span>
| <span data-ttu-id="1d503-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1d503-121">Name</span></span>       | <span data-ttu-id="1d503-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1d503-122">Type</span></span> | <span data-ttu-id="1d503-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1d503-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1d503-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d503-124">Authorization</span></span>  | <span data-ttu-id="1d503-125">string</span><span class="sxs-lookup"><span data-stu-id="1d503-125">string</span></span>  | <span data-ttu-id="1d503-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d503-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d503-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d503-128">Request body</span></span>
<span data-ttu-id="1d503-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1d503-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d503-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d503-130">Response</span></span>

<span data-ttu-id="1d503-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1d503-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1d503-132">Пример</span><span class="sxs-lookup"><span data-stu-id="1d503-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1d503-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d503-133">Request</span></span>
<span data-ttu-id="1d503-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d503-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="1d503-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d503-135">Response</span></span>
<span data-ttu-id="1d503-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1d503-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
