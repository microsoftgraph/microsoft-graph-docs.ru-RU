---
title: Список memberOf
description: Получение connectorgroup, которое соединитель.
localization_priority: Normal
ms.openlocfilehash: 4f9bea5e61b12b6a59413a3a159148e6b5963f16
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530169"
---
# <a name="list-memberof"></a><span data-ttu-id="57934-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="57934-103">List memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57934-104">Получение connectorgroup, которое соединитель.</span><span class="sxs-lookup"><span data-stu-id="57934-104">Retrieve the connectorgroup the connector is a member of.</span></span>
## <a name="permissions"></a><span data-ttu-id="57934-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57934-105">Permissions</span></span>
<span data-ttu-id="57934-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57934-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57934-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57934-108">Permission type</span></span>      | <span data-ttu-id="57934-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57934-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57934-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57934-110">Delegated (work or school account)</span></span> | <span data-ttu-id="57934-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="57934-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="57934-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57934-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57934-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57934-113">Not supported.</span></span>    |
|<span data-ttu-id="57934-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57934-114">Application</span></span> | <span data-ttu-id="57934-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57934-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57934-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57934-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectors/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="57934-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="57934-117">Optional query parameters</span></span>
<span data-ttu-id="57934-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="57934-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57934-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57934-119">Request headers</span></span>
| <span data-ttu-id="57934-120">Имя</span><span class="sxs-lookup"><span data-stu-id="57934-120">Name</span></span>      |<span data-ttu-id="57934-121">Описание</span><span class="sxs-lookup"><span data-stu-id="57934-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="57934-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="57934-122">Authorization</span></span>  | <span data-ttu-id="57934-123">Токен носителя.</span><span class="sxs-lookup"><span data-stu-id="57934-123">Bearer.</span></span> <span data-ttu-id="57934-124">Обязательный</span><span class="sxs-lookup"><span data-stu-id="57934-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="57934-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57934-125">Request body</span></span>
<span data-ttu-id="57934-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57934-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57934-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="57934-127">Response</span></span>

<span data-ttu-id="57934-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [connectorGroup](../resources/connectorgroup.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="57934-128">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="57934-129">Пример</span><span class="sxs-lookup"><span data-stu-id="57934-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="57934-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="57934-130">Request</span></span>
<span data-ttu-id="57934-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57934-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="57934-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="57934-132">Response</span></span>
<span data-ttu-id="57934-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="57934-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 164

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value",
      "connectorGroupType": "connectorGroupType-value",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connector-list-memberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
