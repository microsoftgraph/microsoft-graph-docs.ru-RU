---
title: Список agreementAcceptances
description: Получение списка объектов agreementAcceptance пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 22babc13c3b1db4cf143a35ab2119e97c43c822b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517871"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="572bf-103">Список agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="572bf-103">List agreementAcceptances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="572bf-104">Получение списка объектов [agreementAcceptance](../resources/agreementacceptance.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="572bf-104">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="572bf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="572bf-105">Permissions</span></span>
<span data-ttu-id="572bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="572bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="572bf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="572bf-108">Permission type</span></span>                        | <span data-ttu-id="572bf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="572bf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="572bf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="572bf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="572bf-111">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="572bf-111">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="572bf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="572bf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="572bf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="572bf-113">Not supported.</span></span> |
|<span data-ttu-id="572bf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="572bf-114">Application</span></span>                            | <span data-ttu-id="572bf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="572bf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="572bf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="572bf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="572bf-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="572bf-117">Request headers</span></span>
| <span data-ttu-id="572bf-118">Имя</span><span class="sxs-lookup"><span data-stu-id="572bf-118">Name</span></span>      |<span data-ttu-id="572bf-119">Описание</span><span class="sxs-lookup"><span data-stu-id="572bf-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="572bf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="572bf-120">Authorization</span></span> | <span data-ttu-id="572bf-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="572bf-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="572bf-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="572bf-122">Request body</span></span>
<span data-ttu-id="572bf-123">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="572bf-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="572bf-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="572bf-124">Response</span></span>
<span data-ttu-id="572bf-125">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [agreementAcceptance](../resources/agreementacceptance.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="572bf-125">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="572bf-126">Пример</span><span class="sxs-lookup"><span data-stu-id="572bf-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="572bf-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="572bf-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
##### <a name="response"></a><span data-ttu-id="572bf-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="572bf-128">Response</span></span>
><span data-ttu-id="572bf-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="572bf-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "agreementId-value",
      "userId": "userId-value",
      "agreementFileId": "agreementFileId-value",
      "recordedDateTime": "datetime-value",
      "userDisplayName": "userDisplayName-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-agreementacceptances.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
