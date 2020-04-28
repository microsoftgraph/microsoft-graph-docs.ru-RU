---
title: 'Предупреждение: Упдатеалертс'
description: Обновление нескольких оповещений в одном запросе вместо нескольких запросов.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 684c96aeb0f297c783343001a1ab00bc82f9da63
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441636"
---
# <a name="alert-updatealerts"></a><span data-ttu-id="2052c-103">Предупреждение: Упдатеалертс</span><span class="sxs-lookup"><span data-stu-id="2052c-103">alert: updateAlerts</span></span>

<span data-ttu-id="2052c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2052c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2052c-105">Обновление нескольких оповещений в одном запросе вместо нескольких запросов.</span><span class="sxs-lookup"><span data-stu-id="2052c-105">Update multiple alerts in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="2052c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2052c-106">Permissions</span></span>

<span data-ttu-id="2052c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2052c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2052c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2052c-109">Permission type</span></span>                        | <span data-ttu-id="2052c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2052c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="2052c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2052c-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="2052c-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2052c-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="2052c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2052c-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2052c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2052c-114">Not supported.</span></span>  |
|<span data-ttu-id="2052c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2052c-115">Application</span></span> | <span data-ttu-id="2052c-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2052c-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2052c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2052c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a><span data-ttu-id="2052c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2052c-118">Request headers</span></span>

| <span data-ttu-id="2052c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2052c-119">Name</span></span>          | <span data-ttu-id="2052c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2052c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2052c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2052c-121">Authorization</span></span> | <span data-ttu-id="2052c-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2052c-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2052c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2052c-123">Request body</span></span>

<span data-ttu-id="2052c-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2052c-124">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="2052c-125">У каждой сущности должны быть свойства **ID** и **вендоринформатион** .</span><span class="sxs-lookup"><span data-stu-id="2052c-125">Each entity must have **id** and **vendorInformation** properties.</span></span> <span data-ttu-id="2052c-126">Для получения дополнительных сведений о свойствах, которые можно обновить, ознакомьтесь со статьей [Обновление оповещения](alert-update.md).</span><span class="sxs-lookup"><span data-stu-id="2052c-126">For details about properties that can be updated, see [update alert](alert-update.md).</span></span>

| <span data-ttu-id="2052c-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="2052c-127">Parameter</span></span>    | <span data-ttu-id="2052c-128">Тип</span><span class="sxs-lookup"><span data-stu-id="2052c-128">Type</span></span>        | <span data-ttu-id="2052c-129">Описание</span><span class="sxs-lookup"><span data-stu-id="2052c-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2052c-130">значение</span><span class="sxs-lookup"><span data-stu-id="2052c-130">value</span></span>|<span data-ttu-id="2052c-131">Коллекция [alert](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="2052c-131">[alert](../resources/alert.md) collection</span></span>| <span data-ttu-id="2052c-132">Коллекция оповещений, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="2052c-132">Collection of alerts to update.</span></span> <span data-ttu-id="2052c-133">Каждая сущность должна иметь **идентификатор**, **вендоринформатион**и другие редактируемые свойства, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="2052c-133">Each entity must have **id**, **vendorInformation**, and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="2052c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2052c-134">Response</span></span>

<span data-ttu-id="2052c-135">В случае успешного выполнения этот метод `200, OK` возвращает код отклика и объект коллекции [Alerts](../resources/alert.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2052c-135">If successful, this method returns `200, OK` response code and [alert](../resources/alert.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2052c-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="2052c-136">Examples</span></span>

<span data-ttu-id="2052c-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="2052c-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2052c-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="2052c-138">Request</span></span>

<span data-ttu-id="2052c-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2052c-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2052c-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="2052c-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2052c-141">C#</span><span class="sxs-lookup"><span data-stu-id="2052c-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/alert-updatealerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2052c-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2052c-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/alert-updatealerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2052c-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2052c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/alert-updatealerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2052c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="2052c-144">Response</span></span>

<span data-ttu-id="2052c-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2052c-145">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="2052c-146">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2052c-146">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2052c-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2052c-147">All the properties will be returned from an actual call.</span></span>

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
