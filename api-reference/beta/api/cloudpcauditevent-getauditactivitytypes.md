---
title: 'cloudPcAuditEvent: getAuditActivityTypes'
description: Получите типы действий аудита по id клиента.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: a6e5fd01d0b2100affa6b5d89c43a50cddbaa533
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211337"
---
# <a name="cloudpcauditevent-getauditactivitytypes"></a><span data-ttu-id="95d8c-103">cloudPcAuditEvent: getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="95d8c-103">cloudPcAuditEvent: getAuditActivityTypes</span></span>

<span data-ttu-id="95d8c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95d8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95d8c-105">Получите типы действий аудита по ID клиента.</span><span class="sxs-lookup"><span data-stu-id="95d8c-105">Get audit activity types by tenant ID.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="95d8c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95d8c-106">Permissions</span></span>

<span data-ttu-id="95d8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95d8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95d8c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95d8c-109">Permission type</span></span>| <span data-ttu-id="95d8c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95d8c-110">Permissions (from least to most privileged)</span></span> |
|:---|:---|
|<span data-ttu-id="95d8c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95d8c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="95d8c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95d8c-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="95d8c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95d8c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95d8c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95d8c-114">Not supported.</span></span>|
|<span data-ttu-id="95d8c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="95d8c-115">Application</span></span>|<span data-ttu-id="95d8c-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95d8c-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95d8c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95d8c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="95d8c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95d8c-118">Request headers</span></span>

| <span data-ttu-id="95d8c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="95d8c-119">Name</span></span>          | <span data-ttu-id="95d8c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="95d8c-120">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="95d8c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95d8c-121">Authorization</span></span> | <span data-ttu-id="95d8c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95d8c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95d8c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95d8c-124">Request body</span></span>

<span data-ttu-id="95d8c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95d8c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95d8c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="95d8c-126">Response</span></span>

<span data-ttu-id="95d8c-127">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` строк в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="95d8c-127">If successful, this method returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="95d8c-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="95d8c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="95d8c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="95d8c-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "cloudpcauditevent_getauditactivitytypes"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/auditEvents/getAuditActivityTypes
```

### <a name="response"></a><span data-ttu-id="95d8c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="95d8c-130">Response</span></span>


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
