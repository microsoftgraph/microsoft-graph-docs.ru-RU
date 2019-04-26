---
title: Список приложений
description: Получение списка приложений в этой организации.
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5b0addab6106999bcb11333016b43819e8a79027
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322966"
---
# <a name="list-applications"></a><span data-ttu-id="fa64f-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="fa64f-103">List applications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa64f-104">Получение списка приложений в этой организации.</span><span class="sxs-lookup"><span data-stu-id="fa64f-104">Retrieve the list of applications in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa64f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa64f-105">Permissions</span></span>
<span data-ttu-id="fa64f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa64f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fa64f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa64f-108">Permission type</span></span>      | <span data-ttu-id="fa64f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa64f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa64f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa64f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fa64f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa64f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fa64f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa64f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa64f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa64f-113">Not supported.</span></span>    |
|<span data-ttu-id="fa64f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa64f-114">Application</span></span> | <span data-ttu-id="fa64f-115">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa64f-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa64f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa64f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fa64f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fa64f-117">Optional query parameters</span></span>
<span data-ttu-id="fa64f-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fa64f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa64f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa64f-119">Request headers</span></span>
| <span data-ttu-id="fa64f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fa64f-120">Name</span></span>       | <span data-ttu-id="fa64f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="fa64f-121">Type</span></span> | <span data-ttu-id="fa64f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fa64f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fa64f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa64f-123">Authorization</span></span>  | <span data-ttu-id="fa64f-124">string</span><span class="sxs-lookup"><span data-stu-id="fa64f-124">string</span></span>  | <span data-ttu-id="fa64f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa64f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fa64f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa64f-127">Request body</span></span>
<span data-ttu-id="fa64f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa64f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa64f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa64f-129">Response</span></span>

<span data-ttu-id="fa64f-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [application](../resources/application.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa64f-130">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fa64f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fa64f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa64f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa64f-132">Request</span></span>
<span data-ttu-id="fa64f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa64f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```http
GET https://graph.microsoft.com/beta/applications
```
##### <a name="response"></a><span data-ttu-id="fa64f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa64f-134">Response</span></span>
<span data-ttu-id="fa64f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa64f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
