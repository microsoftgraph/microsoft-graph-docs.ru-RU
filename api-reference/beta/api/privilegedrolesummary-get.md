---
title: Получение privilegedRoleSummary
description: Извлечение свойств и связи объекта privilegedRoleSummary.
localization_priority: Normal
ms.openlocfilehash: 3778ddcc297607b062354dcdf44727a0f57375dc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508232"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="c3064-103">Получение privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="c3064-103">Get privilegedRoleSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3064-104">Извлечение свойств и связи объекта [privilegedRoleSummary](../resources/privilegedrolesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c3064-104">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c3064-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3064-105">Permissions</span></span>
<span data-ttu-id="c3064-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3064-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c3064-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3064-108">Permission type</span></span>      | <span data-ttu-id="c3064-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3064-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3064-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3064-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c3064-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c3064-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c3064-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3064-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3064-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3064-113">Not supported.</span></span>    |
|<span data-ttu-id="c3064-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3064-114">Application</span></span> | <span data-ttu-id="c3064-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3064-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3064-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3064-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c3064-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c3064-117">Optional query parameters</span></span>
<span data-ttu-id="c3064-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c3064-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3064-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3064-119">Request headers</span></span>
| <span data-ttu-id="c3064-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c3064-120">Name</span></span>      |<span data-ttu-id="c3064-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c3064-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c3064-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3064-122">Authorization</span></span>  | <span data-ttu-id="c3064-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3064-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3064-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3064-125">Request body</span></span>
<span data-ttu-id="c3064-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3064-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3064-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3064-127">Response</span></span>

<span data-ttu-id="c3064-128">Успешно завершена, этот метод возвращает `200 OK` объект [privilegedRoleSummary](../resources/privilegedrolesummary.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c3064-128">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="c3064-129">Обратите внимание, что необходимо зарегистрировать для PIM клиента.</span><span class="sxs-lookup"><span data-stu-id="c3064-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c3064-130">В противном случае будут возвращены код состояния HTTP 403 запрещено.</span><span class="sxs-lookup"><span data-stu-id="c3064-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="c3064-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c3064-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3064-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3064-132">Request</span></span>
<span data-ttu-id="c3064-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3064-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
##### <a name="response"></a><span data-ttu-id="c3064-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3064-134">Response</span></span>
<span data-ttu-id="c3064-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c3064-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 137

{
  "id": "id-value",
  "status": "status-value",
  "usersCount": 99,
  "managedCount": 99,
  "elevatedCount": 99,
  "mfaEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrolesummary-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
