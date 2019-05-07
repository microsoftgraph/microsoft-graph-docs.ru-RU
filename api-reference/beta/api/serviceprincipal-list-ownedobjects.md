---
title: 'СервицепринЦипалс: List ownedObjects'
description: Получение списка объектов, принадлежащих servicePrincipal.  Это могут быть приложения или группы.
localization_priority: Normal
ms.openlocfilehash: 8837b6c0505b31fa187ce5bf3caebe27b950a155
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638720"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="8b314-104">СервицепринЦипалс: List ownedObjects</span><span class="sxs-lookup"><span data-stu-id="8b314-104">servicePrincipals: List ownedObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b314-105">Получение списка объектов, принадлежащих servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="8b314-105">Retrieve a list of objects owned by the servicePrincipal.</span></span>  <span data-ttu-id="8b314-106">Это могут быть приложения или группы.</span><span class="sxs-lookup"><span data-stu-id="8b314-106">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b314-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b314-107">Permissions</span></span>
<span data-ttu-id="8b314-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b314-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b314-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b314-110">Permission type</span></span>      | <span data-ttu-id="8b314-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b314-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b314-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b314-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8b314-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8b314-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8b314-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b314-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b314-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b314-115">Not supported.</span></span>    |
|<span data-ttu-id="8b314-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b314-116">Application</span></span> | <span data-ttu-id="8b314-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b314-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b314-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b314-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8b314-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8b314-119">Optional query parameters</span></span>
<span data-ttu-id="8b314-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8b314-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b314-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b314-121">Request headers</span></span>
| <span data-ttu-id="8b314-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8b314-122">Name</span></span>       | <span data-ttu-id="8b314-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8b314-123">Type</span></span> | <span data-ttu-id="8b314-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8b314-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8b314-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b314-125">Authorization</span></span>  | <span data-ttu-id="8b314-126">string</span><span class="sxs-lookup"><span data-stu-id="8b314-126">string</span></span>  | <span data-ttu-id="8b314-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b314-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b314-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b314-129">Request body</span></span>
<span data-ttu-id="8b314-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b314-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b314-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b314-131">Response</span></span>

<span data-ttu-id="8b314-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b314-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b314-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8b314-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b314-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b314-134">Request</span></span>
<span data-ttu-id="8b314-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b314-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
##### <a name="response"></a><span data-ttu-id="8b314-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b314-136">Response</span></span>
<span data-ttu-id="8b314-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b314-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8b314-140">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="8b314-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8b314-141">Языках</span><span class="sxs-lookup"><span data-stu-id="8b314-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_ownedobjects-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8b314-142">Язык</span><span class="sxs-lookup"><span data-stu-id="8b314-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_ownedobjects-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-ownedobjects.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-list-ownedobjects.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
