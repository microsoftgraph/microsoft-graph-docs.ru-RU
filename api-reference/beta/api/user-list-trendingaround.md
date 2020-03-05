---
title: Список trendingAround
description: Вычисляемое представление, возвращающее список элементов, которые обходить пользователь.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6b1da05001da565e03cdcc06fc46459e971cf660
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451744"
---
# <a name="list-trendingaround"></a><span data-ttu-id="3f502-103">Список trendingAround</span><span class="sxs-lookup"><span data-stu-id="3f502-103">List trendingAround</span></span>

<span data-ttu-id="3f502-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3f502-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f502-105">Вычисляемое представление, возвращающее список элементов, которые обходить пользователь.</span><span class="sxs-lookup"><span data-stu-id="3f502-105">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="3f502-106">**Примечание:** Этот API будет устаревшим и заменен [API-интерфейсом тенденций](../resources/insights-trending.md).</span><span class="sxs-lookup"><span data-stu-id="3f502-106">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3f502-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f502-107">Permissions</span></span>
<span data-ttu-id="3f502-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f502-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f502-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f502-110">Permission type</span></span>      | <span data-ttu-id="3f502-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f502-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f502-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f502-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3f502-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f502-113">Sites.Read.All</span></span>    |
|<span data-ttu-id="3f502-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f502-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f502-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f502-115">Not supported.</span></span>    |
|<span data-ttu-id="3f502-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f502-116">Application</span></span> | <span data-ttu-id="3f502-117">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f502-117">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f502-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f502-118">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3f502-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3f502-119">Optional query parameters</span></span>
<span data-ttu-id="3f502-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3f502-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f502-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f502-121">Request headers</span></span>
| <span data-ttu-id="3f502-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f502-122">Header</span></span>         | <span data-ttu-id="3f502-123">Значение</span><span class="sxs-lookup"><span data-stu-id="3f502-123">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="3f502-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f502-124">Authorization</span></span>  | <span data-ttu-id="3f502-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f502-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3f502-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3f502-127">Content-Type</span></span>   | <span data-ttu-id="3f502-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3f502-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="3f502-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f502-129">Request body</span></span>
<span data-ttu-id="3f502-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3f502-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f502-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="3f502-131">Response</span></span>

<span data-ttu-id="3f502-132">В случае успешного выполнения этот метод возвращает код ответа 200 ОК и коллекцию объектов [driveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f502-132">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f502-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3f502-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f502-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f502-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="3f502-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f502-135">Response</span></span>
<span data-ttu-id="3f502-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f502-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
