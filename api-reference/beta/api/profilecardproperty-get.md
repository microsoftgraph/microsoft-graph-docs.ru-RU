---
title: Получение Профилекардпроперти
description: Получение свойств и связей объекта Профилекардпроперти.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c9a4f4c1ca9cc71f496b577f24771ffdb058bb2d
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080793"
---
# <a name="get-profilecardproperty"></a><span data-ttu-id="72d2f-103">Получение Профилекардпроперти</span><span class="sxs-lookup"><span data-stu-id="72d2f-103">Get profileCardProperty</span></span>

<span data-ttu-id="72d2f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72d2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72d2f-105">Получение свойств и связей объекта [профилекардпроперти](../resources/profilecardproperty.md) , содержащего настройки карты профилей, существующие в организации Microsoft 365 для данного поля.</span><span class="sxs-lookup"><span data-stu-id="72d2f-105">Retrieve the properties and relationships of a [profileCardProperty](../resources/profilecardproperty.md) entity, which contains the profile card customizations that exist in your Microsoft 365 organization for a given field.</span></span> <span data-ttu-id="72d2f-106">Профилекардпроперти определяется свойством **директорипропертинаме** .</span><span class="sxs-lookup"><span data-stu-id="72d2f-106">The profileCardProperty is identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="72d2f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72d2f-107">Permissions</span></span>

<span data-ttu-id="72d2f-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="72d2f-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="72d2f-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72d2f-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72d2f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72d2f-110">Permission type</span></span>                        | <span data-ttu-id="72d2f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72d2f-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="72d2f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72d2f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="72d2f-113">User. Read, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="72d2f-113">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="72d2f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72d2f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72d2f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72d2f-115">Not supported.</span></span>                              |
| <span data-ttu-id="72d2f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72d2f-116">Application</span></span>                            | <span data-ttu-id="72d2f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72d2f-117">Not supported.</span></span>                              |

><span data-ttu-id="72d2f-118">**Примечание:** Для этой операции с делегированными разрешениями необходимо, чтобы вошедшего в систему пользователя была назначена роль администратора клиента или роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="72d2f-118">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="72d2f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72d2f-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings/profileCardProperties/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72d2f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="72d2f-120">Optional query parameters</span></span>

<span data-ttu-id="72d2f-121">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="72d2f-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="72d2f-122">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="72d2f-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="72d2f-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72d2f-123">Request headers</span></span>

| <span data-ttu-id="72d2f-124">Имя</span><span class="sxs-lookup"><span data-stu-id="72d2f-124">Name</span></span>      |<span data-ttu-id="72d2f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="72d2f-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72d2f-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72d2f-126">Authorization</span></span> | <span data-ttu-id="72d2f-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="72d2f-127">Bearer {token}.</span></span> <span data-ttu-id="72d2f-128">Required.</span><span class="sxs-lookup"><span data-stu-id="72d2f-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72d2f-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="72d2f-129">Request body</span></span>

<span data-ttu-id="72d2f-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72d2f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72d2f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="72d2f-131">Response</span></span>

<span data-ttu-id="72d2f-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [профилекардпроперти](../resources/profilecardproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72d2f-132">If successful, this method returns a `200 OK` response code and the requested [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72d2f-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="72d2f-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72d2f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="72d2f-134">Request</span></span>

<span data-ttu-id="72d2f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72d2f-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72d2f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="72d2f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_profilecardproperty"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/settings/profileCardProperties/{id}
```
# <a name="c"></a>[<span data-ttu-id="72d2f-137">C#</span><span class="sxs-lookup"><span data-stu-id="72d2f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-profilecardproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72d2f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72d2f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72d2f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72d2f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-profilecardproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="72d2f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="72d2f-140">Response</span></span>

<span data-ttu-id="72d2f-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="72d2f-141">The following is an example of the response.</span></span>

> <span data-ttu-id="72d2f-142">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="72d2f-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="72d2f-143">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="72d2f-143">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "directoryPropertyName": "CustomAttribute1",
  "annotations": [
    {
      "displayName": "Cost Center",
      "localizations": [
        {
          "languageTag": "ru-RU",
          "displayName": "центр затрат"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get profileCardProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
