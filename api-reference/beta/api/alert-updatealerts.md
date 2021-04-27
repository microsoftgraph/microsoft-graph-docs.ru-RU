---
title: 'оповещение: updateAlerts'
description: Обновление нескольких оповещений в одном запросе вместо нескольких запросов.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 86c391f0684ebad30ef5abab0c3a7e8746445a32
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048185"
---
# <a name="alert-updatealerts"></a><span data-ttu-id="60eb7-103">оповещение: updateAlerts</span><span class="sxs-lookup"><span data-stu-id="60eb7-103">alert: updateAlerts</span></span>

<span data-ttu-id="60eb7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60eb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60eb7-105">Обновление нескольких оповещений в одном запросе вместо нескольких запросов.</span><span class="sxs-lookup"><span data-stu-id="60eb7-105">Update multiple alerts in one request instead of multiple requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="60eb7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60eb7-106">Permissions</span></span>

<span data-ttu-id="60eb7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60eb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60eb7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60eb7-109">Permission type</span></span>                        | <span data-ttu-id="60eb7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60eb7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="60eb7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60eb7-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="60eb7-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60eb7-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="60eb7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60eb7-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="60eb7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60eb7-114">Not supported.</span></span>  |
|<span data-ttu-id="60eb7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="60eb7-115">Application</span></span> | <span data-ttu-id="60eb7-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60eb7-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60eb7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60eb7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/alerts/updateAlerts
```

## <a name="request-headers"></a><span data-ttu-id="60eb7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60eb7-118">Request headers</span></span>

| <span data-ttu-id="60eb7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="60eb7-119">Name</span></span>          | <span data-ttu-id="60eb7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="60eb7-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="60eb7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60eb7-121">Authorization</span></span> | <span data-ttu-id="60eb7-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="60eb7-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="60eb7-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60eb7-123">Request body</span></span>

<span data-ttu-id="60eb7-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="60eb7-124">In the request body, provide a JSON object with the following parameters.</span></span> <span data-ttu-id="60eb7-125">Каждая сущность должна иметь **свойства id** и **vendorInformation.**</span><span class="sxs-lookup"><span data-stu-id="60eb7-125">Each entity must have **id** and **vendorInformation** properties.</span></span> <span data-ttu-id="60eb7-126">Сведения о свойствах, которые можно обновить, см. в [материале Update Alert.](alert-update.md)</span><span class="sxs-lookup"><span data-stu-id="60eb7-126">For details about properties that can be updated, see [update alert](alert-update.md).</span></span>

| <span data-ttu-id="60eb7-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="60eb7-127">Parameter</span></span>    | <span data-ttu-id="60eb7-128">Тип</span><span class="sxs-lookup"><span data-stu-id="60eb7-128">Type</span></span>        | <span data-ttu-id="60eb7-129">Описание</span><span class="sxs-lookup"><span data-stu-id="60eb7-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="60eb7-130">значение</span><span class="sxs-lookup"><span data-stu-id="60eb7-130">value</span></span>|<span data-ttu-id="60eb7-131">Коллекция [alert](../resources/alert.md)</span><span class="sxs-lookup"><span data-stu-id="60eb7-131">[alert](../resources/alert.md) collection</span></span>| <span data-ttu-id="60eb7-132">Коллекция оповещений для обновления.</span><span class="sxs-lookup"><span data-stu-id="60eb7-132">Collection of alerts to update.</span></span> <span data-ttu-id="60eb7-133">Каждый объект должен иметь **id,** **vendorInformation** и другие редактируемые свойства, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="60eb7-133">Each entity must have **id**, **vendorInformation**, and other editable properties to be updated.</span></span>|

## <a name="response"></a><span data-ttu-id="60eb7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="60eb7-134">Response</span></span>

<span data-ttu-id="60eb7-135">В случае успешной работы этот метод возвращает код отклика и объект сбора оповещений `200, OK` в тексте [](../resources/alert.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="60eb7-135">If successful, this method returns `200, OK` response code and [alert](../resources/alert.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60eb7-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="60eb7-136">Examples</span></span>

<span data-ttu-id="60eb7-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="60eb7-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="60eb7-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="60eb7-138">Request</span></span>

<span data-ttu-id="60eb7-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60eb7-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="60eb7-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="60eb7-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="60eb7-141">C#</span><span class="sxs-lookup"><span data-stu-id="60eb7-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/alert-updatealerts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60eb7-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60eb7-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/alert-updatealerts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60eb7-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60eb7-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/alert-updatealerts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60eb7-144">Java</span><span class="sxs-lookup"><span data-stu-id="60eb7-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/alert-updatealerts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="60eb7-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="60eb7-145">Response</span></span>

<span data-ttu-id="60eb7-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="60eb7-146">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="60eb7-147">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="60eb7-147">The response object shown here might be shortened for readability.</span></span>

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


