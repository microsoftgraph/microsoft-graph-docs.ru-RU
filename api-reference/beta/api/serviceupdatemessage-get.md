---
title: Get serviceUpdateMessage
description: Извлечение свойств и связей объекта serviceUpdateMessage.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: 088985c53ec0887eb98e4619780143d8ac8805a8
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208798"
---
# <a name="get-serviceupdatemessage"></a><span data-ttu-id="b6d56-103">Get serviceUpdateMessage</span><span class="sxs-lookup"><span data-stu-id="b6d56-103">Get serviceUpdateMessage</span></span>
<span data-ttu-id="b6d56-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6d56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6d56-105">Извлечение свойств и связей объекта [serviceUpdateMessage.](../resources/serviceupdatemessage.md)</span><span class="sxs-lookup"><span data-stu-id="b6d56-105">Retrieve the properties and relationships of a [serviceUpdateMessage](../resources/serviceupdatemessage.md) object.</span></span>

<span data-ttu-id="b6d56-106">Эта операция извлекает указанное сообщение обновления службы для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6d56-106">This operation retrieves a specified service update message for the tenant.</span></span> <span data-ttu-id="b6d56-107">Операция возвращает ошибку, если сообщение не существует для клиента.</span><span class="sxs-lookup"><span data-stu-id="b6d56-107">The operation returns an error if the message does not exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6d56-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6d56-108">Permissions</span></span>
<span data-ttu-id="b6d56-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6d56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6d56-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6d56-111">Permission type</span></span>|<span data-ttu-id="b6d56-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b6d56-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6d56-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6d56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6d56-114">ServiceMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6d56-114">ServiceMessage.Read.All</span></span>|
|<span data-ttu-id="b6d56-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6d56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6d56-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6d56-116">Not supported.</span></span>|
|<span data-ttu-id="b6d56-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b6d56-117">Application</span></span>|<span data-ttu-id="b6d56-118">ServiceMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6d56-118">ServiceMessage.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6d56-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6d56-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/messages/{serviceUpdateMessageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6d56-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b6d56-120">Optional query parameters</span></span>
<span data-ttu-id="b6d56-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b6d56-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6d56-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6d56-122">Request headers</span></span>
|<span data-ttu-id="b6d56-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b6d56-123">Name</span></span>|<span data-ttu-id="b6d56-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b6d56-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b6d56-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6d56-125">Authorization</span></span>|<span data-ttu-id="b6d56-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b6d56-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6d56-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6d56-128">Request body</span></span>
<span data-ttu-id="b6d56-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6d56-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6d56-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6d56-130">Response</span></span>

<span data-ttu-id="b6d56-131">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [serviceUpdateMessage](../resources/serviceupdatemessage.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b6d56-131">If successful, this method returns a `200 OK` response code and a [serviceUpdateMessage](../resources/serviceupdatemessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6d56-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b6d56-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6d56-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6d56-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b6d56-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6d56-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MC172851"],
  "name": "get_serviceupdatemessage"
}
-->

``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/messages/MC172851
```
# <a name="c"></a>[<span data-ttu-id="b6d56-135">C#</span><span class="sxs-lookup"><span data-stu-id="b6d56-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceupdatemessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b6d56-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b6d56-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceupdatemessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b6d56-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b6d56-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceupdatemessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b6d56-138">Java</span><span class="sxs-lookup"><span data-stu-id="b6d56-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceupdatemessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b6d56-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6d56-139">Response</span></span>
><span data-ttu-id="b6d56-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b6d56-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceUpdateMessage"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#admin/serviceAnnouncement/messages/$entity",
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
      "content": "Updated January 07, 2021: Based on learnings from our early rings, we have made the decision to make additional changes to the code before we proceed with the rollout. We will update the Message center post once we re-start the rollout.  Thank you for your patience........"
    },
    "viewPoint": null
}
```
