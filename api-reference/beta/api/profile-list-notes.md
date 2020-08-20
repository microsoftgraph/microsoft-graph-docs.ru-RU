---
title: Перечисление заметок
description: Получение personAnnotations из свойства навигации "заметки".
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a6cb5eecdd6d779ed89cde263135def3f682c12f
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819400"
---
# <a name="list-notes"></a><span data-ttu-id="09109-103">Перечисление заметок</span><span class="sxs-lookup"><span data-stu-id="09109-103">List notes</span></span>
<span data-ttu-id="09109-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09109-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="09109-105">Получение списка объектов [personAnnotation](../resources/personinterest.md) из профиля [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="09109-105">Retrieve a list of [personAnnotation](../resources/personinterest.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="09109-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09109-106">Permissions</span></span>

<span data-ttu-id="09109-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09109-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09109-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09109-109">Permission type</span></span>                        | <span data-ttu-id="09109-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09109-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="09109-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09109-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="09109-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09109-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="09109-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09109-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09109-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09109-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="09109-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="09109-115">Application</span></span>                            | <span data-ttu-id="09109-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09109-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="09109-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09109-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/notes
GET /users/{id | userPrincipalName}/profile/notes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09109-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="09109-118">Optional query parameters</span></span>

<span data-ttu-id="09109-119">Этот метод поддерживает указанные ниже параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="09109-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="09109-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="09109-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="09109-121">Имя</span><span class="sxs-lookup"><span data-stu-id="09109-121">Name</span></span>            |<span data-ttu-id="09109-122">Значение</span><span class="sxs-lookup"><span data-stu-id="09109-122">Value</span></span>    |<span data-ttu-id="09109-123">Описание</span><span class="sxs-lookup"><span data-stu-id="09109-123">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="09109-124">$filter</span><span class="sxs-lookup"><span data-stu-id="09109-124">$filter</span></span>         |<span data-ttu-id="09109-125">string</span><span class="sxs-lookup"><span data-stu-id="09109-125">string</span></span>   |<span data-ttu-id="09109-126">Возвращает число в отклике только тех объектов, которые содержат указанные условия.</span><span class="sxs-lookup"><span data-stu-id="09109-126">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="09109-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="09109-127">$orderby</span></span>        |<span data-ttu-id="09109-128">строка</span><span class="sxs-lookup"><span data-stu-id="09109-128">string</span></span>   |<span data-ttu-id="09109-129">По умолчанию объекты в ответе сортируются по их значению createdDateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="09109-129">By default the objects in the response are sorted by their createdDateTime value in a query.</span></span> <span data-ttu-id="09109-130">Этот порядок ответа можно изменить с помощью *$orderby* параметра.</span><span class="sxs-lookup"><span data-stu-id="09109-130">You can change the order of the of the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="09109-131">$select</span><span class="sxs-lookup"><span data-stu-id="09109-131">$select</span></span>         |<span data-ttu-id="09109-132">string</span><span class="sxs-lookup"><span data-stu-id="09109-132">string</span></span>   |<span data-ttu-id="09109-p104">Список разделенных запятыми свойств, которые необходимо включить в отклик. Для оптимизации производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="09109-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="09109-135">$skip</span><span class="sxs-lookup"><span data-stu-id="09109-135">$skip</span></span>           |<span data-ttu-id="09109-136">int</span><span class="sxs-lookup"><span data-stu-id="09109-136">int</span></span>      |<span data-ttu-id="09109-137">Пропуск первых n результатов; это удобно при разбиении результатов на страницы.</span><span class="sxs-lookup"><span data-stu-id="09109-137">Skip the first n results, useful for paging.</span></span>                                                                                                                                |
|<span data-ttu-id="09109-138">$top</span><span class="sxs-lookup"><span data-stu-id="09109-138">$top</span></span>            |<span data-ttu-id="09109-139">int</span><span class="sxs-lookup"><span data-stu-id="09109-139">int</span></span>      |<span data-ttu-id="09109-140">Количество возвращаемых результатов.</span><span class="sxs-lookup"><span data-stu-id="09109-140">Number of results to be returned.</span></span>                                                                                                                                           |

## <a name="request-headers"></a><span data-ttu-id="09109-141">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="09109-141">Request headers</span></span>
|<span data-ttu-id="09109-142">Имя</span><span class="sxs-lookup"><span data-stu-id="09109-142">Name</span></span>|<span data-ttu-id="09109-143">Описание</span><span class="sxs-lookup"><span data-stu-id="09109-143">Description</span></span>|
|:---|:---|
|<span data-ttu-id="09109-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09109-144">Authorization</span></span>|<span data-ttu-id="09109-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09109-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="09109-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09109-147">Request body</span></span>
<span data-ttu-id="09109-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09109-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09109-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="09109-149">Response</span></span>

<span data-ttu-id="09109-150">При успешном выполнении этот метод возвращает `200 OK` код отклика и коллекцию [объектов personAnnotation](../resources/personannotation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="09109-150">If successful, this method returns a `200 OK` response code and a collection of [personAnnotation](../resources/personannotation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="09109-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="09109-151">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="09109-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="09109-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_notes"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/notes
```
# <a name="c"></a>[<span data-ttu-id="09109-153">C#</span><span class="sxs-lookup"><span data-stu-id="09109-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-notes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09109-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09109-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-notes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09109-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09109-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-notes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="09109-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="09109-156">Response</span></span>
<span data-ttu-id="09109-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="09109-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.personAnnotation)"
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
      "detail": {
        "contentType": "text",
        "content": "I am originally from Australia, but grew up in Moscow."
      },
      "displayName": "About Me"
    }
  ]
}
```

