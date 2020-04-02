---
title: Список trendingAround
description: Вычисляемое представление, возвращающее список элементов, которые обходить пользователь.
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 0746fc8e72c52ef3d406d7473e4bdf43f59d6562
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107551"
---
# <a name="list-trendingaround"></a><span data-ttu-id="c1024-103">Список trendingAround</span><span class="sxs-lookup"><span data-stu-id="c1024-103">List trendingAround</span></span>

<span data-ttu-id="c1024-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1024-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1024-105">Вычисляемое представление, возвращающее список элементов, которые обходить пользователь.</span><span class="sxs-lookup"><span data-stu-id="c1024-105">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="c1024-106">**Примечание:** Этот API будет устаревшим и заменен [API-интерфейсом тенденций](../resources/insights-trending.md).</span><span class="sxs-lookup"><span data-stu-id="c1024-106">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1024-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1024-107">Permissions</span></span>
<span data-ttu-id="c1024-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1024-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1024-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1024-110">Permission type</span></span>      | <span data-ttu-id="c1024-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1024-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1024-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1024-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c1024-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1024-113">Sites.Read.All</span></span>    |
|<span data-ttu-id="c1024-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1024-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1024-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1024-115">Not supported.</span></span>    |
|<span data-ttu-id="c1024-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1024-116">Application</span></span> | <span data-ttu-id="c1024-117">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1024-117">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1024-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1024-118">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c1024-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c1024-119">Optional query parameters</span></span>
<span data-ttu-id="c1024-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c1024-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1024-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1024-121">Request headers</span></span>
| <span data-ttu-id="c1024-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1024-122">Header</span></span>         | <span data-ttu-id="c1024-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c1024-123">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="c1024-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1024-124">Authorization</span></span>  | <span data-ttu-id="c1024-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1024-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c1024-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1024-127">Content-Type</span></span>   | <span data-ttu-id="c1024-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c1024-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="c1024-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c1024-129">Request body</span></span>
<span data-ttu-id="c1024-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c1024-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1024-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1024-131">Response</span></span>

<span data-ttu-id="c1024-132">В случае успешного выполнения этот метод возвращает код ответа 200 ОК и коллекцию объектов [driveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c1024-132">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1024-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c1024-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1024-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1024-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="c1024-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1024-135">Response</span></span>
<span data-ttu-id="c1024-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1024-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
