---
title: Список приложений
description: Получение списка объектов приложения, связанные с connectorGroup.
localization_priority: Normal
ms.openlocfilehash: 47be81d4f154d87865113fa02b04a58151545507
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519362"
---
# <a name="list-applications"></a><span data-ttu-id="6cb77-103">Список приложений</span><span class="sxs-lookup"><span data-stu-id="6cb77-103">List applications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cb77-104">Получение списка объектов приложения, связанные с connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="6cb77-104">Retrieve a list of application objects associated with the connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="6cb77-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6cb77-105">Permissions</span></span>
<span data-ttu-id="6cb77-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cb77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cb77-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cb77-108">Permission type</span></span>      | <span data-ttu-id="6cb77-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cb77-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cb77-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cb77-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6cb77-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6cb77-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6cb77-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cb77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cb77-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cb77-113">Not supported.</span></span>    |
|<span data-ttu-id="6cb77-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6cb77-114">Application</span></span> | <span data-ttu-id="6cb77-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cb77-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cb77-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cb77-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6cb77-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6cb77-117">Optional query parameters</span></span>
<span data-ttu-id="6cb77-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6cb77-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cb77-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6cb77-119">Request headers</span></span>
| <span data-ttu-id="6cb77-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6cb77-120">Name</span></span>      |<span data-ttu-id="6cb77-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6cb77-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6cb77-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cb77-122">Authorization</span></span>  | <span data-ttu-id="6cb77-123">Токен носителя.</span><span class="sxs-lookup"><span data-stu-id="6cb77-123">Bearer.</span></span> <span data-ttu-id="6cb77-124">Обязательный</span><span class="sxs-lookup"><span data-stu-id="6cb77-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cb77-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6cb77-125">Request body</span></span>
<span data-ttu-id="6cb77-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6cb77-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cb77-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="6cb77-127">Response</span></span>

<span data-ttu-id="6cb77-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [приложения](../resources/application.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6cb77-128">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6cb77-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6cb77-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6cb77-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cb77-130">Request</span></span>
<span data-ttu-id="6cb77-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cb77-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
```
##### <a name="response"></a><span data-ttu-id="6cb77-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="6cb77-132">Response</span></span>
<span data-ttu-id="6cb77-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6cb77-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 420

{
  "value": [
    {
      "appId": "appId-value",
      "onPremisesPublishing": {
        "externalUrl": "externalUrl-value",
        "internalUrl": "internalUrl-value",
        "externalAuthenticationType": "externalAuthenticationType-value",
        "customDomainCertificate": "customDomainCertificate-value",
        "isTranslateHostHeaderEnabled": true,
        "isOnPremPublishingEnabled": true
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
    "Error: /api-reference/beta/api/connectorgroup-list-applications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
