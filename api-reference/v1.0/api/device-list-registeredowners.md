---
title: Список registeredOwners
description: Получение списка пользователей, являющихся зарегистрированными владельцами устройства. Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство. Зарегистрированный владелец задается при регистрации. Сейчас можно настроить лишь одного такого владельца.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bf56b72389ae3ffebde2dbf27af70f216107e10a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518121"
---
# <a name="list-registeredowners"></a><span data-ttu-id="52a67-106">Список registeredOwners</span><span class="sxs-lookup"><span data-stu-id="52a67-106">List registeredOwners</span></span>

<span data-ttu-id="52a67-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52a67-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="52a67-108">Получение списка пользователей, являющихся зарегистрированными владельцами устройства.</span><span class="sxs-lookup"><span data-stu-id="52a67-108">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="52a67-109">Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство.</span><span class="sxs-lookup"><span data-stu-id="52a67-109">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="52a67-110">Зарегистрированный владелец задается при регистрации.</span><span class="sxs-lookup"><span data-stu-id="52a67-110">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="52a67-111">Сейчас можно настроить лишь одного такого владельца.</span><span class="sxs-lookup"><span data-stu-id="52a67-111">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="52a67-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="52a67-112">Permissions</span></span>
<span data-ttu-id="52a67-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52a67-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="52a67-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52a67-115">Permission type</span></span>      | <span data-ttu-id="52a67-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="52a67-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52a67-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52a67-117">Delegated (work or school account)</span></span> | <span data-ttu-id="52a67-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="52a67-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="52a67-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52a67-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52a67-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52a67-120">Not supported.</span></span>    |
|<span data-ttu-id="52a67-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52a67-121">Application</span></span> | <span data-ttu-id="52a67-122">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52a67-122">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="52a67-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52a67-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="52a67-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="52a67-124">Optional query parameters</span></span>
<span data-ttu-id="52a67-125">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="52a67-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="52a67-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="52a67-126">Request headers</span></span>
| <span data-ttu-id="52a67-127">Имя</span><span class="sxs-lookup"><span data-stu-id="52a67-127">Name</span></span>       | <span data-ttu-id="52a67-128">Тип</span><span class="sxs-lookup"><span data-stu-id="52a67-128">Type</span></span> | <span data-ttu-id="52a67-129">Описание</span><span class="sxs-lookup"><span data-stu-id="52a67-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="52a67-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="52a67-130">Authorization</span></span>  | <span data-ttu-id="52a67-131">string</span><span class="sxs-lookup"><span data-stu-id="52a67-131">string</span></span>  | <span data-ttu-id="52a67-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52a67-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52a67-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="52a67-134">Request body</span></span>
<span data-ttu-id="52a67-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="52a67-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52a67-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="52a67-136">Response</span></span>

<span data-ttu-id="52a67-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52a67-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52a67-138">Пример</span><span class="sxs-lookup"><span data-stu-id="52a67-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52a67-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="52a67-139">Request</span></span>
<span data-ttu-id="52a67-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52a67-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52a67-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="52a67-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
# <a name="c"></a>[<span data-ttu-id="52a67-142">C#</span><span class="sxs-lookup"><span data-stu-id="52a67-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52a67-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52a67-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52a67-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52a67-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52a67-145">Java</span><span class="sxs-lookup"><span data-stu-id="52a67-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="52a67-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="52a67-146">Response</span></span>
<span data-ttu-id="52a67-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="52a67-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
