---
title: Список trendingAround
description: Вычисляемое представление, возвращающее список элементов, которые обходить пользователь.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dc7b6176fe4fceeeeea78d63c6b7140568ff6875
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996191"
---
# <a name="list-trendingaround"></a><span data-ttu-id="3cdd3-103">Список trendingAround</span><span class="sxs-lookup"><span data-stu-id="3cdd3-103">List trendingAround</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cdd3-104">Вычисляемое представление, возвращающее список элементов, которые обходить пользователь.</span><span class="sxs-lookup"><span data-stu-id="3cdd3-104">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="3cdd3-105">**Примечание:** Этот API будет устаревшим и заменен [API](../resources/insights-trending.md)-интерфейсом тенденций.</span><span class="sxs-lookup"><span data-stu-id="3cdd3-105">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3cdd3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3cdd3-106">Permissions</span></span>
<span data-ttu-id="3cdd3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cdd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cdd3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cdd3-109">Permission type</span></span>      | <span data-ttu-id="3cdd3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cdd3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cdd3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cdd3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3cdd3-112">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cdd3-112">Sites.Read.All</span></span>    |
|<span data-ttu-id="3cdd3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cdd3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cdd3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cdd3-114">Not supported.</span></span>    |
|<span data-ttu-id="3cdd3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cdd3-115">Application</span></span> | <span data-ttu-id="3cdd3-116">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="3cdd3-116">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cdd3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cdd3-117">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3cdd3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3cdd3-118">Optional query parameters</span></span>
<span data-ttu-id="3cdd3-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3cdd3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cdd3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3cdd3-120">Request headers</span></span>
| <span data-ttu-id="3cdd3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3cdd3-121">Header</span></span>         | <span data-ttu-id="3cdd3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3cdd3-122">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="3cdd3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3cdd3-123">Authorization</span></span>  | <span data-ttu-id="3cdd3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cdd3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3cdd3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3cdd3-126">Content-Type</span></span>   | <span data-ttu-id="3cdd3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3cdd3-127">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="3cdd3-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3cdd3-128">Request body</span></span>
<span data-ttu-id="3cdd3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3cdd3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cdd3-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3cdd3-130">Response</span></span>

<span data-ttu-id="3cdd3-131">В случае успешного выполнения этот метод возвращает код ответа 200 ОК и коллекцию объектов [driveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3cdd3-131">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cdd3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3cdd3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3cdd3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3cdd3-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="3cdd3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cdd3-134">Response</span></span>
<span data-ttu-id="3cdd3-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3cdd3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
