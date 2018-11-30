---
title: Список registeredUsers
description: Получение списка пользователей, являющихся зарегистрированными пользователями устройства.
ms.openlocfilehash: 370990b5b9c61b071620fe0df04fd38e98892bd1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027638"
---
# <a name="list-registeredusers"></a><span data-ttu-id="9243d-103">Список registeredUsers</span><span class="sxs-lookup"><span data-stu-id="9243d-103">List registeredUsers</span></span>

<span data-ttu-id="9243d-104">Получение списка пользователей, являющихся зарегистрированными пользователями устройства.</span><span class="sxs-lookup"><span data-stu-id="9243d-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="9243d-105">В случае зарегистрированных личных устройств или устройств, присоединенных через облако, при регистрации для обычных пользователей задается то же значение, что и для владельцев.</span><span class="sxs-lookup"><span data-stu-id="9243d-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="9243d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9243d-106">Permissions</span></span>
<span data-ttu-id="9243d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9243d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9243d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9243d-109">Permission type</span></span>      | <span data-ttu-id="9243d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9243d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9243d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9243d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9243d-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9243d-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9243d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9243d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9243d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9243d-114">Not supported.</span></span>    |
|<span data-ttu-id="9243d-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="9243d-115">Application</span></span> | <span data-ttu-id="9243d-116">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9243d-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9243d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9243d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9243d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9243d-118">Optional query parameters</span></span>
<span data-ttu-id="9243d-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9243d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9243d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9243d-120">Request headers</span></span>
| <span data-ttu-id="9243d-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9243d-121">Name</span></span>       | <span data-ttu-id="9243d-122">Тип</span><span class="sxs-lookup"><span data-stu-id="9243d-122">Type</span></span> | <span data-ttu-id="9243d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9243d-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9243d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9243d-124">Authorization</span></span>  | <span data-ttu-id="9243d-125">string</span><span class="sxs-lookup"><span data-stu-id="9243d-125">string</span></span>  | <span data-ttu-id="9243d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9243d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9243d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9243d-128">Request body</span></span>
<span data-ttu-id="9243d-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9243d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9243d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9243d-130">Response</span></span>

<span data-ttu-id="9243d-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9243d-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9243d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9243d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9243d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9243d-133">Request</span></span>
<span data-ttu-id="9243d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9243d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="9243d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="9243d-135">Response</span></span>
<span data-ttu-id="9243d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9243d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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