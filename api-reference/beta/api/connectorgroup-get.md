---
title: Получение connectorGroup
description: Извлечение свойств объекта connectorGroup.
localization_priority: Normal
ms.openlocfilehash: fd898eecd6c131bef49c4eecdd266ae92642115a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521791"
---
# <a name="get-connectorgroup"></a><span data-ttu-id="315c9-103">Получение connectorGroup</span><span class="sxs-lookup"><span data-stu-id="315c9-103">Get connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="315c9-104">Извлечение свойств объекта connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="315c9-104">Retrieve the properties of a connectorGroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="315c9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="315c9-105">Permissions</span></span>
<span data-ttu-id="315c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="315c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="315c9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="315c9-108">Permission type</span></span>      | <span data-ttu-id="315c9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="315c9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="315c9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="315c9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="315c9-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="315c9-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="315c9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="315c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="315c9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="315c9-113">Not supported.</span></span>    |
|<span data-ttu-id="315c9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="315c9-114">Application</span></span> | <span data-ttu-id="315c9-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="315c9-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="315c9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="315c9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="315c9-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="315c9-117">Optional query parameters</span></span>
<span data-ttu-id="315c9-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="315c9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="315c9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="315c9-119">Request headers</span></span>
| <span data-ttu-id="315c9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="315c9-120">Name</span></span>      |<span data-ttu-id="315c9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="315c9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="315c9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="315c9-122">Authorization</span></span>  | <span data-ttu-id="315c9-123">Токен носителя.</span><span class="sxs-lookup"><span data-stu-id="315c9-123">Bearer.</span></span> <span data-ttu-id="315c9-124">Обязательный</span><span class="sxs-lookup"><span data-stu-id="315c9-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="315c9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="315c9-125">Request body</span></span>
<span data-ttu-id="315c9-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="315c9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="315c9-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="315c9-127">Response</span></span>

<span data-ttu-id="315c9-128">Успешно завершена, этот метод возвращает `200 OK` объект [connectorGroup](../resources/connectorgroup.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="315c9-128">If successful, this method returns a `200 OK` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="315c9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="315c9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="315c9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="315c9-130">Request</span></span>
<span data-ttu-id="315c9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="315c9-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectorgroup"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="315c9-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="315c9-132">Response</span></span>
<span data-ttu-id="315c9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="315c9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
