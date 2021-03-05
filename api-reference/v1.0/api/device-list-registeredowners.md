---
title: Список registeredOwners
description: Получение списка пользователей, являющихся зарегистрированными владельцами устройства.
localization_priority: Normal
author: spunukol
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 198655463c227fa5f0b7b547e59c9f11b08b7571
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434589"
---
# <a name="list-registeredowners"></a><span data-ttu-id="e26a5-103">Список registeredOwners</span><span class="sxs-lookup"><span data-stu-id="e26a5-103">List registeredOwners</span></span>

<span data-ttu-id="e26a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e26a5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e26a5-105">Получение списка пользователей, являющихся зарегистрированными владельцами устройства.</span><span class="sxs-lookup"><span data-stu-id="e26a5-105">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="e26a5-106">Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство.</span><span class="sxs-lookup"><span data-stu-id="e26a5-106">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="e26a5-107">Зарегистрированный владелец задается при регистрации.</span><span class="sxs-lookup"><span data-stu-id="e26a5-107">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="e26a5-108">Сейчас можно настроить лишь одного такого владельца.</span><span class="sxs-lookup"><span data-stu-id="e26a5-108">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="e26a5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e26a5-109">Permissions</span></span>
<span data-ttu-id="e26a5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e26a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e26a5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e26a5-112">Permission type</span></span>      | <span data-ttu-id="e26a5-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e26a5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e26a5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e26a5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e26a5-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e26a5-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e26a5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e26a5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e26a5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e26a5-117">Not supported.</span></span>    |
|<span data-ttu-id="e26a5-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e26a5-118">Application</span></span> | <span data-ttu-id="e26a5-119">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e26a5-119">Directory.Read.All or Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e26a5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e26a5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e26a5-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e26a5-121">Optional query parameters</span></span>
<span data-ttu-id="e26a5-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e26a5-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e26a5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e26a5-123">Request headers</span></span>
| <span data-ttu-id="e26a5-124">Имя</span><span class="sxs-lookup"><span data-stu-id="e26a5-124">Name</span></span>       | <span data-ttu-id="e26a5-125">Тип</span><span class="sxs-lookup"><span data-stu-id="e26a5-125">Type</span></span> | <span data-ttu-id="e26a5-126">Описание</span><span class="sxs-lookup"><span data-stu-id="e26a5-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e26a5-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e26a5-127">Authorization</span></span>  | <span data-ttu-id="e26a5-128">string</span><span class="sxs-lookup"><span data-stu-id="e26a5-128">string</span></span>  | <span data-ttu-id="e26a5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e26a5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e26a5-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e26a5-131">Request body</span></span>
<span data-ttu-id="e26a5-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e26a5-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e26a5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e26a5-133">Response</span></span>

<span data-ttu-id="e26a5-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e26a5-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e26a5-135">Пример</span><span class="sxs-lookup"><span data-stu-id="e26a5-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e26a5-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="e26a5-136">Request</span></span>
<span data-ttu-id="e26a5-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e26a5-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e26a5-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e26a5-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
# <a name="c"></a>[<span data-ttu-id="e26a5-139">C#</span><span class="sxs-lookup"><span data-stu-id="e26a5-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e26a5-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e26a5-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e26a5-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e26a5-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e26a5-142">Java</span><span class="sxs-lookup"><span data-stu-id="e26a5-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e26a5-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e26a5-143">Response</span></span>
<span data-ttu-id="e26a5-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e26a5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
