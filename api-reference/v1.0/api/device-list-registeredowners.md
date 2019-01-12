---
title: Список registeredOwners
description: Получение списка пользователей, являющихся зарегистрированными владельцами устройства. Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство. Зарегистрированный владелец задается при регистрации. Сейчас можно настроить лишь одного такого владельца.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ec8990a2b0c2d0f674304c4005fbf28a0b5a631e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976893"
---
# <a name="list-registeredowners"></a><span data-ttu-id="7ed25-106">Список registeredOwners</span><span class="sxs-lookup"><span data-stu-id="7ed25-106">List registeredOwners</span></span>

<span data-ttu-id="7ed25-107">Получение списка пользователей, являющихся зарегистрированными владельцами устройства.</span><span class="sxs-lookup"><span data-stu-id="7ed25-107">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="7ed25-108">Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство.</span><span class="sxs-lookup"><span data-stu-id="7ed25-108">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="7ed25-109">Зарегистрированный владелец задается при регистрации.</span><span class="sxs-lookup"><span data-stu-id="7ed25-109">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="7ed25-110">Сейчас можно настроить лишь одного такого владельца.</span><span class="sxs-lookup"><span data-stu-id="7ed25-110">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ed25-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ed25-111">Permissions</span></span>
<span data-ttu-id="7ed25-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ed25-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7ed25-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ed25-114">Permission type</span></span>      | <span data-ttu-id="7ed25-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ed25-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ed25-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ed25-116">Delegated (work or school account)</span></span> | <span data-ttu-id="7ed25-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7ed25-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7ed25-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ed25-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ed25-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ed25-119">Not supported.</span></span>    |
|<span data-ttu-id="7ed25-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="7ed25-120">Application</span></span> | <span data-ttu-id="7ed25-121">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ed25-121">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ed25-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ed25-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7ed25-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7ed25-123">Optional query parameters</span></span>
<span data-ttu-id="7ed25-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7ed25-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7ed25-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ed25-125">Request headers</span></span>
| <span data-ttu-id="7ed25-126">Имя</span><span class="sxs-lookup"><span data-stu-id="7ed25-126">Name</span></span>       | <span data-ttu-id="7ed25-127">Тип</span><span class="sxs-lookup"><span data-stu-id="7ed25-127">Type</span></span> | <span data-ttu-id="7ed25-128">Описание</span><span class="sxs-lookup"><span data-stu-id="7ed25-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7ed25-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ed25-129">Authorization</span></span>  | <span data-ttu-id="7ed25-130">строка</span><span class="sxs-lookup"><span data-stu-id="7ed25-130">string</span></span>  | <span data-ttu-id="7ed25-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ed25-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ed25-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ed25-133">Request body</span></span>
<span data-ttu-id="7ed25-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ed25-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ed25-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ed25-135">Response</span></span>

<span data-ttu-id="7ed25-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7ed25-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7ed25-137">Пример</span><span class="sxs-lookup"><span data-stu-id="7ed25-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ed25-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ed25-138">Request</span></span>
<span data-ttu-id="7ed25-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ed25-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="7ed25-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ed25-140">Response</span></span>
<span data-ttu-id="7ed25-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7ed25-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
