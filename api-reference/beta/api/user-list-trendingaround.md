---
title: Список trendingAround
description: Вычисляемые представление, которое возвращает список элементов, прибора вокруг пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 625ae9d66ce1b891ebdba3209d92bd0e88b06a94
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507630"
---
# <a name="list-trendingaround"></a><span data-ttu-id="c2e93-103">Список trendingAround</span><span class="sxs-lookup"><span data-stu-id="c2e93-103">List trendingAround</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2e93-104">Вычисляемые представление, которое возвращает список элементов, прибора вокруг пользователя.</span><span class="sxs-lookup"><span data-stu-id="c2e93-104">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="c2e93-105">**Примечание:** Этот интерфейс API будет устаревшим и вместо нее [Прибора API](../resources/insights-trending.md).</span><span class="sxs-lookup"><span data-stu-id="c2e93-105">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2e93-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2e93-106">Permissions</span></span>
<span data-ttu-id="c2e93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2e93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2e93-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2e93-109">Permission type</span></span>      | <span data-ttu-id="c2e93-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2e93-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2e93-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2e93-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c2e93-112">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2e93-112">Sites.Read.All</span></span>    |
|<span data-ttu-id="c2e93-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2e93-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2e93-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2e93-114">Not supported.</span></span>    |
|<span data-ttu-id="c2e93-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2e93-115">Application</span></span> | <span data-ttu-id="c2e93-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2e93-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2e93-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2e93-117">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c2e93-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2e93-118">Optional query parameters</span></span>
<span data-ttu-id="c2e93-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c2e93-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2e93-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2e93-120">Request headers</span></span>
| <span data-ttu-id="c2e93-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2e93-121">Header</span></span>         | <span data-ttu-id="c2e93-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2e93-122">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="c2e93-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2e93-123">Authorization</span></span>  | <span data-ttu-id="c2e93-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2e93-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c2e93-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2e93-126">Content-Type</span></span>   | <span data-ttu-id="c2e93-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c2e93-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="c2e93-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2e93-128">Request body</span></span>
<span data-ttu-id="c2e93-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2e93-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2e93-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2e93-130">Response</span></span>

<span data-ttu-id="c2e93-131">Если успешно завершена, этот метод возвращает 200 OK ответа код и коллекцию объектов [driveItem](../resources/driveitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c2e93-131">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2e93-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c2e93-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2e93-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2e93-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="c2e93-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2e93-134">Response</span></span>
<span data-ttu-id="c2e93-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c2e93-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 226

{
  "id": "id-value",
  "name": "name-value",
  "DateTimeCreated": "DateTimeCreated-value",
  "DateTimeLastModified": "DateTimeLastModified-value",
  "webUrl": "webUrl-value",
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-trendingaround.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
