---
title: 'Предупреждение: Упдатеалертс'
description: Обновление нескольких оповещений в одном запросе вместо нескольких запросов.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 7b061b1ab8e323158b12a20262349321b80236fc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855362"
---
# <a name="alert-updatealerts"></a><span data-ttu-id="6b368-103">Предупреждение: Упдатеалертс</span><span class="sxs-lookup"><span data-stu-id="6b368-103">alert: updateAlerts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b368-104">Обновление нескольких оповещений в одном запросе вместо нескольких запросов.</span><span class="sxs-lookup"><span data-stu-id="6b368-104">Update multiple alerts in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b368-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b368-105">Permissions</span></span>

<span data-ttu-id="6b368-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b368-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b368-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b368-108">Permission type</span></span>                        | <span data-ttu-id="6b368-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b368-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="6b368-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b368-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="6b368-111">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b368-111">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="6b368-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b368-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6b368-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b368-113">Not supported.</span></span>  |
|<span data-ttu-id="6b368-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b368-114">Application</span></span> | <span data-ttu-id="6b368-115">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b368-115">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b368-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b368-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a><span data-ttu-id="6b368-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b368-117">Request headers</span></span>

| <span data-ttu-id="6b368-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6b368-118">Name</span></span>          | <span data-ttu-id="6b368-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6b368-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6b368-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b368-120">Authorization</span></span> | <span data-ttu-id="6b368-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6b368-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b368-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b368-122">Request body</span></span>

<span data-ttu-id="6b368-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6b368-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="6b368-124">У каждой сущности должны быть свойства **ID** и **вендоринформатион** .</span><span class="sxs-lookup"><span data-stu-id="6b368-124">Each entity must have **id** and **vendorInformation** properties.</span></span> <span data-ttu-id="6b368-125">Для получения дополнительных сведений о свойствах, которые можно обновить, ознакомьтесь со статьей [Обновление оповещения](alert-update.md).</span><span class="sxs-lookup"><span data-stu-id="6b368-125">For details about properties that can be updated, see [update alert](alert-update.md).</span></span>

| <span data-ttu-id="6b368-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="6b368-126">Parameter</span></span>    | <span data-ttu-id="6b368-127">Тип</span><span class="sxs-lookup"><span data-stu-id="6b368-127">Type</span></span>        | <span data-ttu-id="6b368-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6b368-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6b368-129">значение</span><span class="sxs-lookup"><span data-stu-id="6b368-129">value</span></span>|<span data-ttu-id="6b368-130">Коллекция [alert](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="6b368-130">[alert](../resources/alert.md) collection</span></span>| <span data-ttu-id="6b368-131">Коллекция оповещений, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6b368-131">Collection of alerts to update.</span></span> <span data-ttu-id="6b368-132">Каждая сущность должна иметь **идентификатор**, **вендоринформатион**и другие редактируемые свойства, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6b368-132">Each entity must have **id**, **vendorInformation**, and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="6b368-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b368-133">Response</span></span>

<span data-ttu-id="6b368-134">В случае успешного выполнения этот метод `200, OK` возвращает код отклика и объект коллекции [Alerts](../resources/alert.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b368-134">If successful, this method returns `200, OK` response code and [alert](../resources/alert.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6b368-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="6b368-135">Examples</span></span>

<span data-ttu-id="6b368-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="6b368-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6b368-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b368-137">Request</span></span>

<span data-ttu-id="6b368-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b368-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6b368-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b368-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6b368-140">C#</span><span class="sxs-lookup"><span data-stu-id="6b368-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/alert-updatealerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6b368-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="6b368-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/alert-updatealerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6b368-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6b368-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/alert-updatealerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6b368-143">Java</span><span class="sxs-lookup"><span data-stu-id="6b368-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/alert-updatealerts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6b368-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b368-144">Response</span></span>

<span data-ttu-id="6b368-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6b368-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="6b368-146">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6b368-146">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6b368-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b368-147">All the properties will be returned from an actual call.</span></span>

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
