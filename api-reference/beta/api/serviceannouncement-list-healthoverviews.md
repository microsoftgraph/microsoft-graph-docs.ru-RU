---
title: Список healthOverviews
description: Извлекать ресурсы serviceHealth из свойства навигации healthOverviews.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: d8e2905acb0989d2d47d1f3df7c71237dca083c4
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210929"
---
# <a name="list-healthoverviews"></a><span data-ttu-id="942c7-103">Список healthOverviews</span><span class="sxs-lookup"><span data-stu-id="942c7-103">List healthOverviews</span></span>
<span data-ttu-id="942c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="942c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="942c7-105">Извлекать [ресурсы serviceHealth](../resources/servicehealth.md) из **свойства навигации healthOverviews.**</span><span class="sxs-lookup"><span data-stu-id="942c7-105">Retrieve the [serviceHealth](../resources/servicehealth.md) resources from the **healthOverviews** navigation property.</span></span>

<span data-ttu-id="942c7-106">Эта операция предоставляет отчет о состоянии здоровья всех подписаных служб для клиента.</span><span class="sxs-lookup"><span data-stu-id="942c7-106">This operation provides the health report of all subscribed services for a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="942c7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="942c7-107">Permissions</span></span>
<span data-ttu-id="942c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="942c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="942c7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="942c7-110">Permission type</span></span>|<span data-ttu-id="942c7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="942c7-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="942c7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="942c7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="942c7-113">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="942c7-113">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="942c7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="942c7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="942c7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="942c7-115">Not supported.</span></span>|
|<span data-ttu-id="942c7-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="942c7-116">Application</span></span>|<span data-ttu-id="942c7-117">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="942c7-117">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="942c7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="942c7-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/healthOverviews
```

## <a name="optional-query-parameters"></a><span data-ttu-id="942c7-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="942c7-119">Optional query parameters</span></span>
<span data-ttu-id="942c7-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="942c7-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="942c7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="942c7-121">Request headers</span></span>
|<span data-ttu-id="942c7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="942c7-122">Name</span></span>|<span data-ttu-id="942c7-123">Описание</span><span class="sxs-lookup"><span data-stu-id="942c7-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="942c7-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="942c7-124">Authorization</span></span>|<span data-ttu-id="942c7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="942c7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="942c7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="942c7-127">Request body</span></span>
<span data-ttu-id="942c7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="942c7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="942c7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="942c7-129">Response</span></span>

<span data-ttu-id="942c7-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [serviceHealth](../resources/servicehealth.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="942c7-130">If successful, this method returns a `200 OK` response code and a collection of [serviceHealth](../resources/servicehealth.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="942c7-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="942c7-131">Examples</span></span>

### <a name="example-1-get-servicehealth-resources"></a><span data-ttu-id="942c7-132">Пример 1. Получить ресурсы serviceHealth</span><span class="sxs-lookup"><span data-stu-id="942c7-132">Example 1: Get serviceHealth resources</span></span>

#### <a name="request"></a><span data-ttu-id="942c7-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="942c7-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="942c7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="942c7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_healthoverviews"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews
```
# <a name="c"></a>[<span data-ttu-id="942c7-135">C#</span><span class="sxs-lookup"><span data-stu-id="942c7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-healthoverviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="942c7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="942c7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-healthoverviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="942c7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="942c7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-healthoverviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="942c7-138">Java</span><span class="sxs-lookup"><span data-stu-id="942c7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-healthoverviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="942c7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="942c7-139">Response</span></span>
><span data-ttu-id="942c7-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="942c7-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews",
  "value": [
    {
        "service": "Exchange Online",
        "status": "ServicaOperational",
        "id": "Exchange"
    },
    {
        "service": "Identity Service",
        "status": "ServiceRestored",
        "id": "OrgLiveID"
    },
    {
        "service": "Microsoft 365 suite",
        "status": "ServiceOperational",
        "id": "OSDPPlatform"
    }
  ]
}
```

### <a name="example-2-include-navigation-property-issues"></a><span data-ttu-id="942c7-141">Пример 2. Включаем проблемы свойств навигации</span><span class="sxs-lookup"><span data-stu-id="942c7-141">Example 2: Include navigation property issues</span></span>

#### <a name="request"></a><span data-ttu-id="942c7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="942c7-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="942c7-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="942c7-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_healthoverviews_with_issues"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/healthOverviews?$expand=issues
```
# <a name="c"></a>[<span data-ttu-id="942c7-144">C#</span><span class="sxs-lookup"><span data-stu-id="942c7-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-healthoverviews-with-issues-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="942c7-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="942c7-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-healthoverviews-with-issues-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="942c7-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="942c7-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-healthoverviews-with-issues-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="942c7-147">Java</span><span class="sxs-lookup"><span data-stu-id="942c7-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-healthoverviews-with-issues-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="942c7-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="942c7-148">Response</span></span>
><span data-ttu-id="942c7-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="942c7-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealth",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/healthOverviews(issues())",
  "value": [
    {
      "service": "Exchange Online",
      "status": "ServiceOperational",
      "id": "Exchange",
      "issues": [
          {
              "startDateTime": "2020-11-04T00:00:00Z",
              "endDateTime": "2020-11-20T17:00:00Z",
              "lastModifiedDateTime": "2020-11-20T17:56:31.39Z",
              "title": "Admins are unable to migrate some user mailboxes from IMAP using the Exchange admin center or PowerShell",
              "id": "EX226574",
              "impactDescription": "Admins attempting to migrate some user mailboxes using the Exchange admin center or PowerShell experienced failures.",
              "classification": "Advisory",
              "origin": "Microsoft",
              "status": "ServiceRestored",
              "service": "Exchange Online",
              "feature": "Tenant Administration (Provisioning, Remote PowerShell)",
              "featureGroup": "Management and Provisioning",
              "isResolved": true,
              "details": [],
              "posts": [
                  {
                    "createdDateTime": "2020-11-12T07:07:38.97Z",
                    "postType": "Regular",
                    "description": {
                        "contentType": "Text",
                        "content": "Title: Exchange Online service has login issue. We'll provide an update within 30 minutes."
                    }
                  }
                ]
          }
        ]
    }
  ]
}
```
