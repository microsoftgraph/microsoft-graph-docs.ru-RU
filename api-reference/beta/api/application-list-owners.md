---
title: Список владельцев
description: Получение списка владельцев (объектов directoryObject) для приложения.
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 29b90fba024d97ceecfd4fe72f37a72de6f7fb8a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129214"
---
# <a name="list-owners"></a><span data-ttu-id="67938-103">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="67938-103">List owners</span></span>

<span data-ttu-id="67938-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67938-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67938-105">Получение списка владельцев приложения, которое является [объектами directoryObject.](../resources/directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="67938-105">Retrieve a list of owners for an application that are [directoryObject](../resources/directoryobject.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="67938-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67938-106">Permissions</span></span>
<span data-ttu-id="67938-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67938-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67938-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67938-109">Permission type</span></span>      | <span data-ttu-id="67938-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67938-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67938-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67938-111">Delegated (work or school account)</span></span> | <span data-ttu-id="67938-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67938-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="67938-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67938-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67938-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67938-114">Not supported.</span></span>    |
|<span data-ttu-id="67938-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67938-115">Application</span></span> | <span data-ttu-id="67938-116">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67938-116">Application.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="67938-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67938-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="67938-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="67938-118">Optional query parameters</span></span>
<span data-ttu-id="67938-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="67938-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67938-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67938-120">Request headers</span></span>
| <span data-ttu-id="67938-121">Имя</span><span class="sxs-lookup"><span data-stu-id="67938-121">Name</span></span>           | <span data-ttu-id="67938-122">Описание</span><span class="sxs-lookup"><span data-stu-id="67938-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="67938-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67938-123">Authorization</span></span>  | <span data-ttu-id="67938-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67938-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="67938-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67938-126">Request body</span></span>
<span data-ttu-id="67938-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="67938-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67938-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="67938-128">Response</span></span>

<span data-ttu-id="67938-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="67938-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67938-130">Пример</span><span class="sxs-lookup"><span data-stu-id="67938-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67938-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="67938-131">Request</span></span>
<span data-ttu-id="67938-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67938-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67938-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="67938-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="67938-134">C#</span><span class="sxs-lookup"><span data-stu-id="67938-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67938-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67938-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67938-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67938-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67938-137">Java</span><span class="sxs-lookup"><span data-stu-id="67938-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="67938-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="67938-138">Response</span></span>
<span data-ttu-id="67938-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67938-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

