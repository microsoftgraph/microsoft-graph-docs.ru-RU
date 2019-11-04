---
title: Получение профиля
description: Получение свойств и связей объекта Profile.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b6d551ff4920a7e7c132cac532dd1c7a59f54604
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937821"
---
# <a name="get-profile"></a><span data-ttu-id="422c4-103">Получение профиля</span><span class="sxs-lookup"><span data-stu-id="422c4-103">Get profile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="422c4-104">Получение свойств и связей объекта [Profile](../resources/profile.md) для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="422c4-104">Retrieve the properties and relationships of a [profile](../resources/profile.md) object for a given user.</span></span>

## <a name="permissions"></a><span data-ttu-id="422c4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="422c4-105">Permissions</span></span>

<span data-ttu-id="422c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="422c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="422c4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="422c4-108">Permission type</span></span>                        | <span data-ttu-id="422c4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="422c4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="422c4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="422c4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="422c4-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="422c4-111">Not supported.</span></span>                              |
| <span data-ttu-id="422c4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="422c4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="422c4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="422c4-113">Not supported.</span></span>                              |
| <span data-ttu-id="422c4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="422c4-114">Application</span></span>                            | <span data-ttu-id="422c4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="422c4-115">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="422c4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="422c4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="422c4-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="422c4-117">Optional query parameters</span></span>

<span data-ttu-id="422c4-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="422c4-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="422c4-119">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="422c4-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="422c4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="422c4-120">Request headers</span></span>

| <span data-ttu-id="422c4-121">Имя</span><span class="sxs-lookup"><span data-stu-id="422c4-121">Name</span></span>           |<span data-ttu-id="422c4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="422c4-122">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="422c4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="422c4-123">Authorization</span></span>  | <span data-ttu-id="422c4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="422c4-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="422c4-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="422c4-126">Content-Type</span></span>   | <span data-ttu-id="422c4-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="422c4-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="422c4-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="422c4-129">Request body</span></span>

<span data-ttu-id="422c4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="422c4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="422c4-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="422c4-131">Response</span></span>

<span data-ttu-id="422c4-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [Profile](../resources/profile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="422c4-132">If successful, this method returns a `200 OK` response code and the requested [profile](../resources/profile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="422c4-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="422c4-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="422c4-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="422c4-134">Request</span></span>

<span data-ttu-id="422c4-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="422c4-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_profile"
}-->

```http
GET https://graph.microsoft.com/beta/me/profile
```

### <a name="response"></a><span data-ttu-id="422c4-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="422c4-136">Response</span></span>

<span data-ttu-id="422c4-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="422c4-137">The following is an example of the response.</span></span>

> <span data-ttu-id="422c4-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="422c4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get profile",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->