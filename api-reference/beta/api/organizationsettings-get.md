---
title: Получение Организатионсеттингс
description: Получение свойств и связей объекта Организатионсеттингс.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 240704fd29f3950060342f4d2b8ab2efcc6f2ee0
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051138"
---
# <a name="get-organizationsettings"></a><span data-ttu-id="a78da-103">Получение Организатионсеттингс</span><span class="sxs-lookup"><span data-stu-id="a78da-103">Get organizationSettings</span></span>

<span data-ttu-id="a78da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a78da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a78da-105">Получение свойств и связей объекта [организатионсеттингс](../resources/organizationsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="a78da-105">Retrieve the properties and relationships of an [organizationSettings](../resources/organizationsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a78da-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a78da-106">Permissions</span></span>

<span data-ttu-id="a78da-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="a78da-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a78da-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a78da-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a78da-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a78da-109">Permission type</span></span>                        | <span data-ttu-id="a78da-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a78da-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a78da-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a78da-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a78da-112">User. Read, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="a78da-112">User.Read, User.Read.All</span></span>                    |
| <span data-ttu-id="a78da-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a78da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a78da-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a78da-114">Not supported.</span></span>                              |
| <span data-ttu-id="a78da-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a78da-115">Application</span></span>                            | <span data-ttu-id="a78da-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a78da-116">Not supported.</span></span>                              |

><span data-ttu-id="a78da-117">**Примечание:** Для этой операции с делегированными разрешениями необходимо, чтобы вошедшего в систему пользователя была назначена роль администратора клиента или роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="a78da-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="a78da-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a78da-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/organization/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a78da-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a78da-119">Optional query parameters</span></span>

<span data-ttu-id="a78da-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a78da-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a78da-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a78da-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a78da-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a78da-122">Request headers</span></span>

| <span data-ttu-id="a78da-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a78da-123">Name</span></span>          |<span data-ttu-id="a78da-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a78da-124">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="a78da-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a78da-125">Authorization</span></span> | <span data-ttu-id="a78da-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="a78da-126">Bearer {token}.</span></span> <span data-ttu-id="a78da-127">Required.</span><span class="sxs-lookup"><span data-stu-id="a78da-127">Required.</span></span>   |
| <span data-ttu-id="a78da-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a78da-128">Content-Type</span></span>  | <span data-ttu-id="a78da-129">application/json.</span><span class="sxs-lookup"><span data-stu-id="a78da-129">application/json.</span></span> <span data-ttu-id="a78da-130">Required.</span><span class="sxs-lookup"><span data-stu-id="a78da-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a78da-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a78da-131">Request body</span></span>

<span data-ttu-id="a78da-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a78da-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a78da-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a78da-133">Response</span></span>

<span data-ttu-id="a78da-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [организатионсеттингс](../resources/organizationsettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a78da-134">If successful, this method returns a `200 OK` response code and the requested [organizationSettings](../resources/organizationsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a78da-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="a78da-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a78da-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a78da-136">Request</span></span>

<span data-ttu-id="a78da-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a78da-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationsettings"
}-->

```http
GET https://graph.microsoft.com/beta/organization/settings
```

### <a name="response"></a><span data-ttu-id="a78da-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a78da-138">Response</span></span>

<span data-ttu-id="a78da-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a78da-139">The following is an example of the response.</span></span>

> <span data-ttu-id="a78da-140">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="a78da-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a78da-141">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="a78da-141">All the properties will be returned from an actual call.</span></span>

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
