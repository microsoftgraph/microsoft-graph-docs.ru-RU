---
title: Список registeredOwners
description: Получение списка пользователей, являющихся зарегистрированными владельцами устройства. Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство. Зарегистрированный владелец задается при регистрации. Сейчас можно настроить лишь одного такого владельца.
ms.openlocfilehash: 7a56e036ac904f98fdc1cc2d4f781f97f43c85dc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025216"
---
# <a name="list-registeredowners"></a><span data-ttu-id="e36d7-106">Список registeredOwners</span><span class="sxs-lookup"><span data-stu-id="e36d7-106">List registeredOwners</span></span>

<span data-ttu-id="e36d7-107">Получение списка пользователей, являющихся зарегистрированными владельцами устройства.</span><span class="sxs-lookup"><span data-stu-id="e36d7-107">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="e36d7-108">Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство.</span><span class="sxs-lookup"><span data-stu-id="e36d7-108">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="e36d7-109">Зарегистрированный владелец задается при регистрации.</span><span class="sxs-lookup"><span data-stu-id="e36d7-109">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="e36d7-110">Сейчас можно настроить лишь одного такого владельца.</span><span class="sxs-lookup"><span data-stu-id="e36d7-110">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="e36d7-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e36d7-111">Permissions</span></span>
<span data-ttu-id="e36d7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e36d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e36d7-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e36d7-114">Permission type</span></span>      | <span data-ttu-id="e36d7-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e36d7-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e36d7-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e36d7-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e36d7-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e36d7-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e36d7-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e36d7-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e36d7-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e36d7-119">Not supported.</span></span>    |
|<span data-ttu-id="e36d7-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="e36d7-120">Application</span></span> | <span data-ttu-id="e36d7-121">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e36d7-121">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e36d7-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e36d7-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e36d7-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e36d7-123">Optional query parameters</span></span>
<span data-ttu-id="e36d7-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e36d7-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e36d7-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e36d7-125">Request headers</span></span>
| <span data-ttu-id="e36d7-126">Имя</span><span class="sxs-lookup"><span data-stu-id="e36d7-126">Name</span></span>       | <span data-ttu-id="e36d7-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e36d7-127">Type</span></span> | <span data-ttu-id="e36d7-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e36d7-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e36d7-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="e36d7-129">Authorization</span></span>  | <span data-ttu-id="e36d7-130">string</span><span class="sxs-lookup"><span data-stu-id="e36d7-130">string</span></span>  | <span data-ttu-id="e36d7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e36d7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e36d7-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e36d7-133">Request body</span></span>
<span data-ttu-id="e36d7-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e36d7-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e36d7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e36d7-135">Response</span></span>

<span data-ttu-id="e36d7-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e36d7-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e36d7-137">Пример</span><span class="sxs-lookup"><span data-stu-id="e36d7-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e36d7-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="e36d7-138">Request</span></span>
<span data-ttu-id="e36d7-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e36d7-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="e36d7-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="e36d7-140">Response</span></span>
<span data-ttu-id="e36d7-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e36d7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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