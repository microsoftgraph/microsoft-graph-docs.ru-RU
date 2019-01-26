---
title: Список oauth2PermissionGrants
description: Получение списка объектов oauth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: 4a3ab48b4ab3162fd2222bc98f261d4f12c8d39a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572642"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="61b0c-103">Список oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="61b0c-103">List oauth2PermissionGrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61b0c-104">Получение списка объектов oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="61b0c-104">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="61b0c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61b0c-105">Permissions</span></span>

<span data-ttu-id="61b0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61b0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="61b0c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61b0c-108">Permission type</span></span>      | <span data-ttu-id="61b0c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61b0c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61b0c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61b0c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="61b0c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="61b0c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="61b0c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61b0c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61b0c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61b0c-113">Not supported.</span></span>    |
|<span data-ttu-id="61b0c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61b0c-114">Application</span></span> | <span data-ttu-id="61b0c-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61b0c-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="61b0c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61b0c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="61b0c-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="61b0c-117">Optional query parameters</span></span>
<span data-ttu-id="61b0c-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="61b0c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="61b0c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61b0c-119">Request headers</span></span>
| <span data-ttu-id="61b0c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="61b0c-120">Name</span></span> | <span data-ttu-id="61b0c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="61b0c-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="61b0c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="61b0c-122">Authorization</span></span>  | <span data-ttu-id="61b0c-123">string</span><span class="sxs-lookup"><span data-stu-id="61b0c-123">string</span></span>  | <span data-ttu-id="61b0c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61b0c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61b0c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61b0c-126">Request body</span></span>
<span data-ttu-id="61b0c-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="61b0c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61b0c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="61b0c-128">Response</span></span>

<span data-ttu-id="61b0c-129">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="61b0c-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="61b0c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="61b0c-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="61b0c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="61b0c-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
##### <a name="response"></a><span data-ttu-id="61b0c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="61b0c-132">Response</span></span>

<span data-ttu-id="61b0c-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="61b0c-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
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
