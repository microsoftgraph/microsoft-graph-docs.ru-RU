---
title: Список scopedMembers для роли каталога
description: Получение списка объектов scopedRoleMembership для роли каталога.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ab6b68ac96e35249ef216266fafed76be68f40b7
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642480"
---
# <a name="list-scopedmembers-for-a-directory-role"></a><span data-ttu-id="7ebc8-103">Список scopedMembers для роли каталога</span><span class="sxs-lookup"><span data-stu-id="7ebc8-103">List scopedMembers for a directory role</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ebc8-104">Получение списка объектов [scopedRoleMembership](../resources/scopedrolemembership.md) для роли каталога.</span><span class="sxs-lookup"><span data-stu-id="7ebc8-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) objects for a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="7ebc8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ebc8-105">Permissions</span></span>
<span data-ttu-id="7ebc8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ebc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ebc8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ebc8-108">Permission type</span></span>      | <span data-ttu-id="7ebc8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ebc8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ebc8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ebc8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7ebc8-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7ebc8-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7ebc8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ebc8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ebc8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ebc8-113">Not supported.</span></span>    |
|<span data-ttu-id="7ebc8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ebc8-114">Application</span></span> | <span data-ttu-id="7ebc8-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ebc8-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ebc8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ebc8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryroles/{id}/scopedMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7ebc8-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7ebc8-117">Optional query parameters</span></span>
<span data-ttu-id="7ebc8-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7ebc8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ebc8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ebc8-119">Request headers</span></span>
| <span data-ttu-id="7ebc8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7ebc8-120">Name</span></span>      |<span data-ttu-id="7ebc8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7ebc8-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7ebc8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ebc8-122">Authorization</span></span>  | <span data-ttu-id="7ebc8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ebc8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ebc8-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ebc8-125">Request body</span></span>
<span data-ttu-id="7ebc8-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ebc8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ebc8-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ebc8-127">Response</span></span>

<span data-ttu-id="7ebc8-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [scopedRoleMembership](../resources/scopedrolemembership.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7ebc8-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7ebc8-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7ebc8-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ebc8-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ebc8-130">Request</span></span>
<span data-ttu-id="7ebc8-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ebc8-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/scopedMembers
```
##### <a name="response"></a><span data-ttu-id="7ebc8-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ebc8-132">Response</span></span>
<span data-ttu-id="7ebc8-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ebc8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List scopedmembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-list-scopedadministrators.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
