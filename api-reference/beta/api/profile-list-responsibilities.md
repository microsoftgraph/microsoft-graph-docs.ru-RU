---
title: Список обязанностей
description: Получите personResponsibilities из свойства навигации об обязанностях.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c94ea1d4ef1e7014841b71876c927ce6fca952af
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292065"
---
# <a name="list-responsibilities"></a><span data-ttu-id="3b519-103">Список обязанностей</span><span class="sxs-lookup"><span data-stu-id="3b519-103">List responsibilities</span></span>
<span data-ttu-id="3b519-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b519-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3b519-105">Получить список объектов [personResponsibility](../resources/personresponsibility.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="3b519-105">Retrieve a list of [personResponsibility](../resources/personresponsibility.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3b519-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b519-106">Permissions</span></span>

<span data-ttu-id="3b519-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b519-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3b519-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b519-109">Permission type</span></span>                        | <span data-ttu-id="3b519-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b519-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="3b519-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b519-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3b519-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b519-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="3b519-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b519-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b519-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b519-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="3b519-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b519-115">Application</span></span>                            | <span data-ttu-id="3b519-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b519-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="3b519-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b519-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/responsibilities
GET /users/{id | userPrincipalName}/responsibilities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b519-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3b519-118">Optional query parameters</span></span>

<span data-ttu-id="3b519-119">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3b519-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="3b519-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3b519-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="3b519-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3b519-121">Name</span></span>            |<span data-ttu-id="3b519-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3b519-122">Value</span></span>    |<span data-ttu-id="3b519-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3b519-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="3b519-124">$filter</span><span class="sxs-lookup"><span data-stu-id="3b519-124">$filter</span></span>         |<span data-ttu-id="3b519-125">string</span><span class="sxs-lookup"><span data-stu-id="3b519-125">string</span></span>   |<span data-ttu-id="3b519-126">Ограничивает отклик только теми объектами, которые содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="3b519-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="3b519-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="3b519-127">$orderby</span></span>        |<span data-ttu-id="3b519-128">строка</span><span class="sxs-lookup"><span data-stu-id="3b519-128">string</span></span>   |<span data-ttu-id="3b519-129">По умолчанию объекты в отклике сортируются по их значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="3b519-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="3b519-130">Вы можете изменить порядок ответа с помощью параметра *$orderby.*</span><span class="sxs-lookup"><span data-stu-id="3b519-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="3b519-131">$select</span><span class="sxs-lookup"><span data-stu-id="3b519-131">$select</span></span>         |<span data-ttu-id="3b519-132">string</span><span class="sxs-lookup"><span data-stu-id="3b519-132">string</span></span>   |<span data-ttu-id="3b519-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="3b519-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="3b519-135">$skip</span><span class="sxs-lookup"><span data-stu-id="3b519-135">$skip</span></span>           |<span data-ttu-id="3b519-136">int</span><span class="sxs-lookup"><span data-stu-id="3b519-136">int</span></span>      |<span data-ttu-id="3b519-137">Пропустите первые n результаты, полезные для разгибания по простоям.</span><span class="sxs-lookup"><span data-stu-id="3b519-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="3b519-138">$top</span><span class="sxs-lookup"><span data-stu-id="3b519-138">$top</span></span>            |<span data-ttu-id="3b519-139">int</span><span class="sxs-lookup"><span data-stu-id="3b519-139">int</span></span>      |<span data-ttu-id="3b519-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="3b519-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="3b519-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3b519-141">Request headers</span></span>
|<span data-ttu-id="3b519-142">Имя</span><span class="sxs-lookup"><span data-stu-id="3b519-142">Name</span></span>|<span data-ttu-id="3b519-143">Описание</span><span class="sxs-lookup"><span data-stu-id="3b519-143">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3b519-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b519-144">Authorization</span></span>|<span data-ttu-id="3b519-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b519-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b519-147">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3b519-147">Request body</span></span>
<span data-ttu-id="3b519-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3b519-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b519-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b519-149">Response</span></span>

<span data-ttu-id="3b519-150">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [personResponsibility](../resources/personresponsibility.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b519-150">If successful, this method returns a `200 OK` response code and a collection of [personResponsibility](../resources/personresponsibility.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3b519-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="3b519-151">Examples</span></span>

<!-- {
  "blockType": "request",
  "name": "get_responsibilities_from_profile"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/responsibilities
```

### <a name="response"></a><span data-ttu-id="3b519-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b519-152">Response</span></span>
<span data-ttu-id="3b519-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3b519-153">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.personResponsibility)",
  "isCollection": true
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
      "source": null,
      "description": "Member of the Microsoft API Council",
      "displayName": "API Council",
      "webUrl": null,
      "collaborationTags": [
        "askMeAbout"
      ]
    }
  ]
}
```


