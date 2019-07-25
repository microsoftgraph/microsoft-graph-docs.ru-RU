---
title: Список registeredOwners
description: Получение списка пользователей, являющихся зарегистрированными владельцами устройства. Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство. Зарегистрированный владелец задается при регистрации. Сейчас можно настроить лишь одного такого владельца.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 479901336f2f38b57aff268e90e0fcd3b7a96f5f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862732"
---
# <a name="list-registeredowners"></a><span data-ttu-id="a51f3-106">Список registeredOwners</span><span class="sxs-lookup"><span data-stu-id="a51f3-106">List registeredOwners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a51f3-107">Получение списка пользователей, являющихся зарегистрированными владельцами устройства.</span><span class="sxs-lookup"><span data-stu-id="a51f3-107">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="a51f3-108">Зарегистрированный владелец — пользователь, который присоединил устройство через облако или зарегистрировал личное устройство.</span><span class="sxs-lookup"><span data-stu-id="a51f3-108">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="a51f3-109">Зарегистрированный владелец задается при регистрации.</span><span class="sxs-lookup"><span data-stu-id="a51f3-109">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="a51f3-110">Сейчас можно настроить лишь одного такого владельца.</span><span class="sxs-lookup"><span data-stu-id="a51f3-110">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="a51f3-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a51f3-111">Permissions</span></span>

<span data-ttu-id="a51f3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a51f3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a51f3-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a51f3-114">Permission type</span></span>      | <span data-ttu-id="a51f3-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a51f3-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a51f3-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a51f3-116">Delegated (work or school account)</span></span> | <span data-ttu-id="a51f3-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a51f3-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a51f3-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a51f3-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a51f3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a51f3-119">Not supported.</span></span>    |
|<span data-ttu-id="a51f3-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a51f3-120">Application</span></span> | <span data-ttu-id="a51f3-121">Directory.Read.All или Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a51f3-121">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a51f3-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a51f3-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```

> <span data-ttu-id="a51f3-123">Примечание. Параметр id в запросе — это свойство id объекта device, а не свойство deviceId.</span><span class="sxs-lookup"><span data-stu-id="a51f3-123">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="a51f3-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a51f3-124">Optional query parameters</span></span>
<span data-ttu-id="a51f3-125">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a51f3-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a51f3-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a51f3-126">Request headers</span></span>
| <span data-ttu-id="a51f3-127">Имя</span><span class="sxs-lookup"><span data-stu-id="a51f3-127">Name</span></span>       | <span data-ttu-id="a51f3-128">Тип</span><span class="sxs-lookup"><span data-stu-id="a51f3-128">Type</span></span> | <span data-ttu-id="a51f3-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a51f3-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a51f3-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="a51f3-130">Authorization</span></span>  | <span data-ttu-id="a51f3-131">string</span><span class="sxs-lookup"><span data-stu-id="a51f3-131">string</span></span>  | <span data-ttu-id="a51f3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a51f3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a51f3-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a51f3-134">Request body</span></span>
<span data-ttu-id="a51f3-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a51f3-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a51f3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a51f3-136">Response</span></span>

<span data-ttu-id="a51f3-137">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a51f3-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a51f3-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a51f3-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a51f3-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a51f3-139">Request</span></span>
<span data-ttu-id="a51f3-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a51f3-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a51f3-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="a51f3-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredOwners
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a51f3-142">C#</span><span class="sxs-lookup"><span data-stu-id="a51f3-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a51f3-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="a51f3-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a51f3-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a51f3-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a51f3-145">Java</span><span class="sxs-lookup"><span data-stu-id="a51f3-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a51f3-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="a51f3-146">Response</span></span>
<span data-ttu-id="a51f3-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a51f3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
