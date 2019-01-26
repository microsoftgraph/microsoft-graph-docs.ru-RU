---
title: 'servicePrincipal: список oAuth2Permissiongrants'
description: Получение списка объектов oAuth2Permissiongrant.
localization_priority: Normal
ms.openlocfilehash: 2d7e27b61dc9c0cdeb4f2f188bb945a3b4544f16
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572628"
---
# <a name="serviceprincipal-list-oauth2permissiongrants"></a><span data-ttu-id="29cd9-103">servicePrincipal: список oAuth2Permissiongrants</span><span class="sxs-lookup"><span data-stu-id="29cd9-103">servicePrincipal: List oAuth2Permissiongrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29cd9-104">Получение списка объектов oAuth2Permissiongrant.</span><span class="sxs-lookup"><span data-stu-id="29cd9-104">Retrieve a list of oAuth2Permissiongrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="29cd9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29cd9-105">Permissions</span></span>
<span data-ttu-id="29cd9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29cd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29cd9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29cd9-108">Permission type</span></span>      | <span data-ttu-id="29cd9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29cd9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29cd9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29cd9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="29cd9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29cd9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="29cd9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29cd9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29cd9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29cd9-113">Not supported.</span></span>    |
|<span data-ttu-id="29cd9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29cd9-114">Application</span></span> | <span data-ttu-id="29cd9-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29cd9-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29cd9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29cd9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/oAuth2Permissiongrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="29cd9-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="29cd9-117">Optional query parameters</span></span>
<span data-ttu-id="29cd9-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="29cd9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29cd9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="29cd9-119">Request headers</span></span>
| <span data-ttu-id="29cd9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="29cd9-120">Name</span></span>       | <span data-ttu-id="29cd9-121">Тип</span><span class="sxs-lookup"><span data-stu-id="29cd9-121">Type</span></span> | <span data-ttu-id="29cd9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="29cd9-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="29cd9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="29cd9-123">Authorization</span></span>  | <span data-ttu-id="29cd9-124">string</span><span class="sxs-lookup"><span data-stu-id="29cd9-124">string</span></span>  | <span data-ttu-id="29cd9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29cd9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29cd9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="29cd9-127">Request body</span></span>
<span data-ttu-id="29cd9-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="29cd9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29cd9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="29cd9-129">Response</span></span>

<span data-ttu-id="29cd9-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="29cd9-130">If successful, this method returns a `200 OK` response code and collection of [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29cd9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="29cd9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29cd9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="29cd9-132">Request</span></span>
<span data-ttu-id="29cd9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29cd9-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/oAuth2Permissiongrants
```
##### <a name="response"></a><span data-ttu-id="29cd9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="29cd9-134">Response</span></span>
<span data-ttu-id="29cd9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="29cd9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/serviceprincipal-list-oauth2permissiongrants.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
