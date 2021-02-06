---
title: 'servicePrincipal: Перечисление createdObjects'
description: Получение списка объектов directoryobject.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 52a36d4afaaee71775b0b88a690d54c30ce36cc6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134343"
---
# <a name="serviceprincipal-list-createdobjects"></a><span data-ttu-id="334b1-103">servicePrincipal: Перечисление createdObjects</span><span class="sxs-lookup"><span data-stu-id="334b1-103">servicePrincipal: List createdObjects</span></span>

<span data-ttu-id="334b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="334b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="334b1-105">Получение списка объектов directoryobject.</span><span class="sxs-lookup"><span data-stu-id="334b1-105">Retrieve a list of directoryobject objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="334b1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="334b1-106">Permissions</span></span>
<span data-ttu-id="334b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="334b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="334b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="334b1-109">Permission type</span></span>      | <span data-ttu-id="334b1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="334b1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="334b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="334b1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="334b1-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="334b1-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="334b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="334b1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="334b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="334b1-114">Not supported.</span></span>    |
|<span data-ttu-id="334b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="334b1-115">Application</span></span> | <span data-ttu-id="334b1-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="334b1-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="334b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="334b1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="334b1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="334b1-118">Optional query parameters</span></span>
<span data-ttu-id="334b1-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="334b1-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="334b1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="334b1-120">Request headers</span></span>
| <span data-ttu-id="334b1-121">Имя</span><span class="sxs-lookup"><span data-stu-id="334b1-121">Name</span></span>           | <span data-ttu-id="334b1-122">Описание</span><span class="sxs-lookup"><span data-stu-id="334b1-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="334b1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="334b1-123">Authorization</span></span>  | <span data-ttu-id="334b1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="334b1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="334b1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="334b1-126">Request body</span></span>
<span data-ttu-id="334b1-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="334b1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="334b1-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="334b1-128">Response</span></span>

<span data-ttu-id="334b1-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="334b1-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="334b1-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="334b1-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="334b1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="334b1-131">Request</span></span>
<span data-ttu-id="334b1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="334b1-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="334b1-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="334b1-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipals_get_createdobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/createdObjects
```
# <a name="c"></a>[<span data-ttu-id="334b1-134">C#</span><span class="sxs-lookup"><span data-stu-id="334b1-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="334b1-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="334b1-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="334b1-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="334b1-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="334b1-137">Java</span><span class="sxs-lookup"><span data-stu-id="334b1-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipals-get-createdobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="334b1-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="334b1-138">Response</span></span>
<span data-ttu-id="334b1-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="334b1-139">Here is an example of the response.</span></span> 
><span data-ttu-id="334b1-p103">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="334b1-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

