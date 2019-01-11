---
title: Список registeredOwners
description: Получение списка пользователей, являющихся зарегистрированными владельцами устройства. Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство. Зарегистрированный владелец задается при регистрации. Сейчас можно настроить лишь одного такого владельца.
localization_priority: Normal
ms.openlocfilehash: a0b4fac3ef36ac3137307186ab736b812e5f0274
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833343"
---
# <a name="list-registeredowners"></a><span data-ttu-id="1bd64-106">Список registeredOwners</span><span class="sxs-lookup"><span data-stu-id="1bd64-106">List registeredOwners</span></span>

> <span data-ttu-id="1bd64-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1bd64-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1bd64-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bd64-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1bd64-109">Получение списка пользователей, являющихся зарегистрированными владельцами устройства.</span><span class="sxs-lookup"><span data-stu-id="1bd64-109">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="1bd64-110">Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство.</span><span class="sxs-lookup"><span data-stu-id="1bd64-110">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="1bd64-111">Зарегистрированный владелец задается при регистрации.</span><span class="sxs-lookup"><span data-stu-id="1bd64-111">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="1bd64-112">Сейчас можно настроить лишь одного такого владельца.</span><span class="sxs-lookup"><span data-stu-id="1bd64-112">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bd64-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1bd64-113">Permissions</span></span>

<span data-ttu-id="1bd64-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bd64-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bd64-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bd64-116">Permission type</span></span>      | <span data-ttu-id="1bd64-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bd64-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bd64-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bd64-118">Delegated (work or school account)</span></span> | <span data-ttu-id="1bd64-119">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1bd64-119">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1bd64-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bd64-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bd64-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bd64-121">Not supported.</span></span>    |
|<span data-ttu-id="1bd64-122">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1bd64-122">Application</span></span> | <span data-ttu-id="1bd64-123">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bd64-123">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bd64-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bd64-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```

> <span data-ttu-id="1bd64-125">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="1bd64-125">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="1bd64-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1bd64-126">Optional query parameters</span></span>
<span data-ttu-id="1bd64-127">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1bd64-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1bd64-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bd64-128">Request headers</span></span>
| <span data-ttu-id="1bd64-129">Имя</span><span class="sxs-lookup"><span data-stu-id="1bd64-129">Name</span></span>       | <span data-ttu-id="1bd64-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1bd64-130">Type</span></span> | <span data-ttu-id="1bd64-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1bd64-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1bd64-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bd64-132">Authorization</span></span>  | <span data-ttu-id="1bd64-133">string</span><span class="sxs-lookup"><span data-stu-id="1bd64-133">string</span></span>  | <span data-ttu-id="1bd64-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bd64-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1bd64-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1bd64-136">Request body</span></span>
<span data-ttu-id="1bd64-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1bd64-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bd64-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bd64-138">Response</span></span>

<span data-ttu-id="1bd64-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1bd64-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1bd64-140">Пример</span><span class="sxs-lookup"><span data-stu-id="1bd64-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bd64-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bd64-141">Request</span></span>
<span data-ttu-id="1bd64-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bd64-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="1bd64-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="1bd64-143">Response</span></span>
<span data-ttu-id="1bd64-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1bd64-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
