---
title: Список registeredOwners
description: Получение списка пользователей, являющихся зарегистрированными владельцами устройства. Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство. Зарегистрированный владелец задается при регистрации. Сейчас можно настроить лишь одного такого владельца.
localization_priority: Normal
ms.openlocfilehash: f2b39217485ef248cb7da203152f8e87c483096d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845684"
---
# <a name="list-registeredowners"></a><span data-ttu-id="1fbfd-106">Список registeredOwners</span><span class="sxs-lookup"><span data-stu-id="1fbfd-106">List registeredOwners</span></span>

<span data-ttu-id="1fbfd-107">Получение списка пользователей, являющихся зарегистрированными владельцами устройства.</span><span class="sxs-lookup"><span data-stu-id="1fbfd-107">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="1fbfd-108">Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство.</span><span class="sxs-lookup"><span data-stu-id="1fbfd-108">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="1fbfd-109">Зарегистрированный владелец задается при регистрации.</span><span class="sxs-lookup"><span data-stu-id="1fbfd-109">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="1fbfd-110">Сейчас можно настроить лишь одного такого владельца.</span><span class="sxs-lookup"><span data-stu-id="1fbfd-110">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fbfd-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1fbfd-111">Permissions</span></span>
<span data-ttu-id="1fbfd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fbfd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1fbfd-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fbfd-114">Permission type</span></span>      | <span data-ttu-id="1fbfd-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fbfd-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fbfd-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fbfd-116">Delegated (work or school account)</span></span> | <span data-ttu-id="1fbfd-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1fbfd-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1fbfd-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fbfd-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fbfd-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fbfd-119">Not supported.</span></span>    |
|<span data-ttu-id="1fbfd-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="1fbfd-120">Application</span></span> | <span data-ttu-id="1fbfd-121">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fbfd-121">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fbfd-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fbfd-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1fbfd-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1fbfd-123">Optional query parameters</span></span>
<span data-ttu-id="1fbfd-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1fbfd-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1fbfd-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1fbfd-125">Request headers</span></span>
| <span data-ttu-id="1fbfd-126">Имя</span><span class="sxs-lookup"><span data-stu-id="1fbfd-126">Name</span></span>       | <span data-ttu-id="1fbfd-127">Тип</span><span class="sxs-lookup"><span data-stu-id="1fbfd-127">Type</span></span> | <span data-ttu-id="1fbfd-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1fbfd-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1fbfd-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fbfd-129">Authorization</span></span>  | <span data-ttu-id="1fbfd-130">string</span><span class="sxs-lookup"><span data-stu-id="1fbfd-130">string</span></span>  | <span data-ttu-id="1fbfd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fbfd-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fbfd-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1fbfd-133">Request body</span></span>
<span data-ttu-id="1fbfd-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1fbfd-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fbfd-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fbfd-135">Response</span></span>

<span data-ttu-id="1fbfd-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1fbfd-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1fbfd-137">Пример</span><span class="sxs-lookup"><span data-stu-id="1fbfd-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1fbfd-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fbfd-138">Request</span></span>
<span data-ttu-id="1fbfd-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fbfd-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="1fbfd-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="1fbfd-140">Response</span></span>
<span data-ttu-id="1fbfd-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1fbfd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
