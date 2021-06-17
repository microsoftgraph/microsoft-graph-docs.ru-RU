---
title: Список административныхуунитс
description: Извлечение списка объектов administrativeUnit.
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2117087f09bd3140ae273eae136742bc713da3a2
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991962"
---
# <a name="list-administrativeunits"></a><span data-ttu-id="3bcea-103">Список административныхуунитс</span><span class="sxs-lookup"><span data-stu-id="3bcea-103">List administrativeUnits</span></span>

<span data-ttu-id="3bcea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bcea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bcea-105">Извлечение списка [объектов administrativeUnit.](../resources/administrativeunit.md)</span><span class="sxs-lookup"><span data-stu-id="3bcea-105">Retrieve a list of [administrativeUnit](../resources/administrativeunit.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="3bcea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3bcea-106">Permissions</span></span>
<span data-ttu-id="3bcea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bcea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3bcea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3bcea-109">Permission type</span></span>      | <span data-ttu-id="3bcea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3bcea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bcea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bcea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3bcea-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3bcea-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3bcea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bcea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bcea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bcea-114">Not supported.</span></span>    |
|<span data-ttu-id="3bcea-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3bcea-115">Application</span></span> | <span data-ttu-id="3bcea-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bcea-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bcea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bcea-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3bcea-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3bcea-118">Optional query parameters</span></span>
<span data-ttu-id="3bcea-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3bcea-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3bcea-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bcea-120">Request headers</span></span>
| <span data-ttu-id="3bcea-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3bcea-121">Name</span></span>      |<span data-ttu-id="3bcea-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3bcea-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3bcea-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3bcea-123">Authorization</span></span>  | <span data-ttu-id="3bcea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3bcea-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bcea-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3bcea-126">Request body</span></span>
<span data-ttu-id="3bcea-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3bcea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bcea-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bcea-128">Response</span></span>

<span data-ttu-id="3bcea-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` коллекцию [объектов administrativeUnit](../resources/administrativeunit.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3bcea-129">If successful, this method returns a `200 OK` response code and collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3bcea-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3bcea-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3bcea-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bcea-131">Request</span></span>
<span data-ttu-id="3bcea-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3bcea-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3bcea-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3bcea-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunits"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits
```
# <a name="c"></a>[<span data-ttu-id="3bcea-134">C#</span><span class="sxs-lookup"><span data-stu-id="3bcea-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3bcea-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bcea-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3bcea-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3bcea-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3bcea-137">Java</span><span class="sxs-lookup"><span data-stu-id="3bcea-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-administrativeunits-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3bcea-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bcea-138">Response</span></span>
<span data-ttu-id="3bcea-p103">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3bcea-p103">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
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
