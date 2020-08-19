---
title: Перечисление телефонов
description: Получение списка объектов Итемфоне.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a7a9e6af49a76d985fa4e7b16fe505d29ecf30c7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810666"
---
# <a name="list-phones"></a><span data-ttu-id="c8e98-103">Перечисление телефонов</span><span class="sxs-lookup"><span data-stu-id="c8e98-103">List phones</span></span>

<span data-ttu-id="c8e98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8e98-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8e98-105">Получение списка объектов [итемфоне](../resources/itemphone.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="c8e98-105">Retrieve a list of [itemPhone](../resources/itemphone.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c8e98-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c8e98-106">Permissions</span></span>

<span data-ttu-id="c8e98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8e98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8e98-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8e98-109">Permission type</span></span>                        | <span data-ttu-id="c8e98-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8e98-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="c8e98-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8e98-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8e98-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c8e98-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="c8e98-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8e98-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8e98-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c8e98-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="c8e98-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c8e98-115">Application</span></span>                            | <span data-ttu-id="c8e98-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c8e98-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="c8e98-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8e98-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/phones
GET /user/{id | userPrincipalName}/profile/phones
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8e98-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c8e98-118">Optional query parameters</span></span>

<span data-ttu-id="c8e98-119">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c8e98-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="c8e98-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c8e98-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="c8e98-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c8e98-121">Name</span></span>            |<span data-ttu-id="c8e98-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c8e98-122">Value</span></span>    |<span data-ttu-id="c8e98-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c8e98-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="c8e98-124">$filter</span><span class="sxs-lookup"><span data-stu-id="c8e98-124">$filter</span></span>         |<span data-ttu-id="c8e98-125">string</span><span class="sxs-lookup"><span data-stu-id="c8e98-125">string</span></span>   |<span data-ttu-id="c8e98-126">Разрешает отклик только на те объекты, которые содержат заданные условия.</span><span class="sxs-lookup"><span data-stu-id="c8e98-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="c8e98-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="c8e98-127">$orderby</span></span>        |<span data-ttu-id="c8e98-128">строка</span><span class="sxs-lookup"><span data-stu-id="c8e98-128">string</span></span>   |<span data-ttu-id="c8e98-129">По умолчанию объекты в отклике сортируются по значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="c8e98-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="c8e98-130">Вы можете изменить порядок ответа с помощью параметра *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="c8e98-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="c8e98-131">$select</span><span class="sxs-lookup"><span data-stu-id="c8e98-131">$select</span></span>         |<span data-ttu-id="c8e98-132">string</span><span class="sxs-lookup"><span data-stu-id="c8e98-132">string</span></span>   |<span data-ttu-id="c8e98-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="c8e98-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="c8e98-135">$skip</span><span class="sxs-lookup"><span data-stu-id="c8e98-135">$skip</span></span>           |<span data-ttu-id="c8e98-136">int</span><span class="sxs-lookup"><span data-stu-id="c8e98-136">int</span></span>      |<span data-ttu-id="c8e98-137">Пропустите первые n результатов, которые удобно использовать для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="c8e98-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="c8e98-138">$top</span><span class="sxs-lookup"><span data-stu-id="c8e98-138">$top</span></span>            |<span data-ttu-id="c8e98-139">int</span><span class="sxs-lookup"><span data-stu-id="c8e98-139">int</span></span>      |<span data-ttu-id="c8e98-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="c8e98-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="c8e98-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c8e98-141">Request headers</span></span>

|<span data-ttu-id="c8e98-142">Имя</span><span class="sxs-lookup"><span data-stu-id="c8e98-142">Name</span></span>|<span data-ttu-id="c8e98-143">Описание</span><span class="sxs-lookup"><span data-stu-id="c8e98-143">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c8e98-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8e98-144">Authorization</span></span>|<span data-ttu-id="c8e98-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8e98-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8e98-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8e98-147">Request body</span></span>

<span data-ttu-id="c8e98-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8e98-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8e98-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8e98-149">Response</span></span>

<span data-ttu-id="c8e98-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [итемфоне](../resources/itemphone.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8e98-150">If successful, this method returns a `200 OK` response code and a collection of [itemPhone](../resources/itemphone.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8e98-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="c8e98-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c8e98-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8e98-152">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_itemphone"
}
-->

``` http
GET https://graph.microsoft.com/beta/me/profile/phones
```


### <a name="response"></a><span data-ttu-id="c8e98-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8e98-153">Response</span></span>
<span data-ttu-id="c8e98-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c8e98-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.itemPhone)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
      "allowedAudiences": "organization",
      "inference": null,
      "createdDateTime": "2020-07-06T06:34:12.2294868Z",
      "createdBy": {
        "application": null,
        "device": null,
        "user": {
          "displayName": "Innocenty Popov",
          "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
        }
      },
      "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
      "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
          "displayName": "Innocenty Popov",
          "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
        }
      },
      "displayName": "Car Phone",
      "type": "other",
      "number": "+7 499 342 22 13"
    }
  ]
}
```
