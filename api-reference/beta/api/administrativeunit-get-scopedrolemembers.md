---
title: Получение Скопедролемембер
description: Получение определенного ресурса Scopedrolemembership изменен.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a093c731705a07dba933dadd07c01d242b1443a9
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655315"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="7af51-103">Получение Скопедролемембер</span><span class="sxs-lookup"><span data-stu-id="7af51-103">Get a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7af51-104">Получение определенного ресурса [scopedrolemembership изменен](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="7af51-104">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="7af51-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7af51-105">Permissions</span></span>
<span data-ttu-id="7af51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7af51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7af51-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7af51-108">Permission type</span></span>      | <span data-ttu-id="7af51-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7af51-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7af51-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7af51-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7af51-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7af51-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7af51-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7af51-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7af51-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7af51-113">Not supported.</span></span>    |
|<span data-ttu-id="7af51-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7af51-114">Application</span></span> | <span data-ttu-id="7af51-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7af51-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7af51-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7af51-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7af51-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7af51-117">Optional query parameters</span></span>
<span data-ttu-id="7af51-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7af51-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7af51-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7af51-119">Request headers</span></span>
| <span data-ttu-id="7af51-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7af51-120">Name</span></span>      |<span data-ttu-id="7af51-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7af51-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7af51-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7af51-122">Authorization</span></span>  | <span data-ttu-id="7af51-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7af51-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7af51-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7af51-125">Request body</span></span>
<span data-ttu-id="7af51-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7af51-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7af51-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="7af51-127">Response</span></span>

<span data-ttu-id="7af51-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [scopedrolemembership изменен](../resources/scopedrolemembership.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7af51-128">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7af51-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7af51-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7af51-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7af51-130">Request</span></span>
<span data-ttu-id="7af51-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7af51-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="7af51-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7af51-132">Response</span></span>
<span data-ttu-id="7af51-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7af51-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "id": "id-value",
  "roleId": "roleId-value",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleMemberInfo": {
      "id": "id-value",
      "displayName": "displayName-value",
      "userPrincipalName": "userPrincipalName-value"
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7af51-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="7af51-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7af51-137">C#</span><span class="sxs-lookup"><span data-stu-id="7af51-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_scopedrolemember-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7af51-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="7af51-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_scopedrolemember-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-get-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-get-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
