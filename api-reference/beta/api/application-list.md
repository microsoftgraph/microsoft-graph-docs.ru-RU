---
title: Список приложений
description: Получение списка приложений в этой организации.
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 802bf9197ad7574dbf2480fb7c0631e3fd212d9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459005"
---
# <a name="list-applications"></a><span data-ttu-id="94a39-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="94a39-103">List applications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94a39-104">Получение списка приложений в этой организации.</span><span class="sxs-lookup"><span data-stu-id="94a39-104">Retrieve the list of applications in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="94a39-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94a39-105">Permissions</span></span>
<span data-ttu-id="94a39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94a39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="94a39-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94a39-108">Permission type</span></span>      | <span data-ttu-id="94a39-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94a39-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94a39-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94a39-110">Delegated (work or school account)</span></span> | <span data-ttu-id="94a39-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94a39-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="94a39-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94a39-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94a39-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94a39-113">Not supported.</span></span>    |
|<span data-ttu-id="94a39-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94a39-114">Application</span></span> | <span data-ttu-id="94a39-115">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="94a39-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94a39-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94a39-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="94a39-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="94a39-117">Optional query parameters</span></span>
<span data-ttu-id="94a39-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="94a39-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94a39-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94a39-119">Request headers</span></span>
| <span data-ttu-id="94a39-120">Имя</span><span class="sxs-lookup"><span data-stu-id="94a39-120">Name</span></span>       | <span data-ttu-id="94a39-121">Тип</span><span class="sxs-lookup"><span data-stu-id="94a39-121">Type</span></span> | <span data-ttu-id="94a39-122">Описание</span><span class="sxs-lookup"><span data-stu-id="94a39-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="94a39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94a39-123">Authorization</span></span>  | <span data-ttu-id="94a39-124">string</span><span class="sxs-lookup"><span data-stu-id="94a39-124">string</span></span>  | <span data-ttu-id="94a39-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94a39-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94a39-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94a39-127">Request body</span></span>
<span data-ttu-id="94a39-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94a39-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94a39-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="94a39-129">Response</span></span>

<span data-ttu-id="94a39-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="94a39-130">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94a39-131">Пример</span><span class="sxs-lookup"><span data-stu-id="94a39-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94a39-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="94a39-132">Request</span></span>
<span data-ttu-id="94a39-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94a39-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```http
GET https://graph.microsoft.com/beta/applications
```
##### <a name="response"></a><span data-ttu-id="94a39-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="94a39-134">Response</span></span>
<span data-ttu-id="94a39-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94a39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1229

{
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
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
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
