---
title: Получение объекта appRoleAssignment
description: Получение свойств и связей объекта appRoleAssignment.
localization_priority: Priority
ms.openlocfilehash: 35537c45e4f156a0b78ffc708eaa39fec8625754
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459012"
---
# <a name="get-approleassignment"></a><span data-ttu-id="9c3c3-103">Получение объекта appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9c3c3-103">Get appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c3c3-104">Получение свойств и связей объекта appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="9c3c3-104">Retrieve the properties and relationships of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9c3c3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c3c3-105">Permissions</span></span>
<span data-ttu-id="9c3c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c3c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c3c3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c3c3-108">Permission type</span></span>      | <span data-ttu-id="9c3c3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c3c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c3c3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c3c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9c3c3-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9c3c3-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9c3c3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c3c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c3c3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c3c3-113">Not supported.</span></span>    |
|<span data-ttu-id="9c3c3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c3c3-114">Application</span></span> | <span data-ttu-id="9c3c3-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c3c3-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c3c3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c3c3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments/{id}
GET /servicePrincipals/{id}/appRoleAssignedTo
GET /groups/{id}/appRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9c3c3-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9c3c3-117">Optional query parameters</span></span>
<span data-ttu-id="9c3c3-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9c3c3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c3c3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c3c3-119">Request headers</span></span>
| <span data-ttu-id="9c3c3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9c3c3-120">Name</span></span>       | <span data-ttu-id="9c3c3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9c3c3-121">Type</span></span> | <span data-ttu-id="9c3c3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9c3c3-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9c3c3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c3c3-123">Authorization</span></span>  | <span data-ttu-id="9c3c3-124">string</span><span class="sxs-lookup"><span data-stu-id="9c3c3-124">string</span></span>  | <span data-ttu-id="9c3c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c3c3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c3c3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c3c3-127">Request body</span></span>
<span data-ttu-id="9c3c3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c3c3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c3c3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c3c3-129">Response</span></span>

<span data-ttu-id="9c3c3-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [appRoleAssignment](../resources/approleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9c3c3-130">If successful, this method returns a `200 OK` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9c3c3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9c3c3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c3c3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c3c3-132">Request</span></span>
<span data-ttu-id="9c3c3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c3c3-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="9c3c3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c3c3-134">Response</span></span>
<span data-ttu-id="9c3c3-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9c3c3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/approleassignment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
