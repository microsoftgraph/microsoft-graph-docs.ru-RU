---
title: Проблемы со списком
description: Извлекать ресурсы serviceHealthIssue из свойства навигации проблем.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: b798ef786d4c90756d76c9980554cd569ae314c6
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208904"
---
# <a name="list-issues"></a><span data-ttu-id="088b0-103">Проблемы со списком</span><span class="sxs-lookup"><span data-stu-id="088b0-103">List issues</span></span>
<span data-ttu-id="088b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="088b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="088b0-105">[Извлечение ресурсов serviceHealthIssue](../resources/servicehealthissue.md) из свойства **навигации** проблем.</span><span class="sxs-lookup"><span data-stu-id="088b0-105">Retrieve [serviceHealthIssue](../resources/servicehealthissue.md) resources from the **issues** navigation property.</span></span>

<span data-ttu-id="088b0-106">Эта операция извлекает сведения обо всех проблемах со здоровьем служб, которые существуют для клиента.</span><span class="sxs-lookup"><span data-stu-id="088b0-106">This operation retrieves information about all service health issues that exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="088b0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="088b0-107">Permissions</span></span>
<span data-ttu-id="088b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="088b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="088b0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="088b0-110">Permission type</span></span>|<span data-ttu-id="088b0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="088b0-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="088b0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="088b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="088b0-113">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="088b0-113">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="088b0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="088b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="088b0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="088b0-115">Not supported.</span></span>|
|<span data-ttu-id="088b0-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="088b0-116">Application</span></span>|<span data-ttu-id="088b0-117">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="088b0-117">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="088b0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="088b0-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/issues
```

## <a name="optional-query-parameters"></a><span data-ttu-id="088b0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="088b0-119">Optional query parameters</span></span>
<span data-ttu-id="088b0-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="088b0-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="088b0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="088b0-121">Request headers</span></span>
|<span data-ttu-id="088b0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="088b0-122">Name</span></span>|<span data-ttu-id="088b0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="088b0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="088b0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="088b0-124">Authorization</span></span>|<span data-ttu-id="088b0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="088b0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="088b0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="088b0-127">Request body</span></span>
<span data-ttu-id="088b0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="088b0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="088b0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="088b0-129">Response</span></span>

<span data-ttu-id="088b0-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [serviceHealthIssue](../resources/servicehealthissue.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="088b0-130">If successful, this method returns a `200 OK` response code and a collection of [serviceHealthIssue](../resources/servicehealthissue.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="088b0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="088b0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="088b0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="088b0-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="088b0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="088b0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_servicehealthissue"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/issues
```
# <a name="c"></a>[<span data-ttu-id="088b0-134">C#</span><span class="sxs-lookup"><span data-stu-id="088b0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-servicehealthissue-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="088b0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="088b0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-servicehealthissue-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="088b0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="088b0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-servicehealthissue-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="088b0-137">Java</span><span class="sxs-lookup"><span data-stu-id="088b0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-servicehealthissue-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="088b0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="088b0-138">Response</span></span>
><span data-ttu-id="088b0-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="088b0-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceHealthIssue",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/issues",
  "value": [
    {
      "startDateTime": "2020-11-13T21:00:00Z",
      "endDateTime": "2020-11-14T17:15:00Z",
      "lastModifiedDateTime": "2020-11-14T18:20:24.767Z",
      "title": "Limited number of users unable to send or receive email through the Exchange Online service",
      "id": "EX226792",
      "impactDescription": "Users may have been unable to send or receive email through the Exchange Online service.",
      "classification": "Incident",
      "origin": "Microsoft",
      "status": "ServiceRestored",
      "service": "Exchange Online",
      "feature": "Mailflow - delayed delivery from Internet",
      "featureGroup": "E-Mail timely delivery",
      "isResolved": true,
      "details": [
        {
          "name": "NotifyInApp",
          "value": "True"
        }
      ],
      "posts": [
        {
          "createdDateTime": "2020-11-12T07:07:38.97Z",
          "postType": "Regular",
          "description": {
            "contentType": "Text",
            "content": "Title: Limited number of users unable to send or receive email through the Exchange Online service\n\nUser Impact: Users may be unable to send or receive email through the Exchange Online service."
          }
        }
      ]
    }
  ]
}
```

