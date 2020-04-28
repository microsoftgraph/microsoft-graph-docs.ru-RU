---
title: 'orgContact: List directReports'
description: Получение подчиненных отчетов о контакте.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 05ecd35a75b95818d3789ffb3ef002598267ab61
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466982"
---
# <a name="orgcontact-list-directreports"></a><span data-ttu-id="a7600-103">orgContact: List directReports</span><span class="sxs-lookup"><span data-stu-id="a7600-103">orgContact: List directReports</span></span>

<span data-ttu-id="a7600-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7600-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7600-105">Получение подчиненных отчетов о контакте.</span><span class="sxs-lookup"><span data-stu-id="a7600-105">Get the contact's direct reports.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7600-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7600-106">Permissions</span></span>
<span data-ttu-id="a7600-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7600-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7600-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7600-109">Permission type</span></span>      | <span data-ttu-id="a7600-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7600-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7600-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7600-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a7600-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a7600-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a7600-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7600-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7600-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7600-114">Not supported.</span></span>    |
|<span data-ttu-id="a7600-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7600-115">Application</span></span> | <span data-ttu-id="a7600-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7600-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a7600-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7600-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a7600-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a7600-118">Optional query parameters</span></span>
<span data-ttu-id="a7600-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a7600-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7600-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7600-120">Request headers</span></span>
| <span data-ttu-id="a7600-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a7600-121">Name</span></span>       | <span data-ttu-id="a7600-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a7600-122">Type</span></span> | <span data-ttu-id="a7600-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a7600-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a7600-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7600-124">Authorization</span></span>  | <span data-ttu-id="a7600-125">string</span><span class="sxs-lookup"><span data-stu-id="a7600-125">string</span></span>  | <span data-ttu-id="a7600-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7600-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7600-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a7600-128">Request body</span></span>
<span data-ttu-id="a7600-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7600-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7600-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7600-130">Response</span></span>

<span data-ttu-id="a7600-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7600-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a7600-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a7600-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7600-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7600-133">Request</span></span>
<span data-ttu-id="a7600-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7600-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7600-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7600-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contacts_get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/{id}/directReports
```
# <a name="c"></a>[<span data-ttu-id="a7600-136">C#</span><span class="sxs-lookup"><span data-stu-id="a7600-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contacts-get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7600-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7600-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contacts-get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7600-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7600-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contacts-get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a7600-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7600-139">Response</span></span>
<span data-ttu-id="a7600-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7600-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
