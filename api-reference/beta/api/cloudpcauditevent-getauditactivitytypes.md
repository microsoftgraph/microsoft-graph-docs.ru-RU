---
title: 'cloudPcAuditEvent: getAuditActivityTypes'
description: Получите типы действий аудита по id клиента.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 7ea6612160474c2fbbfde792f3565f1100dac146
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316982"
---
# <a name="cloudpcauditevent-getauditactivitytypes"></a><span data-ttu-id="8293d-103">cloudPcAuditEvent: getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="8293d-103">cloudPcAuditEvent: getAuditActivityTypes</span></span>

<span data-ttu-id="8293d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8293d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8293d-105">Получите типы действий аудита по ID клиента.</span><span class="sxs-lookup"><span data-stu-id="8293d-105">Get audit activity types by tenant ID.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="8293d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8293d-106">Permissions</span></span>

<span data-ttu-id="8293d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8293d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8293d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8293d-109">Permission type</span></span>| <span data-ttu-id="8293d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8293d-110">Permissions (from least to most privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="8293d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8293d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8293d-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8293d-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="8293d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8293d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8293d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8293d-114">Not supported.</span></span>|
|<span data-ttu-id="8293d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8293d-115">Application</span></span>|<span data-ttu-id="8293d-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8293d-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8293d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8293d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="8293d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8293d-118">Request headers</span></span>

| <span data-ttu-id="8293d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8293d-119">Name</span></span>          | <span data-ttu-id="8293d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8293d-120">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8293d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8293d-121">Authorization</span></span> | <span data-ttu-id="8293d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8293d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8293d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8293d-124">Request body</span></span>

<span data-ttu-id="8293d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8293d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8293d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8293d-126">Response</span></span>

<span data-ttu-id="8293d-127">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` строк в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8293d-127">If successful, this method returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8293d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8293d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8293d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8293d-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8293d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="8293d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cloudpcauditevent_getauditactivitytypes"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/auditEvents/getAuditActivityTypes
```
# <a name="c"></a>[<span data-ttu-id="8293d-131">C#</span><span class="sxs-lookup"><span data-stu-id="8293d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpcauditevent-getauditactivitytypes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8293d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8293d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpcauditevent-getauditactivitytypes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8293d-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8293d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpcauditevent-getauditactivitytypes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8293d-134">Java</span><span class="sxs-lookup"><span data-stu-id="8293d-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpcauditevent-getauditactivitytypes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8293d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8293d-135">Response</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```
