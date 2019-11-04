---
title: Перечисление имен
description: Получение списка объектов PersonName из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5c13b3ee7454c8b8f0061aafbd9d0bebea6da94a
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937772"
---
# <a name="list-names"></a><span data-ttu-id="936a3-103">Перечисление имен</span><span class="sxs-lookup"><span data-stu-id="936a3-103">List names</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="936a3-104">Получение списка объектов [PersonName](../resources/personname.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="936a3-104">Retrieve a list of [personName](../resources/personname.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="936a3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="936a3-105">Permissions</span></span>

<span data-ttu-id="936a3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="936a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="936a3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="936a3-108">Permission type</span></span>                        | <span data-ttu-id="936a3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="936a3-109">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="936a3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="936a3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="936a3-111">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="936a3-111">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="936a3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="936a3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="936a3-113">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="936a3-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="936a3-114">Application</span><span class="sxs-lookup"><span data-stu-id="936a3-114">Application</span></span>                            | <span data-ttu-id="936a3-115">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="936a3-115">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="936a3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="936a3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/names
```

## <a name="optional-query-parameters"></a><span data-ttu-id="936a3-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="936a3-117">Optional query parameters</span></span>

<span data-ttu-id="936a3-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="936a3-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="936a3-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="936a3-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="936a3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="936a3-120">Request headers</span></span>

| <span data-ttu-id="936a3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="936a3-121">Name</span></span>           |<span data-ttu-id="936a3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="936a3-122">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="936a3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="936a3-123">Authorization</span></span>  | <span data-ttu-id="936a3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="936a3-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="936a3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="936a3-126">Content-Type</span></span>   | <span data-ttu-id="936a3-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="936a3-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="936a3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="936a3-129">Request body</span></span> 

<span data-ttu-id="936a3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="936a3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="936a3-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="936a3-131">Response</span></span>

<span data-ttu-id="936a3-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [PersonName](../resources/personname.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="936a3-132">If successful, this method returns a `200 OK` response code and a collection of [personName](../resources/personname.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="936a3-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="936a3-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="936a3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="936a3-134">Request</span></span>

<span data-ttu-id="936a3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="936a3-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_names"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile/names
```

### <a name="response"></a><span data-ttu-id="936a3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="936a3-136">Response</span></span>

<span data-ttu-id="936a3-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="936a3-137">The following is an example of the response.</span></span>

> <span data-ttu-id="936a3-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="936a3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "displayName-value",
      "first": "first-value",
      "initials": "initials-value",
      "last": "last-value",
      "languageTag": "languageTag-value",
      "maiden": "maiden-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List names",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->