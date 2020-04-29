---
title: Список групп устройств
description: Получение групп, непосредственным участником которых является это устройство. Эта операция не является транзитивной.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f0164345ca2d58ba5d097b6e872f08c1b4801aeb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464017"
---
# <a name="list-device-groups"></a><span data-ttu-id="64783-104">Список групп устройств</span><span class="sxs-lookup"><span data-stu-id="64783-104">List device groups</span></span>

<span data-ttu-id="64783-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64783-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64783-106">Получение групп, непосредственным участником которых является это устройство.</span><span class="sxs-lookup"><span data-stu-id="64783-106">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="64783-107">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="64783-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="64783-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64783-108">Permissions</span></span>

<span data-ttu-id="64783-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64783-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64783-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64783-111">Permission type</span></span>      | <span data-ttu-id="64783-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64783-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64783-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64783-113">Delegated (work or school account)</span></span> | <span data-ttu-id="64783-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="64783-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="64783-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64783-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64783-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64783-116">Not supported.</span></span>    |
|<span data-ttu-id="64783-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64783-117">Application</span></span> | <span data-ttu-id="64783-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64783-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="64783-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64783-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="64783-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="64783-120">Optional query parameters</span></span>
<span data-ttu-id="64783-121">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="64783-121">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="64783-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64783-122">Request headers</span></span>
| <span data-ttu-id="64783-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64783-123">Header</span></span>       | <span data-ttu-id="64783-124">Значение</span><span class="sxs-lookup"><span data-stu-id="64783-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64783-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64783-125">Authorization</span></span>  | <span data-ttu-id="64783-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64783-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="64783-128">Accept</span><span class="sxs-lookup"><span data-stu-id="64783-128">Accept</span></span>  | <span data-ttu-id="64783-129">application/json</span><span class="sxs-lookup"><span data-stu-id="64783-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64783-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64783-130">Request body</span></span>
<span data-ttu-id="64783-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64783-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64783-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="64783-132">Response</span></span>

<span data-ttu-id="64783-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64783-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64783-134">Пример</span><span class="sxs-lookup"><span data-stu-id="64783-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="64783-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="64783-135">Request</span></span>

<span data-ttu-id="64783-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64783-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64783-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="64783-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="64783-138">C#</span><span class="sxs-lookup"><span data-stu-id="64783-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64783-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64783-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64783-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64783-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64783-141">Java</span><span class="sxs-lookup"><span data-stu-id="64783-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="64783-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="64783-142">Response</span></span>
<span data-ttu-id="64783-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64783-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
