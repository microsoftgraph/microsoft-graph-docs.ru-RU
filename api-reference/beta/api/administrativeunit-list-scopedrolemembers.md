---
title: Список Scopedadministrators
description: Получение списка ресурсов Scopedrolemembership изменен.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4254723a4902772cf45b1af024058a32192bc8fb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459642"
---
# <a name="list-scopedrolemembers"></a><span data-ttu-id="651ce-103">Список Scopedadministrators</span><span class="sxs-lookup"><span data-stu-id="651ce-103">List scopedRoleMembers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="651ce-104">Получение списка ресурсов [scopedrolemembership изменен](../resources/scopedrolemembership.md) .</span><span class="sxs-lookup"><span data-stu-id="651ce-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) resources.</span></span>
## <a name="permissions"></a><span data-ttu-id="651ce-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="651ce-105">Permissions</span></span>
<span data-ttu-id="651ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="651ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="651ce-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="651ce-108">Permission type</span></span>      | <span data-ttu-id="651ce-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="651ce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="651ce-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="651ce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="651ce-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="651ce-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="651ce-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="651ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="651ce-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="651ce-113">Not supported.</span></span>    |
|<span data-ttu-id="651ce-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="651ce-114">Application</span></span> | <span data-ttu-id="651ce-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="651ce-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="651ce-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="651ce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="651ce-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="651ce-117">Optional query parameters</span></span>
<span data-ttu-id="651ce-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="651ce-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="651ce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="651ce-119">Request headers</span></span>
| <span data-ttu-id="651ce-120">Имя</span><span class="sxs-lookup"><span data-stu-id="651ce-120">Name</span></span>      |<span data-ttu-id="651ce-121">Описание</span><span class="sxs-lookup"><span data-stu-id="651ce-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="651ce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="651ce-122">Authorization</span></span>  | <span data-ttu-id="651ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="651ce-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="651ce-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="651ce-125">Request body</span></span>
<span data-ttu-id="651ce-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="651ce-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="651ce-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="651ce-127">Response</span></span>

<span data-ttu-id="651ce-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [scopedrolemembership изменен](../resources/scopedrolemembership.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="651ce-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="651ce-129">Пример</span><span class="sxs-lookup"><span data-stu-id="651ce-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="651ce-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="651ce-130">Request</span></span>
<span data-ttu-id="651ce-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="651ce-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers
```
##### <a name="response"></a><span data-ttu-id="651ce-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="651ce-132">Response</span></span>
<span data-ttu-id="651ce-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="651ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership",
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
    "Error: /api-reference/beta/api/administrativeunit-list-scopedrolemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
