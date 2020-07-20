---
title: Получение Организатионсеттингс
description: Получение свойств и связей объекта Организатионсеттингс.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1de3e239f64b81a6e8f2995bfa626a0d7734ef9e
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080772"
---
# <a name="get-organizationsettings"></a><span data-ttu-id="ab1a6-103">Получение Организатионсеттингс</span><span class="sxs-lookup"><span data-stu-id="ab1a6-103">Get organizationSettings</span></span>

<span data-ttu-id="ab1a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab1a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab1a6-105">Получение свойств и связей объекта [организатионсеттингс](../resources/organizationsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="ab1a6-105">Retrieve the properties and relationships of an [organizationSettings](../resources/organizationsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab1a6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab1a6-106">Permissions</span></span>

<span data-ttu-id="ab1a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab1a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab1a6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab1a6-109">Permission type</span></span>                        | <span data-ttu-id="ab1a6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab1a6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ab1a6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab1a6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab1a6-112">User. Read, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="ab1a6-112">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="ab1a6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab1a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab1a6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab1a6-114">Not supported.</span></span>                              |
| <span data-ttu-id="ab1a6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab1a6-115">Application</span></span>                            | <span data-ttu-id="ab1a6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab1a6-116">Not supported.</span></span>                              |

><span data-ttu-id="ab1a6-117">**Примечание:** Для этой операции с делегированными разрешениями необходимо, чтобы вошедшего в систему пользователя была назначена роль администратора клиента или роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="ab1a6-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="ab1a6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab1a6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab1a6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ab1a6-119">Optional query parameters</span></span>

<span data-ttu-id="ab1a6-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ab1a6-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ab1a6-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ab1a6-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab1a6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab1a6-122">Request headers</span></span>

| <span data-ttu-id="ab1a6-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ab1a6-123">Name</span></span>          |<span data-ttu-id="ab1a6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ab1a6-124">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="ab1a6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab1a6-125">Authorization</span></span> | <span data-ttu-id="ab1a6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab1a6-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ab1a6-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab1a6-128">Content-Type</span></span>  | <span data-ttu-id="ab1a6-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab1a6-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab1a6-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab1a6-131">Request body</span></span>

<span data-ttu-id="ab1a6-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab1a6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab1a6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab1a6-133">Response</span></span>

<span data-ttu-id="ab1a6-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [организатионсеттингс](../resources/organizationsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab1a6-134">If successful, this method returns a `200 OK` response code and the requested [organizationSettings](../resources/organizationsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ab1a6-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="ab1a6-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ab1a6-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab1a6-136">Request</span></span>

<span data-ttu-id="ab1a6-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab1a6-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ab1a6-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab1a6-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationsettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/settings
```
# <a name="c"></a>[<span data-ttu-id="ab1a6-139">C#</span><span class="sxs-lookup"><span data-stu-id="ab1a6-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab1a6-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab1a6-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab1a6-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab1a6-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ab1a6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab1a6-142">Response</span></span>

<span data-ttu-id="ab1a6-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ab1a6-143">The following is an example of the response.</span></span>

> <span data-ttu-id="ab1a6-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab1a6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
