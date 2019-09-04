---
title: Список групп устройств
description: Получение групп, непосредственным участником которых является это устройство. Эта операция не является транзитивной.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e81e2b5257b6142592aed8c6fc02eff05baee7ac
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719663"
---
# <a name="list-device-groups"></a><span data-ttu-id="9ec96-104">Список групп устройств</span><span class="sxs-lookup"><span data-stu-id="9ec96-104">List device groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ec96-105">Получение групп, непосредственным участником которых является это устройство.</span><span class="sxs-lookup"><span data-stu-id="9ec96-105">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="9ec96-106">Эта операция не является транзитивной.</span><span class="sxs-lookup"><span data-stu-id="9ec96-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ec96-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ec96-107">Permissions</span></span>

<span data-ttu-id="9ec96-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ec96-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ec96-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ec96-110">Permission type</span></span>      | <span data-ttu-id="9ec96-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ec96-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ec96-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ec96-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9ec96-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9ec96-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9ec96-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ec96-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ec96-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ec96-115">Not supported.</span></span>    |
|<span data-ttu-id="9ec96-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ec96-116">Application</span></span> | <span data-ttu-id="9ec96-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ec96-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ec96-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ec96-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9ec96-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9ec96-119">Optional query parameters</span></span>
<span data-ttu-id="9ec96-120">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9ec96-120">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9ec96-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ec96-121">Request headers</span></span>
| <span data-ttu-id="9ec96-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ec96-122">Header</span></span>       | <span data-ttu-id="9ec96-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9ec96-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9ec96-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ec96-124">Authorization</span></span>  | <span data-ttu-id="9ec96-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ec96-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9ec96-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9ec96-127">Accept</span></span>  | <span data-ttu-id="9ec96-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9ec96-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ec96-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9ec96-129">Request body</span></span>
<span data-ttu-id="9ec96-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ec96-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ec96-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ec96-131">Response</span></span>

<span data-ttu-id="9ec96-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ec96-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ec96-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9ec96-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ec96-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ec96-134">Request</span></span>

<span data-ttu-id="9ec96-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ec96-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9ec96-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ec96-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ec96-137">C#</span><span class="sxs-lookup"><span data-stu-id="9ec96-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ec96-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ec96-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ec96-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9ec96-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9ec96-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ec96-140">Response</span></span>
<span data-ttu-id="9ec96-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ec96-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
