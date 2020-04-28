---
title: Список владельцев
description: Получение списка владельцев (объектов directoryObject) для приложения.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9267f95f5b633cad51c7eed2cba27d4488ced8bd
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107229"
---
# <a name="list-owners"></a><span data-ttu-id="f9667-103">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="f9667-103">List owners</span></span>

<span data-ttu-id="f9667-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9667-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9667-105">Получение списка владельцев для приложения, которое является [directoryObject](../resources/directoryobject.md) объектами.</span><span class="sxs-lookup"><span data-stu-id="f9667-105">Retrieve a list of owners for an application that are [directoryObject](../resources/directoryobject.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9667-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9667-106">Permissions</span></span>
<span data-ttu-id="f9667-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9667-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9667-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9667-109">Permission type</span></span>      | <span data-ttu-id="f9667-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9667-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9667-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9667-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f9667-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f9667-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f9667-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9667-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9667-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9667-114">Not supported.</span></span>    |
|<span data-ttu-id="f9667-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9667-115">Application</span></span> | <span data-ttu-id="f9667-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9667-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="f9667-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9667-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f9667-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f9667-118">Optional query parameters</span></span>
<span data-ttu-id="f9667-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f9667-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9667-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9667-120">Request headers</span></span>
| <span data-ttu-id="f9667-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f9667-121">Name</span></span>       | <span data-ttu-id="f9667-122">Тип</span><span class="sxs-lookup"><span data-stu-id="f9667-122">Type</span></span> | <span data-ttu-id="f9667-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f9667-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f9667-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9667-124">Authorization</span></span>  | <span data-ttu-id="f9667-125">string</span><span class="sxs-lookup"><span data-stu-id="f9667-125">string</span></span>  | <span data-ttu-id="f9667-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9667-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f9667-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f9667-128">Request body</span></span>
<span data-ttu-id="f9667-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9667-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9667-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9667-130">Response</span></span>

<span data-ttu-id="f9667-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9667-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9667-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f9667-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9667-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9667-133">Request</span></span>
<span data-ttu-id="f9667-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9667-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f9667-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9667-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="f9667-136">C#</span><span class="sxs-lookup"><span data-stu-id="f9667-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9667-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9667-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9667-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9667-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f9667-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9667-139">Response</span></span>
<span data-ttu-id="f9667-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9667-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
