---
title: Список registeredOwners
description: Получение списка пользователей, являющихся зарегистрированными владельцами устройства.
localization_priority: Normal
author: spunukol
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 192c618de517dbcc076c8bbd95205075bc7cd81a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437179"
---
# <a name="list-registeredowners"></a><span data-ttu-id="02ae9-103">Список registeredOwners</span><span class="sxs-lookup"><span data-stu-id="02ae9-103">List registeredOwners</span></span>

<span data-ttu-id="02ae9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02ae9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02ae9-105">Получение списка пользователей, являющихся зарегистрированными владельцами устройства.</span><span class="sxs-lookup"><span data-stu-id="02ae9-105">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="02ae9-106">Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство.</span><span class="sxs-lookup"><span data-stu-id="02ae9-106">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="02ae9-107">Зарегистрированный владелец задается при регистрации.</span><span class="sxs-lookup"><span data-stu-id="02ae9-107">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="02ae9-108">Сейчас можно настроить лишь одного такого владельца.</span><span class="sxs-lookup"><span data-stu-id="02ae9-108">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="02ae9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02ae9-109">Permissions</span></span>

<span data-ttu-id="02ae9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02ae9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02ae9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02ae9-112">Permission type</span></span>      | <span data-ttu-id="02ae9-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02ae9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02ae9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02ae9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="02ae9-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="02ae9-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="02ae9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02ae9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02ae9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02ae9-117">Not supported.</span></span>    |
|<span data-ttu-id="02ae9-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="02ae9-118">Application</span></span> | <span data-ttu-id="02ae9-119">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02ae9-119">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="02ae9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02ae9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```

> <span data-ttu-id="02ae9-121">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="02ae9-121">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="02ae9-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="02ae9-122">Optional query parameters</span></span>
<span data-ttu-id="02ae9-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="02ae9-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="02ae9-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02ae9-124">Request headers</span></span>
| <span data-ttu-id="02ae9-125">Имя</span><span class="sxs-lookup"><span data-stu-id="02ae9-125">Name</span></span>       | <span data-ttu-id="02ae9-126">Тип</span><span class="sxs-lookup"><span data-stu-id="02ae9-126">Type</span></span> | <span data-ttu-id="02ae9-127">Описание</span><span class="sxs-lookup"><span data-stu-id="02ae9-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="02ae9-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="02ae9-128">Authorization</span></span>  | <span data-ttu-id="02ae9-129">string</span><span class="sxs-lookup"><span data-stu-id="02ae9-129">string</span></span>  | <span data-ttu-id="02ae9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02ae9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02ae9-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="02ae9-132">Request body</span></span>
<span data-ttu-id="02ae9-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02ae9-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02ae9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="02ae9-134">Response</span></span>

<span data-ttu-id="02ae9-135">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="02ae9-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="02ae9-136">Пример</span><span class="sxs-lookup"><span data-stu-id="02ae9-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02ae9-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="02ae9-137">Request</span></span>
<span data-ttu-id="02ae9-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02ae9-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="02ae9-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="02ae9-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/registeredOwners
```
# <a name="c"></a>[<span data-ttu-id="02ae9-140">C#</span><span class="sxs-lookup"><span data-stu-id="02ae9-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02ae9-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02ae9-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02ae9-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02ae9-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02ae9-143">Java</span><span class="sxs-lookup"><span data-stu-id="02ae9-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="02ae9-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="02ae9-144">Response</span></span>
<span data-ttu-id="02ae9-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02ae9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
