---
title: Перечисление oauth2PermissionGrants
description: Получение списка объектов oauth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: 9af84b4af64466658058259a665d426484511526
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643257"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="0006b-103">Перечисление oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="0006b-103">List oauth2PermissionGrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0006b-104">Получение списка объектов oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="0006b-104">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0006b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0006b-105">Permissions</span></span>

<span data-ttu-id="0006b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0006b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0006b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0006b-108">Permission type</span></span>      | <span data-ttu-id="0006b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0006b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0006b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0006b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0006b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0006b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0006b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0006b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0006b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0006b-113">Not supported.</span></span>    |
|<span data-ttu-id="0006b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0006b-114">Application</span></span> | <span data-ttu-id="0006b-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0006b-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0006b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0006b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0006b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0006b-117">Optional query parameters</span></span>
<span data-ttu-id="0006b-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0006b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0006b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0006b-119">Request headers</span></span>
| <span data-ttu-id="0006b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0006b-120">Name</span></span> | <span data-ttu-id="0006b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0006b-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="0006b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0006b-122">Authorization</span></span>  | <span data-ttu-id="0006b-123">строка</span><span class="sxs-lookup"><span data-stu-id="0006b-123">string</span></span>  | <span data-ttu-id="0006b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0006b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0006b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0006b-126">Request body</span></span>
<span data-ttu-id="0006b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0006b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0006b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="0006b-128">Response</span></span>

<span data-ttu-id="0006b-129">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0006b-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0006b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0006b-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0006b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0006b-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
##### <a name="response"></a><span data-ttu-id="0006b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0006b-132">Response</span></span>

<span data-ttu-id="0006b-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0006b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 259

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "datetime-value",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value",
      "startTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/oauth2permissiongrant-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
