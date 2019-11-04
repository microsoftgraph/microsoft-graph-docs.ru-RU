---
title: Получение Итемфоне
description: Получение свойств и связей объекта итемфоне.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 4dd38709ddcc99d10827f9362b34e6100531fb29
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938438"
---
# <a name="get-itemphonenumber"></a><span data-ttu-id="216c9-103">Получение Итемфоненумбер</span><span class="sxs-lookup"><span data-stu-id="216c9-103">Get itemPhoneNumber</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="216c9-104">Получение свойств и связей объекта [итемфоне](../resources/itemphone.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="216c9-104">Retrieve the properties and relationships of an [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="216c9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="216c9-105">Permissions</span></span>

<span data-ttu-id="216c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="216c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="216c9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="216c9-108">Permission type</span></span>                        | <span data-ttu-id="216c9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="216c9-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="216c9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="216c9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="216c9-111">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="216c9-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="216c9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="216c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="216c9-113">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="216c9-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="216c9-114">Application</span><span class="sxs-lookup"><span data-stu-id="216c9-114">Application</span></span>                            | <span data-ttu-id="216c9-115">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="216c9-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="216c9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="216c9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/phones/{id} 
```

## <a name="optional-query-parameters"></a><span data-ttu-id="216c9-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="216c9-117">Optional query parameters</span></span>

<span data-ttu-id="216c9-118">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="216c9-118">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="216c9-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="216c9-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="216c9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="216c9-120">Name</span></span>            |<span data-ttu-id="216c9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="216c9-121">Value</span></span>    |<span data-ttu-id="216c9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="216c9-122">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="216c9-123">$filter</span><span class="sxs-lookup"><span data-stu-id="216c9-123">$filter</span></span>         |<span data-ttu-id="216c9-124">string</span><span class="sxs-lookup"><span data-stu-id="216c9-124">string</span></span>   |<span data-ttu-id="216c9-125">Разрешает отклик только на те объекты, которые содержат заданные условия.</span><span class="sxs-lookup"><span data-stu-id="216c9-125">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="216c9-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="216c9-126">$orderby</span></span>        |<span data-ttu-id="216c9-127">строка</span><span class="sxs-lookup"><span data-stu-id="216c9-127">string</span></span>   |<span data-ttu-id="216c9-128">По умолчанию объекты в отклике сортируются по значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="216c9-128">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="216c9-129">Вы можете изменить порядок ответа с помощью параметра *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="216c9-129">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="216c9-130">$select</span><span class="sxs-lookup"><span data-stu-id="216c9-130">$select</span></span>         |<span data-ttu-id="216c9-131">string</span><span class="sxs-lookup"><span data-stu-id="216c9-131">string</span></span>   |<span data-ttu-id="216c9-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="216c9-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="216c9-134">$skip</span><span class="sxs-lookup"><span data-stu-id="216c9-134">$skip</span></span>           |<span data-ttu-id="216c9-135">int</span><span class="sxs-lookup"><span data-stu-id="216c9-135">int</span></span>      |<span data-ttu-id="216c9-136">Пропустите первые n результатов, которые удобно использовать для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="216c9-136">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="216c9-137">$top</span><span class="sxs-lookup"><span data-stu-id="216c9-137">$top</span></span>            |<span data-ttu-id="216c9-138">int</span><span class="sxs-lookup"><span data-stu-id="216c9-138">int</span></span>      |<span data-ttu-id="216c9-139">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="216c9-139">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="216c9-140">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="216c9-140">Request headers</span></span>

| <span data-ttu-id="216c9-141">Имя</span><span class="sxs-lookup"><span data-stu-id="216c9-141">Name</span></span>           |<span data-ttu-id="216c9-142">Описание</span><span class="sxs-lookup"><span data-stu-id="216c9-142">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="216c9-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="216c9-143">Authorization</span></span>  | <span data-ttu-id="216c9-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="216c9-p105">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="216c9-146">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="216c9-146">Request body</span></span>

<span data-ttu-id="216c9-147">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="216c9-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="216c9-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="216c9-148">Response</span></span>

<span data-ttu-id="216c9-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [итемфоне](../resources/itemphone.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="216c9-149">If successful, this method returns a `200 OK` response code and the requested [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="216c9-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="216c9-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="216c9-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="216c9-151">Request</span></span>

<span data-ttu-id="216c9-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="216c9-152">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_itemphone"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile/phones/{id}
```

### <a name="response"></a><span data-ttu-id="216c9-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="216c9-153">Response</span></span>

<span data-ttu-id="216c9-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="216c9-154">The following is an example of the response.</span></span>

> <span data-ttu-id="216c9-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="216c9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get itemPhone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
