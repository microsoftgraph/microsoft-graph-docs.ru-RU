---
title: Список Административеунитс
description: Получение списка объектов administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 10bedf9c47e549576748aabfcd7612d7ddb452ce
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441734"
---
# <a name="list-administrativeunits"></a><span data-ttu-id="b3752-103">Список Административеунитс</span><span class="sxs-lookup"><span data-stu-id="b3752-103">List administrativeUnits</span></span>

<span data-ttu-id="b3752-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b3752-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3752-105">Получение списка объектов [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="b3752-105">Retrieve a list of [administrativeUnit](../resources/administrativeunit.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="b3752-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3752-106">Permissions</span></span>
<span data-ttu-id="b3752-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3752-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b3752-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3752-109">Permission type</span></span>      | <span data-ttu-id="b3752-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3752-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3752-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3752-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b3752-112">AdministrativeUnit. Read. ALL, Directory. Read. ALL, AdministrativeUnit. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="b3752-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b3752-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3752-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3752-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3752-114">Not supported.</span></span>    |
|<span data-ttu-id="b3752-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3752-115">Application</span></span> | <span data-ttu-id="b3752-116">AdministrativeUnit. Read. ALL, Directory. Read. ALL, AdministrativeUnit. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b3752-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3752-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3752-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b3752-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b3752-118">Optional query parameters</span></span>
<span data-ttu-id="b3752-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b3752-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3752-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3752-120">Request headers</span></span>
| <span data-ttu-id="b3752-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b3752-121">Name</span></span>      |<span data-ttu-id="b3752-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b3752-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b3752-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3752-123">Authorization</span></span>  | <span data-ttu-id="b3752-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3752-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3752-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3752-126">Request body</span></span>
<span data-ttu-id="b3752-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3752-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3752-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b3752-128">Response</span></span>

<span data-ttu-id="b3752-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [administrativeUnit](../resources/administrativeunit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b3752-129">If successful, this method returns a `200 OK` response code and collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b3752-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b3752-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b3752-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3752-131">Request</span></span>
<span data-ttu-id="b3752-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3752-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b3752-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3752-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunits"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits
```
# <a name="c"></a>[<span data-ttu-id="b3752-134">C#</span><span class="sxs-lookup"><span data-stu-id="b3752-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3752-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3752-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3752-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3752-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b3752-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3752-137">Response</span></span>
<span data-ttu-id="b3752-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3752-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "value": [
    {
      "displayName": "displayName-value",
      "description": "description-value",
      "visibility": "visibility-value",
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
  "description": "List administrativeUnits",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
