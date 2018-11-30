---
title: Список registeredUsers
description: Получение списка пользователей, являющихся зарегистрированными пользователями устройства.
ms.openlocfilehash: 08c6cc2268daa31b0d365e0201536df3586a798c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077223"
---
# <a name="list-registeredusers"></a><span data-ttu-id="8e690-103">Список registeredUsers</span><span class="sxs-lookup"><span data-stu-id="8e690-103">List registeredUsers</span></span>

> <span data-ttu-id="8e690-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8e690-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e690-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e690-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8e690-106">Получение списка пользователей, являющихся зарегистрированными пользователями устройства.</span><span class="sxs-lookup"><span data-stu-id="8e690-106">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="8e690-107">В случае зарегистрированных личных устройств или устройств, присоединенных через облако, при регистрации для обычных пользователей задается то же значение, что и для владельцев.</span><span class="sxs-lookup"><span data-stu-id="8e690-107">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e690-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e690-108">Permissions</span></span>
<span data-ttu-id="8e690-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e690-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e690-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e690-111">Permission type</span></span>      | <span data-ttu-id="8e690-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e690-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e690-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e690-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8e690-114">Directory.Read.All или Directory.ReadWrite.All или Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8e690-114">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8e690-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e690-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e690-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e690-116">Not supported.</span></span> |
|<span data-ttu-id="8e690-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="8e690-117">Application</span></span> | <span data-ttu-id="8e690-118">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e690-118">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e690-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e690-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="8e690-120">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="8e690-120">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="8e690-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8e690-121">Optional query parameters</span></span>
<span data-ttu-id="8e690-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8e690-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8e690-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e690-123">Request headers</span></span>
| <span data-ttu-id="8e690-124">Имя</span><span class="sxs-lookup"><span data-stu-id="8e690-124">Name</span></span>       | <span data-ttu-id="8e690-125">Тип</span><span class="sxs-lookup"><span data-stu-id="8e690-125">Type</span></span> | <span data-ttu-id="8e690-126">Описание</span><span class="sxs-lookup"><span data-stu-id="8e690-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8e690-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e690-127">Authorization</span></span>  | <span data-ttu-id="8e690-128">string</span><span class="sxs-lookup"><span data-stu-id="8e690-128">string</span></span>  | <span data-ttu-id="8e690-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e690-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e690-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e690-131">Request body</span></span>
<span data-ttu-id="8e690-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e690-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e690-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e690-133">Response</span></span>

<span data-ttu-id="8e690-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e690-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e690-135">Пример</span><span class="sxs-lookup"><span data-stu-id="8e690-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e690-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e690-136">Request</span></span>
<span data-ttu-id="8e690-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e690-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="8e690-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="8e690-138">Response</span></span>
<span data-ttu-id="8e690-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8e690-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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