---
title: Создание appRoleAssignment
description: Используйте этот интерфейс API для создания нового appRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: 33bf7a577b01b2f23132a2b761bd80f24e8268c7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574343"
---
# <a name="create-approleassignment"></a><span data-ttu-id="e902c-103">Создание appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e902c-103">Create appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e902c-104">Используйте этот интерфейс API для создания нового appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="e902c-104">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="e902c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e902c-105">Permissions</span></span>
<span data-ttu-id="e902c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e902c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e902c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e902c-108">Permission type</span></span>      | <span data-ttu-id="e902c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e902c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e902c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e902c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e902c-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e902c-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e902c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e902c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e902c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e902c-113">Not supported.</span></span>    |
|<span data-ttu-id="e902c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e902c-114">Application</span></span> | <span data-ttu-id="e902c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e902c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e902c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e902c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="e902c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e902c-117">Request headers</span></span>
| <span data-ttu-id="e902c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e902c-118">Name</span></span>       | <span data-ttu-id="e902c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e902c-119">Type</span></span> | <span data-ttu-id="e902c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e902c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e902c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e902c-121">Authorization</span></span>  | <span data-ttu-id="e902c-122">string</span><span class="sxs-lookup"><span data-stu-id="e902c-122">string</span></span>  | <span data-ttu-id="e902c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e902c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e902c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e902c-125">Request body</span></span>
<span data-ttu-id="e902c-126">В тексте запроса укажите представление JSON объекта [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e902c-126">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e902c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e902c-127">Response</span></span>

<span data-ttu-id="e902c-128">Успешно завершена, этот метод возвращает `201 Created` объект [appRoleAssignment](../resources/approleassignment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e902c-128">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e902c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="e902c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e902c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e902c-130">Request</span></span>
<span data-ttu-id="e902c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e902c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
<span data-ttu-id="e902c-132">В тексте запроса укажите представление JSON объекта [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e902c-132">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e902c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e902c-133">Response</span></span>
<span data-ttu-id="e902c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e902c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
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
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-post-approleassignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
