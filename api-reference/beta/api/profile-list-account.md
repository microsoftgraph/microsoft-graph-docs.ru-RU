---
title: Учетная запись списка
description: Получение списка объектов усераккаунтинформатион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: be248f9555fbc7a5dccf8771668ffbb58b51c853
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937814"
---
# <a name="list-account"></a><span data-ttu-id="5b2d7-103">Учетная запись списка</span><span class="sxs-lookup"><span data-stu-id="5b2d7-103">List account</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b2d7-104">Получает свойства, связанные с учетной записью пользователя, из [профиля](../resources/profile.md).</span><span class="sxs-lookup"><span data-stu-id="5b2d7-104">Retrieves properties related to the user's account from the [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b2d7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b2d7-105">Permissions</span></span>

<span data-ttu-id="5b2d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b2d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b2d7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b2d7-108">Permission type</span></span>                        | <span data-ttu-id="5b2d7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b2d7-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="5b2d7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b2d7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b2d7-111">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5b2d7-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5b2d7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b2d7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b2d7-113">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5b2d7-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="5b2d7-114">Application</span><span class="sxs-lookup"><span data-stu-id="5b2d7-114">Application</span></span>                            | <span data-ttu-id="5b2d7-115">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5b2d7-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="5b2d7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b2d7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/account
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b2d7-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5b2d7-117">Optional query parameters</span></span>

<span data-ttu-id="5b2d7-118">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5b2d7-118">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="5b2d7-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5b2d7-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="5b2d7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5b2d7-120">Name</span></span>            |<span data-ttu-id="5b2d7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5b2d7-121">Value</span></span>    |<span data-ttu-id="5b2d7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5b2d7-122">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="5b2d7-123">$filter</span><span class="sxs-lookup"><span data-stu-id="5b2d7-123">$filter</span></span>         |<span data-ttu-id="5b2d7-124">string</span><span class="sxs-lookup"><span data-stu-id="5b2d7-124">string</span></span>   |<span data-ttu-id="5b2d7-125">Разрешает отклик только на те объекты, которые содержат заданные условия.</span><span class="sxs-lookup"><span data-stu-id="5b2d7-125">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="5b2d7-126">$orderby</span><span class="sxs-lookup"><span data-stu-id="5b2d7-126">$orderby</span></span>        |<span data-ttu-id="5b2d7-127">строка</span><span class="sxs-lookup"><span data-stu-id="5b2d7-127">string</span></span>   |<span data-ttu-id="5b2d7-128">По умолчанию объекты в отклике сортируются по значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="5b2d7-128">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="5b2d7-129">Вы можете изменить порядок ответа с помощью параметра *$OrderBy* .</span><span class="sxs-lookup"><span data-stu-id="5b2d7-129">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="5b2d7-130">$select</span><span class="sxs-lookup"><span data-stu-id="5b2d7-130">$select</span></span>         |<span data-ttu-id="5b2d7-131">string</span><span class="sxs-lookup"><span data-stu-id="5b2d7-131">string</span></span>   |<span data-ttu-id="5b2d7-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="5b2d7-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="5b2d7-134">$skip</span><span class="sxs-lookup"><span data-stu-id="5b2d7-134">$skip</span></span>           |<span data-ttu-id="5b2d7-135">int</span><span class="sxs-lookup"><span data-stu-id="5b2d7-135">int</span></span>      |<span data-ttu-id="5b2d7-136">Пропустите первые n результатов, которые удобно использовать для разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="5b2d7-136">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="5b2d7-137">$top</span><span class="sxs-lookup"><span data-stu-id="5b2d7-137">$top</span></span>            |<span data-ttu-id="5b2d7-138">int</span><span class="sxs-lookup"><span data-stu-id="5b2d7-138">int</span></span>      |<span data-ttu-id="5b2d7-139">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="5b2d7-139">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="5b2d7-140">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5b2d7-140">Request headers</span></span>

| <span data-ttu-id="5b2d7-141">Имя</span><span class="sxs-lookup"><span data-stu-id="5b2d7-141">Name</span></span>           |<span data-ttu-id="5b2d7-142">Описание</span><span class="sxs-lookup"><span data-stu-id="5b2d7-142">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="5b2d7-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b2d7-143">Authorization</span></span>  | <span data-ttu-id="5b2d7-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b2d7-p105">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="5b2d7-146">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5b2d7-146">Content-Type</span></span>   | <span data-ttu-id="5b2d7-p106">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b2d7-p106">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b2d7-149">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b2d7-149">Request body</span></span>

<span data-ttu-id="5b2d7-150">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b2d7-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b2d7-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="5b2d7-151">Response</span></span>

<span data-ttu-id="5b2d7-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усераккаунтинформатион](../resources/useraccountinformation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5b2d7-152">If successful, this method returns a `200 OK` response code and a collection of [userAccountInformation](../resources/useraccountinformation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b2d7-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="5b2d7-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b2d7-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b2d7-154">Request</span></span>

<span data-ttu-id="5b2d7-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b2d7-155">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_account"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile/account
```

### <a name="response"></a><span data-ttu-id="5b2d7-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b2d7-156">Response</span></span>

<span data-ttu-id="5b2d7-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b2d7-157">The following is an example of the response.</span></span>

> <span data-ttu-id="5b2d7-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b2d7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "ageGroup": "ageGroup-value",
      "countryCode": "countryCode-value",
      "preferredLanguageTag": {
        "locale": "locale-value",
        "displayName": "displayName-value"
      },
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List account",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->