---
title: Получение scopedRoleMember
description: Получение определенных scopedRoleMembership ресурсов.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0e961097184730922aebd4348f88b8570d5c24ca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525992"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="3d751-103">Получение scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="3d751-103">Get a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d751-104">Получение определенных [scopedRoleMembership](../resources/scopedrolemembership.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="3d751-104">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="3d751-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d751-105">Permissions</span></span>
<span data-ttu-id="3d751-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d751-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3d751-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d751-108">Permission type</span></span>      | <span data-ttu-id="3d751-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d751-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d751-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d751-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3d751-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3d751-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3d751-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d751-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d751-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d751-113">Not supported.</span></span>    |
|<span data-ttu-id="3d751-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d751-114">Application</span></span> | <span data-ttu-id="3d751-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d751-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d751-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d751-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3d751-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3d751-117">Optional query parameters</span></span>
<span data-ttu-id="3d751-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3d751-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d751-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d751-119">Request headers</span></span>
| <span data-ttu-id="3d751-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3d751-120">Name</span></span>      |<span data-ttu-id="3d751-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3d751-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3d751-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d751-122">Authorization</span></span>  | <span data-ttu-id="3d751-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d751-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d751-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d751-125">Request body</span></span>
<span data-ttu-id="3d751-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3d751-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d751-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="3d751-127">Response</span></span>

<span data-ttu-id="3d751-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект запрошенный [scopedRoleMembership](../resources/scopedrolemembership.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3d751-128">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3d751-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3d751-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d751-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d751-130">Request</span></span>
<span data-ttu-id="3d751-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d751-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="3d751-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="3d751-132">Response</span></span>
<span data-ttu-id="3d751-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="3d751-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership"
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
    "Error: /api-reference/beta/api/administrativeunit-get-scopedrolemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
