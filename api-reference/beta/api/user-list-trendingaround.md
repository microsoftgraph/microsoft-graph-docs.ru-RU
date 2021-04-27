---
title: Список trendingAround
description: Вычислимая информация, возвращаемая списку элементов, относяющихся к пользователю.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b1594d031f9ff007a87243ccf0cf481022b48d89
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052588"
---
# <a name="list-trendingaround"></a><span data-ttu-id="e5c41-103">Список trendingAround</span><span class="sxs-lookup"><span data-stu-id="e5c41-103">List trendingAround</span></span>

<span data-ttu-id="e5c41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5c41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5c41-105">Вычислимая информация, возвращаемая списку элементов, относяющихся к пользователю.</span><span class="sxs-lookup"><span data-stu-id="e5c41-105">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="e5c41-106">**Примечание:** Этот API будет обесценить и заменить [API Trending](../resources/insights-trending.md).</span><span class="sxs-lookup"><span data-stu-id="e5c41-106">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e5c41-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5c41-107">Permissions</span></span>
<span data-ttu-id="e5c41-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5c41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5c41-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5c41-110">Permission type</span></span>      | <span data-ttu-id="e5c41-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5c41-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5c41-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5c41-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e5c41-113">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5c41-113">Sites.Read.All</span></span>    |
|<span data-ttu-id="e5c41-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5c41-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5c41-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5c41-115">Not supported.</span></span>    |
|<span data-ttu-id="e5c41-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e5c41-116">Application</span></span> | <span data-ttu-id="e5c41-117">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5c41-117">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5c41-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5c41-118">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e5c41-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e5c41-119">Optional query parameters</span></span>
<span data-ttu-id="e5c41-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e5c41-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5c41-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5c41-121">Request headers</span></span>
| <span data-ttu-id="e5c41-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5c41-122">Header</span></span>         | <span data-ttu-id="e5c41-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e5c41-123">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="e5c41-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5c41-124">Authorization</span></span>  | <span data-ttu-id="e5c41-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5c41-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e5c41-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5c41-127">Content-Type</span></span>   | <span data-ttu-id="e5c41-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e5c41-128">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="e5c41-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5c41-129">Request body</span></span>
<span data-ttu-id="e5c41-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5c41-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5c41-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5c41-131">Response</span></span>

<span data-ttu-id="e5c41-132">В случае успешной работы этот метод возвращает код ответа 200 ОК и коллекцию [объектов driveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5c41-132">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5c41-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e5c41-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e5c41-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5c41-134">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="e5c41-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5c41-135">Response</span></span>
<span data-ttu-id="e5c41-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e5c41-136">Here is an example of the response.</span></span> <span data-ttu-id="e5c41-137">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e5c41-137">Note: The response object shown here might be shortened for readability.</span></span>
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