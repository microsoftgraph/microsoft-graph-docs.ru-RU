---
title: 'servicePrincipal: List oAuth2Permissiongrants'
description: Получение списка объектов oAuth2Permissiongrant.
localization_priority: Normal
ms.openlocfilehash: 6dabbe8e3ffacbb375ab4b3a9a44d92cf18ef2f6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263786"
---
# <a name="serviceprincipal-list-oauth2permissiongrants"></a><span data-ttu-id="3f9bb-103">servicePrincipal: List oAuth2Permissiongrants</span><span class="sxs-lookup"><span data-stu-id="3f9bb-103">servicePrincipal: List oAuth2Permissiongrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f9bb-104">Получение списка объектов oAuth2Permissiongrant.</span><span class="sxs-lookup"><span data-stu-id="3f9bb-104">Retrieve a list of oAuth2Permissiongrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f9bb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f9bb-105">Permissions</span></span>
<span data-ttu-id="3f9bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f9bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f9bb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f9bb-108">Permission type</span></span>      | <span data-ttu-id="3f9bb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f9bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f9bb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f9bb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3f9bb-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3f9bb-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3f9bb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f9bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f9bb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f9bb-113">Not supported.</span></span>    |
|<span data-ttu-id="3f9bb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f9bb-114">Application</span></span> | <span data-ttu-id="3f9bb-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f9bb-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f9bb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f9bb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/oAuth2Permissiongrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3f9bb-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3f9bb-117">Optional query parameters</span></span>
<span data-ttu-id="3f9bb-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3f9bb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f9bb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f9bb-119">Request headers</span></span>
| <span data-ttu-id="3f9bb-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3f9bb-120">Name</span></span>       | <span data-ttu-id="3f9bb-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3f9bb-121">Type</span></span> | <span data-ttu-id="3f9bb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3f9bb-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3f9bb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f9bb-123">Authorization</span></span>  | <span data-ttu-id="3f9bb-124">string</span><span class="sxs-lookup"><span data-stu-id="3f9bb-124">string</span></span>  | <span data-ttu-id="3f9bb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f9bb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f9bb-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3f9bb-127">Request body</span></span>
<span data-ttu-id="3f9bb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3f9bb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f9bb-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3f9bb-129">Response</span></span>

<span data-ttu-id="3f9bb-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f9bb-130">If successful, this method returns a `200 OK` response code and collection of [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3f9bb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3f9bb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f9bb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f9bb-132">Request</span></span>
<span data-ttu-id="3f9bb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f9bb-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/oAuth2Permissiongrants
```
##### <a name="response"></a><span data-ttu-id="3f9bb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f9bb-134">Response</span></span>
<span data-ttu-id="3f9bb-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f9bb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3f9bb-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="3f9bb-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3f9bb-139">C#</span><span class="sxs-lookup"><span data-stu-id="3f9bb-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_oAuth2Permissiongrants-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3f9bb-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="3f9bb-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_oAuth2Permissiongrants-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3f9bb-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3f9bb-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_oAuth2Permissiongrants-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oAuth2Permissiongrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-oauth2permissiongrants.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/serviceprincipal-list-oauth2permissiongrants.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-list-oauth2permissiongrants.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
