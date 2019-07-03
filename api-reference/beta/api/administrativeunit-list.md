---
title: Список Административеунитс
description: Получение списка объектов administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 12e7fda8ffae49986300a57183f4ed0661a85bda
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439891"
---
# <a name="list-administrativeunits"></a><span data-ttu-id="846b9-103">Список Административеунитс</span><span class="sxs-lookup"><span data-stu-id="846b9-103">List administrativeUnits</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="846b9-104">Получение списка объектов [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="846b9-104">Retrieve a list of [administrativeUnit](../resources/administrativeunit.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="846b9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="846b9-105">Permissions</span></span>
<span data-ttu-id="846b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="846b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="846b9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="846b9-108">Permission type</span></span>      | <span data-ttu-id="846b9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="846b9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="846b9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="846b9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="846b9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="846b9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="846b9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="846b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="846b9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="846b9-113">Not supported.</span></span>    |
|<span data-ttu-id="846b9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="846b9-114">Application</span></span> | <span data-ttu-id="846b9-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="846b9-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="846b9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="846b9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits
```
## <a name="optional-query-parameters"></a><span data-ttu-id="846b9-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="846b9-117">Optional query parameters</span></span>
<span data-ttu-id="846b9-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="846b9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="846b9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="846b9-119">Request headers</span></span>
| <span data-ttu-id="846b9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="846b9-120">Name</span></span>      |<span data-ttu-id="846b9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="846b9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="846b9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="846b9-122">Authorization</span></span>  | <span data-ttu-id="846b9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="846b9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="846b9-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="846b9-125">Request body</span></span>
<span data-ttu-id="846b9-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="846b9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="846b9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="846b9-127">Response</span></span>

<span data-ttu-id="846b9-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [administrativeUnit](../resources/administrativeunit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="846b9-128">If successful, this method returns a `200 OK` response code and collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="846b9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="846b9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="846b9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="846b9-130">Request</span></span>
<span data-ttu-id="846b9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="846b9-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="846b9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="846b9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunits"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="846b9-133">C#</span><span class="sxs-lookup"><span data-stu-id="846b9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="846b9-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="846b9-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="846b9-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="846b9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="846b9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="846b9-136">Response</span></span>
<span data-ttu-id="846b9-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="846b9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
