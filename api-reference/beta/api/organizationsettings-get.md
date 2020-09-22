---
title: Получение Организатионсеттингс
description: Получение свойств и связей объекта Организатионсеттингс.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0e6501c58c2de2cb1bee0724eb7037ca4359e674
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979961"
---
# <a name="get-organizationsettings"></a><span data-ttu-id="289f0-103">Получение Организатионсеттингс</span><span class="sxs-lookup"><span data-stu-id="289f0-103">Get organizationSettings</span></span>

<span data-ttu-id="289f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="289f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="289f0-105">Получение свойств и связей объекта [организатионсеттингс](../resources/organizationsettings.md) , в том числе **профилекардпропертиес**.</span><span class="sxs-lookup"><span data-stu-id="289f0-105">Retrieve the properties and relationships of an [organizationSettings](../resources/organizationsettings.md) object, including **profileCardProperties**.</span></span>

<span data-ttu-id="289f0-106">Эта операция не возвращает [итеминсигхтссеттингс](../resources/iteminsightssettings.md) с помощью свойства навигации **итеминсигхтс** .</span><span class="sxs-lookup"><span data-stu-id="289f0-106">This operation does not return [itemInsightsSettings](../resources/iteminsightssettings.md) through the **itemInsights** navigation property.</span></span> <span data-ttu-id="289f0-107">Вместо этого используйте [Get итеминсигхтссеттингс](iteminsightssettings-get.md) .</span><span class="sxs-lookup"><span data-stu-id="289f0-107">Use [get itemInsightsSettings](iteminsightssettings-get.md) instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="289f0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="289f0-108">Permissions</span></span>

<span data-ttu-id="289f0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="289f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="289f0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="289f0-111">Permission type</span></span>                        | <span data-ttu-id="289f0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="289f0-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="289f0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="289f0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="289f0-114">User. Read, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="289f0-114">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="289f0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="289f0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="289f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="289f0-116">Not supported.</span></span>                              |
| <span data-ttu-id="289f0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="289f0-117">Application</span></span>                            | <span data-ttu-id="289f0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="289f0-118">Not supported.</span></span>                              |

><span data-ttu-id="289f0-119">**Примечание:** Для этой операции с делегированными разрешениями необходимо, чтобы вошедшего в систему пользователя была назначена роль администратора клиента или роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="289f0-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="289f0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="289f0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="289f0-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="289f0-121">Optional query parameters</span></span>

<span data-ttu-id="289f0-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="289f0-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="289f0-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="289f0-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="289f0-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="289f0-124">Request headers</span></span>

| <span data-ttu-id="289f0-125">Имя</span><span class="sxs-lookup"><span data-stu-id="289f0-125">Name</span></span>          |<span data-ttu-id="289f0-126">Описание</span><span class="sxs-lookup"><span data-stu-id="289f0-126">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="289f0-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="289f0-127">Authorization</span></span> | <span data-ttu-id="289f0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="289f0-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="289f0-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="289f0-130">Content-Type</span></span>  | <span data-ttu-id="289f0-p105">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="289f0-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="289f0-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="289f0-133">Request body</span></span>

<span data-ttu-id="289f0-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="289f0-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="289f0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="289f0-135">Response</span></span>

<span data-ttu-id="289f0-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [организатионсеттингс](../resources/organizationsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="289f0-136">If successful, this method returns a `200 OK` response code and the requested [organizationSettings](../resources/organizationsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="289f0-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="289f0-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="289f0-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="289f0-138">Request</span></span>

<span data-ttu-id="289f0-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="289f0-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="289f0-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="289f0-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationsettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/settings
```
# <a name="c"></a>[<span data-ttu-id="289f0-141">C#</span><span class="sxs-lookup"><span data-stu-id="289f0-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="289f0-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="289f0-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="289f0-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="289f0-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="289f0-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="289f0-144">Response</span></span>

<span data-ttu-id="289f0-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="289f0-145">The following is an example of the response.</span></span>

> <span data-ttu-id="289f0-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="289f0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


