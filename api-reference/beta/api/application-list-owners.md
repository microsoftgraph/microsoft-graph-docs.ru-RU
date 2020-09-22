---
title: Список владельцев
description: Получение списка владельцев (объектов directoryObject) для приложения.
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 10a722762b3691f7b495f0b315ee8e4533f00772
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996915"
---
# <a name="list-owners"></a><span data-ttu-id="8b8f0-103">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="8b8f0-103">List owners</span></span>

<span data-ttu-id="8b8f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b8f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b8f0-105">Получение списка владельцев для приложения, которое является [directoryObject](../resources/directoryobject.md) объектами.</span><span class="sxs-lookup"><span data-stu-id="8b8f0-105">Retrieve a list of owners for an application that are [directoryObject](../resources/directoryobject.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b8f0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b8f0-106">Permissions</span></span>
<span data-ttu-id="8b8f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b8f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b8f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b8f0-109">Permission type</span></span>      | <span data-ttu-id="8b8f0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b8f0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b8f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b8f0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8b8f0-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8b8f0-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8b8f0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b8f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b8f0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b8f0-114">Not supported.</span></span>    |
|<span data-ttu-id="8b8f0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b8f0-115">Application</span></span> | <span data-ttu-id="8b8f0-116">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b8f0-116">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="8b8f0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b8f0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8b8f0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8b8f0-118">Optional query parameters</span></span>
<span data-ttu-id="8b8f0-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8b8f0-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b8f0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b8f0-120">Request headers</span></span>
| <span data-ttu-id="8b8f0-121">Имя</span><span class="sxs-lookup"><span data-stu-id="8b8f0-121">Name</span></span>           | <span data-ttu-id="8b8f0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8b8f0-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="8b8f0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b8f0-123">Authorization</span></span>  | <span data-ttu-id="8b8f0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b8f0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8b8f0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8b8f0-126">Request body</span></span>
<span data-ttu-id="8b8f0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b8f0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b8f0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b8f0-128">Response</span></span>

<span data-ttu-id="8b8f0-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b8f0-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b8f0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8b8f0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b8f0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b8f0-131">Request</span></span>
<span data-ttu-id="8b8f0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b8f0-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b8f0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b8f0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="8b8f0-134">C#</span><span class="sxs-lookup"><span data-stu-id="8b8f0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b8f0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b8f0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b8f0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b8f0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8b8f0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b8f0-137">Response</span></span>
<span data-ttu-id="8b8f0-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b8f0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


