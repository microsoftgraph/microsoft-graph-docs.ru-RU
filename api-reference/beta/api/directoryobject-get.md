---
title: Получение объекта DirectoryObject
description: Извлечение свойств и связей объекта directoryobject.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7303cefc9779f4080ddccd3fbe6b55ec6a4404c3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436920"
---
# <a name="get-directoryobject"></a><span data-ttu-id="8cd68-103">Получение объекта DirectoryObject</span><span class="sxs-lookup"><span data-stu-id="8cd68-103">Get directoryObject</span></span>

<span data-ttu-id="8cd68-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cd68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cd68-105">Извлечение свойств и связей объекта directoryobject.</span><span class="sxs-lookup"><span data-stu-id="8cd68-105">Retrieve the properties and relationships of directoryobject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8cd68-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8cd68-106">Permissions</span></span>
<span data-ttu-id="8cd68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cd68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cd68-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cd68-109">Permission type</span></span>      | <span data-ttu-id="8cd68-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cd68-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cd68-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cd68-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8cd68-112">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8cd68-112">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8cd68-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cd68-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cd68-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cd68-114">Not supported.</span></span>    |
|<span data-ttu-id="8cd68-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8cd68-115">Application</span></span> | <span data-ttu-id="8cd68-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cd68-116">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cd68-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cd68-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8cd68-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8cd68-118">Optional query parameters</span></span>
<span data-ttu-id="8cd68-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8cd68-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8cd68-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cd68-120">Request headers</span></span>
| <span data-ttu-id="8cd68-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8cd68-121">Name</span></span>       | <span data-ttu-id="8cd68-122">Тип</span><span class="sxs-lookup"><span data-stu-id="8cd68-122">Type</span></span> | <span data-ttu-id="8cd68-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8cd68-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8cd68-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cd68-124">Authorization</span></span>  | <span data-ttu-id="8cd68-125">string</span><span class="sxs-lookup"><span data-stu-id="8cd68-125">string</span></span>  | <span data-ttu-id="8cd68-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cd68-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cd68-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8cd68-128">Request body</span></span>
<span data-ttu-id="8cd68-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8cd68-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cd68-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cd68-130">Response</span></span>

<span data-ttu-id="8cd68-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8cd68-131">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8cd68-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8cd68-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8cd68-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cd68-133">Request</span></span>
<span data-ttu-id="8cd68-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cd68-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8cd68-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cd68-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryObjects/{id}
```
# <a name="c"></a>[<span data-ttu-id="8cd68-136">C#</span><span class="sxs-lookup"><span data-stu-id="8cd68-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8cd68-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cd68-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8cd68-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cd68-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8cd68-139">Java</span><span class="sxs-lookup"><span data-stu-id="8cd68-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8cd68-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cd68-140">Response</span></span>
<span data-ttu-id="8cd68-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8cd68-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 22

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
