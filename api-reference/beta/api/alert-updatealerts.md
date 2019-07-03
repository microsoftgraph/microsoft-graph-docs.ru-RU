---
title: 'Предупреждение: Упдатеалертс'
description: Обновление нескольких оповещений в одном запросе вместо нескольких запросов.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 109767fb4d3bfaea173337a7d853e84e2261ef85
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439751"
---
# <a name="alert-updatealerts"></a><span data-ttu-id="01255-103">Предупреждение: Упдатеалертс</span><span class="sxs-lookup"><span data-stu-id="01255-103">alert: updateAlerts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01255-104">Обновление нескольких оповещений в одном запросе вместо нескольких запросов.</span><span class="sxs-lookup"><span data-stu-id="01255-104">Update multiple alerts in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="01255-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01255-105">Permissions</span></span>

<span data-ttu-id="01255-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01255-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01255-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01255-108">Permission type</span></span>                        | <span data-ttu-id="01255-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01255-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="01255-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01255-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="01255-111">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01255-111">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="01255-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01255-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="01255-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01255-113">Not supported.</span></span>  |
|<span data-ttu-id="01255-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01255-114">Application</span></span> | <span data-ttu-id="01255-115">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01255-115">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01255-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01255-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a><span data-ttu-id="01255-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01255-117">Request headers</span></span>

| <span data-ttu-id="01255-118">Имя</span><span class="sxs-lookup"><span data-stu-id="01255-118">Name</span></span>          | <span data-ttu-id="01255-119">Описание</span><span class="sxs-lookup"><span data-stu-id="01255-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="01255-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01255-120">Authorization</span></span> | <span data-ttu-id="01255-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="01255-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="01255-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01255-122">Request body</span></span>

<span data-ttu-id="01255-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="01255-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="01255-124">У каждой сущности должны быть свойства **ID** и **вендоринформатион** .</span><span class="sxs-lookup"><span data-stu-id="01255-124">Each entity must have **id** and **vendorInformation** properties.</span></span> <span data-ttu-id="01255-125">Для получения дополнительных сведений о свойствах, которые можно обновить, ознакомьтесь со статьей [Обновление оповещения](alert-update.md).</span><span class="sxs-lookup"><span data-stu-id="01255-125">For details about properties that can be updated, see [update alert](alert-update.md).</span></span>

| <span data-ttu-id="01255-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="01255-126">Parameter</span></span>    | <span data-ttu-id="01255-127">Тип</span><span class="sxs-lookup"><span data-stu-id="01255-127">Type</span></span>        | <span data-ttu-id="01255-128">Описание</span><span class="sxs-lookup"><span data-stu-id="01255-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="01255-129">значение</span><span class="sxs-lookup"><span data-stu-id="01255-129">value</span></span>|<span data-ttu-id="01255-130">Коллекция [alert](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="01255-130">[alert](../resources/alert.md) collection</span></span>| <span data-ttu-id="01255-131">Коллекция оповещений, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="01255-131">Collection of alerts to update.</span></span> <span data-ttu-id="01255-132">Каждая сущность должна иметь **идентификатор**, **вендоринформатион**и другие редактируемые свойства, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="01255-132">Each entity must have **id**, **vendorInformation**, and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="01255-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="01255-133">Response</span></span>

<span data-ttu-id="01255-134">В случае успешного выполнения этот метод `200, OK` возвращает код отклика и объект коллекции [Alerts](../resources/alert.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01255-134">If successful, this method returns `200, OK` response code and [alert](../resources/alert.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01255-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="01255-135">Examples</span></span>

<span data-ttu-id="01255-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="01255-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="01255-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="01255-137">Request</span></span>

<span data-ttu-id="01255-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01255-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="01255-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="01255-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "alert_updatealerts",
   "isCollection": "true"
}-->

```http
POST https://graph.microsoft.com/beta/security/alerts/updateAlerts
Content-type: application/json

{
  "value": [
    {
      "assignedTo": "String",
      "closedDateTime": "String (timestamp)",
      "comments": ["String"],
      "feedback": {"@odata.type": "microsoft.graph.alertFeedback"},
      "id": "String (identifier)",
      "status": {"@odata.type": "microsoft.graph.alertStatus"},
      "tags": ["String"],
      "vendorInformation":
        {
          "provider": "String",
          "vendor": "String"
        }
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="01255-140">C#</span><span class="sxs-lookup"><span data-stu-id="01255-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/alert-updatealerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01255-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="01255-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/alert-updatealerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="01255-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="01255-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/alert-updatealerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="01255-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="01255-143">Response</span></span>

<span data-ttu-id="01255-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="01255-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="01255-145">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="01255-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="01255-146">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="01255-146">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert: updateAlerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
