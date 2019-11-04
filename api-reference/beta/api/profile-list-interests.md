---
title: Список интересов
description: Получение списка объектов Персонинтерест.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1d6b31aca0f37de23d212497c72842d331201ffb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937788"
---
# <a name="list-interests"></a><span data-ttu-id="f2a48-103">Список интересов</span><span class="sxs-lookup"><span data-stu-id="f2a48-103">List interests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2a48-104">Получение списка объектов [персонинтерест](../resources/personinterest.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="f2a48-104">Retrieve a list of [personInterest](../resources/personinterest.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2a48-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2a48-105">Permissions</span></span>

<span data-ttu-id="f2a48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2a48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2a48-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2a48-108">Permission type</span></span>                        | <span data-ttu-id="f2a48-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2a48-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="f2a48-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2a48-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2a48-111">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f2a48-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f2a48-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2a48-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2a48-113">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f2a48-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f2a48-114">Application</span><span class="sxs-lookup"><span data-stu-id="f2a48-114">Application</span></span>                            | <span data-ttu-id="f2a48-115">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f2a48-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="f2a48-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2a48-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/interests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2a48-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2a48-117">Optional query parameters</span></span>

<span data-ttu-id="f2a48-118">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f2a48-118">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="f2a48-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f2a48-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="f2a48-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f2a48-120">Name</span></span>            |<span data-ttu-id="f2a48-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f2a48-121">Value</span></span>    |<span data-ttu-id="f2a48-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f2a48-122">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="f2a48-123">$filter</span><span class="sxs-lookup"><span data-stu-id="f2a48-123">$filter</span></span>         |<span data-ttu-id="f2a48-124">string</span><span class="sxs-lookup"><span data-stu-id="f2a48-124">string</span></span>   |<span data-ttu-id="f2a48-125">Разрешает отклик только на те объекты, которые содержат заданные условия.</span><span class="sxs-lookup"><span data-stu-id="f2a48-125">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="f2a48-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="f2a48-126">$orderby</span></span>        |<span data-ttu-id="f2a48-127">строка</span><span class="sxs-lookup"><span data-stu-id="f2a48-127">string</span></span>   |<span data-ttu-id="f2a48-128">По умолчанию объекты в отклике сортируются по значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="f2a48-128">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="f2a48-129">Вы можете изменить порядок ответа с помощью параметра *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="f2a48-129">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="f2a48-130">$select</span><span class="sxs-lookup"><span data-stu-id="f2a48-130">$select</span></span>         |<span data-ttu-id="f2a48-131">string</span><span class="sxs-lookup"><span data-stu-id="f2a48-131">string</span></span>   |<span data-ttu-id="f2a48-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="f2a48-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="f2a48-134">$skip</span><span class="sxs-lookup"><span data-stu-id="f2a48-134">$skip</span></span>           |<span data-ttu-id="f2a48-135">int</span><span class="sxs-lookup"><span data-stu-id="f2a48-135">int</span></span>      |<span data-ttu-id="f2a48-136">Пропустите первые n результатов, которые удобно использовать для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="f2a48-136">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="f2a48-137">$top</span><span class="sxs-lookup"><span data-stu-id="f2a48-137">$top</span></span>            |<span data-ttu-id="f2a48-138">int</span><span class="sxs-lookup"><span data-stu-id="f2a48-138">int</span></span>      |<span data-ttu-id="f2a48-139">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="f2a48-139">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="f2a48-140">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f2a48-140">Request headers</span></span>

| <span data-ttu-id="f2a48-141">Имя</span><span class="sxs-lookup"><span data-stu-id="f2a48-141">Name</span></span>           |<span data-ttu-id="f2a48-142">Описание</span><span class="sxs-lookup"><span data-stu-id="f2a48-142">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="f2a48-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2a48-143">Authorization</span></span>  | <span data-ttu-id="f2a48-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2a48-p105">Bearer {token}. Required.</span></span>   |


## <a name="request-body"></a><span data-ttu-id="f2a48-146">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2a48-146">Request body</span></span>

<span data-ttu-id="f2a48-147">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2a48-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2a48-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="f2a48-148">Response</span></span>

<span data-ttu-id="f2a48-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [персонинтерест](../resources/personinterest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f2a48-149">If successful, this method returns a `200 OK` response code and a collection of [personInterest](../resources/personinterest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2a48-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="f2a48-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2a48-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2a48-151">Request</span></span>

<span data-ttu-id="f2a48-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2a48-152">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_interests"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile/interests
```

### <a name="response"></a><span data-ttu-id="f2a48-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2a48-153">Response</span></span>

<span data-ttu-id="f2a48-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f2a48-154">The following is an example of the response.</span></span>

> <span data-ttu-id="f2a48-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2a48-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "categories": [
        "categories-value"
      ],
      "description": "description-value",
      "displayName": "displayName-value",
      "webUrl": "webUrl-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List interests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
