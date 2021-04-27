---
title: Get organizationSettings
description: Извлечение свойств и связей объекта organizationSettings.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 53bf7e03d56ad949683b0c363af3d4aa017502d6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052070"
---
# <a name="get-organizationsettings"></a><span data-ttu-id="5f521-103">Get organizationSettings</span><span class="sxs-lookup"><span data-stu-id="5f521-103">Get organizationSettings</span></span>

<span data-ttu-id="5f521-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f521-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f521-105">Извлечение свойств и связей объекта [organizationSettings,](../resources/organizationsettings.md) включая **profileCardProperties.**</span><span class="sxs-lookup"><span data-stu-id="5f521-105">Retrieve the properties and relationships of an [organizationSettings](../resources/organizationsettings.md) object, including **profileCardProperties**.</span></span>

<span data-ttu-id="5f521-106">Эта операция не возвращает [itemInsightsSettings](../resources/iteminsightssettings.md) через **свойство навигации itemInsights.**</span><span class="sxs-lookup"><span data-stu-id="5f521-106">This operation does not return [itemInsightsSettings](../resources/iteminsightssettings.md) through the **itemInsights** navigation property.</span></span> <span data-ttu-id="5f521-107">Вместо [этого используйте get itemInsightsSettings.](iteminsightssettings-get.md)</span><span class="sxs-lookup"><span data-stu-id="5f521-107">Use [get itemInsightsSettings](iteminsightssettings-get.md) instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f521-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f521-108">Permissions</span></span>

<span data-ttu-id="5f521-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f521-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5f521-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f521-111">Permission type</span></span>                        | <span data-ttu-id="5f521-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f521-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5f521-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f521-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f521-114">User.Read, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f521-114">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="5f521-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f521-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f521-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f521-116">Not supported.</span></span>                              |
| <span data-ttu-id="5f521-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f521-117">Application</span></span>                            | <span data-ttu-id="5f521-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f521-118">Not supported.</span></span>                              |

><span data-ttu-id="5f521-119">**Примечание:** Использование делегирования разрешений для этой операции требует от пользователя, вписаного, роли администратора клиента или глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="5f521-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="5f521-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f521-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f521-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5f521-121">Optional query parameters</span></span>

<span data-ttu-id="5f521-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5f521-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5f521-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5f521-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f521-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f521-124">Request headers</span></span>

| <span data-ttu-id="5f521-125">Имя</span><span class="sxs-lookup"><span data-stu-id="5f521-125">Name</span></span>          |<span data-ttu-id="5f521-126">Описание</span><span class="sxs-lookup"><span data-stu-id="5f521-126">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="5f521-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f521-127">Authorization</span></span> | <span data-ttu-id="5f521-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f521-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="5f521-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f521-130">Content-Type</span></span>  | <span data-ttu-id="5f521-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f521-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f521-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f521-133">Request body</span></span>

<span data-ttu-id="5f521-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f521-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f521-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f521-135">Response</span></span>

<span data-ttu-id="5f521-136">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [organizationSettings](../resources/organizationsettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5f521-136">If successful, this method returns a `200 OK` response code and the requested [organizationSettings](../resources/organizationsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f521-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="5f521-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f521-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f521-138">Request</span></span>

<span data-ttu-id="5f521-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f521-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5f521-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f521-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationsettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/settings
```
# <a name="c"></a>[<span data-ttu-id="5f521-141">C#</span><span class="sxs-lookup"><span data-stu-id="5f521-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f521-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f521-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f521-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f521-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f521-144">Java</span><span class="sxs-lookup"><span data-stu-id="5f521-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5f521-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f521-145">Response</span></span>

<span data-ttu-id="5f521-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5f521-146">The following is an example of the response.</span></span>

> <span data-ttu-id="5f521-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5f521-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "345233-676277-644334-445677-334556",
  "profileCardProperties": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


