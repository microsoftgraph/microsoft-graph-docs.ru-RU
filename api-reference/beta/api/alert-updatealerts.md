---
title: 'Предупреждение: Упдатеалертс'
description: Обновление нескольких оповещений в одном запросе вместо нескольких запросов.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b04227886085305103dd6a9ba6c243565d0e5a06
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636529"
---
# <a name="alert-updatealerts"></a><span data-ttu-id="59df4-103">Предупреждение: Упдатеалертс</span><span class="sxs-lookup"><span data-stu-id="59df4-103">alert: updateAlerts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59df4-104">Обновление нескольких оповещений в одном запросе вместо нескольких запросов.</span><span class="sxs-lookup"><span data-stu-id="59df4-104">Update multiple alerts in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="59df4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59df4-105">Permissions</span></span>

<span data-ttu-id="59df4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59df4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="59df4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59df4-108">Permission type</span></span>                        | <span data-ttu-id="59df4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59df4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="59df4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59df4-110">Delegated (work or school account)</span></span> |   <span data-ttu-id="59df4-111">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59df4-111">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="59df4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59df4-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="59df4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59df4-113">Not supported.</span></span>  |
|<span data-ttu-id="59df4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="59df4-114">Application</span></span> | <span data-ttu-id="59df4-115">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59df4-115">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59df4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59df4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a><span data-ttu-id="59df4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59df4-117">Request headers</span></span>

| <span data-ttu-id="59df4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="59df4-118">Name</span></span>          | <span data-ttu-id="59df4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="59df4-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="59df4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59df4-120">Authorization</span></span> | <span data-ttu-id="59df4-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="59df4-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="59df4-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59df4-122">Request body</span></span>

<span data-ttu-id="59df4-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="59df4-123">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="59df4-124">У каждой сущности должны быть свойства **ID** и **вендоринформатион** .</span><span class="sxs-lookup"><span data-stu-id="59df4-124">Each entity must have **id** and **vendorInformation** properties.</span></span> <span data-ttu-id="59df4-125">Для получения дополнительных сведений о свойствах, которые можно обновить, ознакомьтесь со статьей [Обновление оповещения](alert-update.md).</span><span class="sxs-lookup"><span data-stu-id="59df4-125">For details about properties that can be updated, see [update alert](alert-update.md).</span></span>

| <span data-ttu-id="59df4-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="59df4-126">Parameter</span></span>    | <span data-ttu-id="59df4-127">Тип</span><span class="sxs-lookup"><span data-stu-id="59df4-127">Type</span></span>        | <span data-ttu-id="59df4-128">Описание</span><span class="sxs-lookup"><span data-stu-id="59df4-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="59df4-129">значение</span><span class="sxs-lookup"><span data-stu-id="59df4-129">value</span></span>|<span data-ttu-id="59df4-130">Коллекция [alert](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="59df4-130">[alert](../resources/alert.md) collection</span></span>| <span data-ttu-id="59df4-131">Коллекция оповещений, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="59df4-131">Collection of alerts to update.</span></span> <span data-ttu-id="59df4-132">Каждая сущность должна иметь **идентификатор**, **вендоринформатион**и другие редактируемые свойства, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="59df4-132">Each entity must have **id**, **vendorInformation**, and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="59df4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="59df4-133">Response</span></span>

<span data-ttu-id="59df4-134">В случае успешного выполнения этот метод `200, OK` возвращает код отклика и объект коллекции [Alerts](../resources/alert.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="59df4-134">If successful, this method returns `200, OK` response code and [alert](../resources/alert.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="59df4-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="59df4-135">Examples</span></span>

<span data-ttu-id="59df4-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="59df4-136">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="59df4-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="59df4-137">Request</span></span>

<span data-ttu-id="59df4-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59df4-138">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="59df4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="59df4-139">Response</span></span>

<span data-ttu-id="59df4-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="59df4-140">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="59df4-141">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="59df4-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="59df4-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59df4-142">All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="59df4-143">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="59df4-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="59df4-144">Языках</span><span class="sxs-lookup"><span data-stu-id="59df4-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/alert_updatealerts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59df4-145">Язык</span><span class="sxs-lookup"><span data-stu-id="59df4-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/alert_updatealerts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alert: updateAlerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/alert-updatealerts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/alert-updatealerts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
