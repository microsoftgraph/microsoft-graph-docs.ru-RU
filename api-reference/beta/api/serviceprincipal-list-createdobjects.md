---
title: 'servicePrincipal: Перечисление createdObjects'
description: Получение списка объектов directoryobject.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: d6904f7183247f9b47977fe89eff65cf0129883e
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373050"
---
# <a name="serviceprincipal-list-createdobjects"></a><span data-ttu-id="1fe88-103">servicePrincipal: Перечисление createdObjects</span><span class="sxs-lookup"><span data-stu-id="1fe88-103">servicePrincipal: List createdObjects</span></span>

<span data-ttu-id="1fe88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fe88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fe88-105">Получение списка объектов directoryobject.</span><span class="sxs-lookup"><span data-stu-id="1fe88-105">Retrieve a list of directoryobject objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fe88-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1fe88-106">Permissions</span></span>
<span data-ttu-id="1fe88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fe88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fe88-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fe88-109">Permission type</span></span>      | <span data-ttu-id="1fe88-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fe88-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fe88-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fe88-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1fe88-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1fe88-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1fe88-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fe88-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fe88-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fe88-114">Not supported.</span></span>    |
|<span data-ttu-id="1fe88-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1fe88-115">Application</span></span> | <span data-ttu-id="1fe88-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fe88-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="1fe88-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fe88-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1fe88-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1fe88-118">Optional query parameters</span></span>
<span data-ttu-id="1fe88-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1fe88-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1fe88-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1fe88-120">Request headers</span></span>
| <span data-ttu-id="1fe88-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1fe88-121">Name</span></span>           | <span data-ttu-id="1fe88-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1fe88-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="1fe88-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1fe88-123">Authorization</span></span>  | <span data-ttu-id="1fe88-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fe88-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1fe88-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1fe88-126">Request body</span></span>
<span data-ttu-id="1fe88-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1fe88-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fe88-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fe88-128">Response</span></span>

<span data-ttu-id="1fe88-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1fe88-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="1fe88-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="1fe88-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="1fe88-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fe88-131">Request</span></span>
<span data-ttu-id="1fe88-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fe88-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1fe88-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fe88-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipals_get_createdobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/createdObjects
```
# <a name="c"></a>[<span data-ttu-id="1fe88-134">C#</span><span class="sxs-lookup"><span data-stu-id="1fe88-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fe88-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fe88-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fe88-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fe88-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1fe88-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fe88-137">Response</span></span>
<span data-ttu-id="1fe88-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1fe88-138">Here is an example of the response.</span></span> 
><span data-ttu-id="1fe88-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1fe88-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
