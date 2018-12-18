---
title: Список trendingAround
description: Вычисляемые представление, которое возвращает список элементов, прибора вокруг пользователя.
author: dkershaw10
ms.openlocfilehash: 2f2595cbaacc74053b23d6b26b64fb9a17e2924a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333833"
---
# <a name="list-trendingaround"></a><span data-ttu-id="5b714-103">Список trendingAround</span><span class="sxs-lookup"><span data-stu-id="5b714-103">List trendingAround</span></span>

> <span data-ttu-id="5b714-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5b714-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b714-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b714-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b714-106">Вычисляемые представление, которое возвращает список элементов, прибора вокруг пользователя.</span><span class="sxs-lookup"><span data-stu-id="5b714-106">Calculated insight that returns the list of items trending around a user.</span></span>

<span data-ttu-id="5b714-107">**Примечание:** Этот интерфейс API будет устаревшим и вместо нее [Прибора API](../resources/insights-trending.md).</span><span class="sxs-lookup"><span data-stu-id="5b714-107">**Note:** This API will be deprecated and replaced by the [Trending API](../resources/insights-trending.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b714-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b714-108">Permissions</span></span>
<span data-ttu-id="5b714-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b714-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b714-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b714-111">Permission type</span></span>      | <span data-ttu-id="5b714-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b714-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b714-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b714-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5b714-114">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b714-114">Sites.Read.All</span></span>    |
|<span data-ttu-id="5b714-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b714-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b714-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b714-116">Not supported.</span></span>    |
|<span data-ttu-id="5b714-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b714-117">Application</span></span> | <span data-ttu-id="5b714-118">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b714-118">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b714-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b714-119">HTTP request</span></span>
```http
GET /me/trendingAround
GET /users/{id | userPrincipalName}/trendingAround
GET /drive/root/createdByUser/trendingAround
GET /drive/root/lastModifiedByUser/trendingAround
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b714-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5b714-120">Optional query parameters</span></span>
<span data-ttu-id="5b714-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5b714-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b714-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b714-122">Request headers</span></span>
| <span data-ttu-id="5b714-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b714-123">Header</span></span>         | <span data-ttu-id="5b714-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5b714-124">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="5b714-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b714-125">Authorization</span></span>  | <span data-ttu-id="5b714-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b714-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5b714-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b714-128">Content-Type</span></span>   | <span data-ttu-id="5b714-129">application/json</span><span class="sxs-lookup"><span data-stu-id="5b714-129">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="5b714-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b714-130">Request body</span></span>
<span data-ttu-id="5b714-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b714-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b714-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b714-132">Response</span></span>

<span data-ttu-id="5b714-133">Если успешно завершена, этот метод возвращает 200 OK ответа код и коллекцию объектов [driveItem](../resources/driveitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5b714-133">If successful, this method returns a 200 OK response code and collection of [driveItem](../resources/driveitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b714-134">Пример</span><span class="sxs-lookup"><span data-stu-id="5b714-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b714-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b714-135">Request</span></span>
```http
GET https://graph.microsoft.com/beta/me/trendingAround
```
##### <a name="response"></a><span data-ttu-id="5b714-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b714-136">Response</span></span>
<span data-ttu-id="5b714-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5b714-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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