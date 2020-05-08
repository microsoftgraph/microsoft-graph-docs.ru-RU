---
title: Получение профиля
description: Получение свойств и связей объекта Profile.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fd6c68f79ffb417b12eb1f8e28d874f4461fb24e
ms.sourcegitcommit: 5d4bf35774eba6de21f4252b46f7e9d8f64a517f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/08/2020
ms.locfileid: "44168558"
---
# <a name="get-profile"></a><span data-ttu-id="61752-103">Получение профиля</span><span class="sxs-lookup"><span data-stu-id="61752-103">Get profile</span></span>

<span data-ttu-id="61752-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61752-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61752-105">Получение свойств и связей объекта [Profile](../resources/profile.md) для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="61752-105">Retrieve the properties and relationships of a [profile](../resources/profile.md) object for a given user.</span></span>

<span data-ttu-id="61752-106">Ресурс **Profile** предоставляет различные расширенные свойства, которые могут быть описательными для пользователя как [отношения](../resources/profile.md#relationships), например юбилеи и действия по образованию.</span><span class="sxs-lookup"><span data-stu-id="61752-106">The **profile** resource exposes various rich properties that are descriptive of the user as [relationships](../resources/profile.md#relationships), for example, anniversaries and education activities.</span></span> <span data-ttu-id="61752-107">Чтобы получить одно из этих свойств навигации, используйте соответствующий метод GET для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="61752-107">To get one of these navigation properties, use the corresponding GET method on that property.</span></span> <span data-ttu-id="61752-108">Просмотрите [методы](../resources/profile.md) , предоставляемые **профилем**.</span><span class="sxs-lookup"><span data-stu-id="61752-108">See the [methods](../resources/profile.md) exposed by **profile**.</span></span>

## <a name="permissions"></a><span data-ttu-id="61752-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61752-109">Permissions</span></span>

<span data-ttu-id="61752-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61752-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61752-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61752-112">Permission type</span></span>                        | <span data-ttu-id="61752-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61752-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="61752-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61752-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="61752-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61752-115">Not supported.</span></span>                              |
| <span data-ttu-id="61752-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61752-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61752-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61752-117">Not supported.</span></span>                              |
| <span data-ttu-id="61752-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="61752-118">Application</span></span>                            | <span data-ttu-id="61752-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61752-119">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="61752-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61752-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="61752-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="61752-121">Optional query parameters</span></span>

<span data-ttu-id="61752-122">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="61752-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="61752-123">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="61752-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="61752-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61752-124">Request headers</span></span>

| <span data-ttu-id="61752-125">Имя</span><span class="sxs-lookup"><span data-stu-id="61752-125">Name</span></span>           |<span data-ttu-id="61752-126">Описание</span><span class="sxs-lookup"><span data-stu-id="61752-126">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="61752-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61752-127">Authorization</span></span>  | <span data-ttu-id="61752-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61752-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="61752-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="61752-130">Content-Type</span></span>   | <span data-ttu-id="61752-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61752-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61752-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61752-133">Request body</span></span>

<span data-ttu-id="61752-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="61752-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="61752-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="61752-135">Response</span></span>

<span data-ttu-id="61752-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [Profile](../resources/profile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="61752-136">If successful, this method returns a `200 OK` response code and the requested [profile](../resources/profile.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="61752-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="61752-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="61752-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="61752-138">Request</span></span>

<span data-ttu-id="61752-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61752-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="61752-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="61752-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile
```
# <a name="c"></a>[<span data-ttu-id="61752-141">C#</span><span class="sxs-lookup"><span data-stu-id="61752-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61752-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61752-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61752-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61752-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="61752-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="61752-144">Response</span></span>

<span data-ttu-id="61752-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="61752-145">The following is an example of the response.</span></span>

> <span data-ttu-id="61752-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="61752-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
