---
title: Список Scopedadministrators для роли каталога
description: Получение списка объектов Scopedrolemembership изменен для роли каталога.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 606ca3e919bcb07fb23a075f015d24be78a739f2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260658"
---
# <a name="list-scopedmembers-for-a-directory-role"></a><span data-ttu-id="3bd2c-103">Список Scopedadministrators для роли каталога</span><span class="sxs-lookup"><span data-stu-id="3bd2c-103">List scopedMembers for a directory role</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bd2c-104">Получение списка объектов [scopedrolemembership изменен](../resources/scopedrolemembership.md) для роли каталога.</span><span class="sxs-lookup"><span data-stu-id="3bd2c-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) objects for a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="3bd2c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3bd2c-105">Permissions</span></span>
<span data-ttu-id="3bd2c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bd2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bd2c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3bd2c-108">Permission type</span></span>      | <span data-ttu-id="3bd2c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3bd2c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bd2c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bd2c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3bd2c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3bd2c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3bd2c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bd2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bd2c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bd2c-113">Not supported.</span></span>    |
|<span data-ttu-id="3bd2c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3bd2c-114">Application</span></span> | <span data-ttu-id="3bd2c-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bd2c-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bd2c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bd2c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryroles/{id}/scopedMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3bd2c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3bd2c-117">Optional query parameters</span></span>
<span data-ttu-id="3bd2c-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3bd2c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3bd2c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bd2c-119">Request headers</span></span>
| <span data-ttu-id="3bd2c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3bd2c-120">Name</span></span>      |<span data-ttu-id="3bd2c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3bd2c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3bd2c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3bd2c-122">Authorization</span></span>  | <span data-ttu-id="3bd2c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3bd2c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3bd2c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3bd2c-125">Request body</span></span>
<span data-ttu-id="3bd2c-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3bd2c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bd2c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="3bd2c-127">Response</span></span>

<span data-ttu-id="3bd2c-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [scopedrolemembership изменен](../resources/scopedrolemembership.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3bd2c-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3bd2c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3bd2c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3bd2c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bd2c-130">Request</span></span>
<span data-ttu-id="3bd2c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3bd2c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/scopedMembers
```
##### <a name="response"></a><span data-ttu-id="3bd2c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bd2c-132">Response</span></span>
<span data-ttu-id="3bd2c-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3bd2c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
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
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3bd2c-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="3bd2c-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3bd2c-137">C#</span><span class="sxs-lookup"><span data-stu-id="3bd2c-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_scopedmembers_directoryrole-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3bd2c-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="3bd2c-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_scopedmembers_directoryrole-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3bd2c-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3bd2c-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_scopedmembers_directoryrole-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedmembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-list-scopedadministrators.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directoryrole-list-scopedadministrators.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryrole-list-scopedadministrators.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
