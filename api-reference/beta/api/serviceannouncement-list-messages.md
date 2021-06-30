---
title: Список сообщений
description: Извлекать ресурсы serviceUpdateMessage из свойства навигации сообщений.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 556bf38ee32fe6652f36be7e909535c551b9f602
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208861"
---
# <a name="list-messages"></a><span data-ttu-id="094b5-103">Список сообщений</span><span class="sxs-lookup"><span data-stu-id="094b5-103">List messages</span></span>
<span data-ttu-id="094b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="094b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="094b5-105">Извлекать [ресурсы serviceUpdateMessage](../resources/serviceupdatemessage.md) из свойства **навигации** сообщений.</span><span class="sxs-lookup"><span data-stu-id="094b5-105">Retrieve the [serviceUpdateMessage](../resources/serviceupdatemessage.md) resources from the **messages** navigation property.</span></span>

<span data-ttu-id="094b5-106">Эта операция извлекает все сообщения обновления службы, которые существуют для клиента.</span><span class="sxs-lookup"><span data-stu-id="094b5-106">This operation retrieves all service update messages that exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="094b5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="094b5-107">Permissions</span></span>
<span data-ttu-id="094b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="094b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="094b5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="094b5-110">Permission type</span></span>|<span data-ttu-id="094b5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="094b5-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="094b5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="094b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="094b5-113">ServiceMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="094b5-113">ServiceMessage.Read.All</span></span>|
|<span data-ttu-id="094b5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="094b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="094b5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="094b5-115">Not supported.</span></span>|
|<span data-ttu-id="094b5-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="094b5-116">Application</span></span>|<span data-ttu-id="094b5-117">ServiceMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="094b5-117">ServiceMessage.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="094b5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="094b5-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="094b5-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="094b5-119">Optional query parameters</span></span>
<span data-ttu-id="094b5-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="094b5-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="094b5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="094b5-121">Request headers</span></span>
|<span data-ttu-id="094b5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="094b5-122">Name</span></span>|<span data-ttu-id="094b5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="094b5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="094b5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="094b5-124">Authorization</span></span>|<span data-ttu-id="094b5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="094b5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="094b5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="094b5-127">Request body</span></span>
<span data-ttu-id="094b5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="094b5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="094b5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="094b5-129">Response</span></span>

<span data-ttu-id="094b5-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [serviceUpdateMessage](../resources/serviceupdatemessage.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="094b5-130">If successful, this method returns a `200 OK` response code and a collection of [serviceUpdateMessage](../resources/serviceupdatemessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="094b5-131">Пример</span><span class="sxs-lookup"><span data-stu-id="094b5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="094b5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="094b5-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="094b5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="094b5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceupdatemessage"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages
```
# <a name="c"></a>[<span data-ttu-id="094b5-134">C#</span><span class="sxs-lookup"><span data-stu-id="094b5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceupdatemessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="094b5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="094b5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceupdatemessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="094b5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="094b5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceupdatemessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="094b5-137">Java</span><span class="sxs-lookup"><span data-stu-id="094b5-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceupdatemessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="094b5-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="094b5-138">Response</span></span>
><span data-ttu-id="094b5-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="094b5-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceUpdateMessage",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/messages",
  "value": [
    {
      "startDateTime": "2019-02-01T18:51:00Z",
      "endDateTime": "2019-06-01T08:00:00Z",
      "lastModifiedDateTime": "2021-01-08T01:10:06.843Z",
      "title": "(Updated) New feature: Changes to PowerPoint and Word to open files faster",
      "id": "MC172851",
      "category": "StayInformed",
      "severity": "Normal",
      "tags": [
        "Updated message"
      ],
      "isMajorChange": true,
      "actionRequiredByDateTime": null,
      "services": [
        "SharePoint Online",
        "OneDrive for Business"
      ],
      "details": [
        {
          "name": "ExternalLink",
          "value": "https://support.office.com/article/office-document-cache-settings-4b497318-ae4f-4a99-be42-b242b2e8b692"
        }
      ],
      "body": {
        "contentType": "Text",
        "content": "Updated January 07, 2021: Based on learnings from our early rings, we have made the decision to make additional changes to the code before we proceed with the rollout. We will update the Message center post once we re-start the rollout......"
      },
      "viewPoint": null
    }
  ]
}
```

