---
title: 'serviceHealthIssue: incidentReport'
description: Предосмотрить документ по проверке после инцидента (PIR) указанной проблемы службы для клиента.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: apiPageType
ms.openlocfilehash: c04a5c25ed5cd21f09f5f44066737a0337259663
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107858"
---
# <a name="servicehealthissue-incidentreport"></a><span data-ttu-id="2cc1a-103">serviceHealthIssue: incidentReport</span><span class="sxs-lookup"><span data-stu-id="2cc1a-103">serviceHealthIssue: incidentReport</span></span>
<span data-ttu-id="2cc1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cc1a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cc1a-105">Предосмотрить документ по проверке после инцидента (PIR) указанной проблемы службы для клиента.</span><span class="sxs-lookup"><span data-stu-id="2cc1a-105">Provide the Post-Incident Review (PIR) document of a specified service issue for tenant.</span></span>

<span data-ttu-id="2cc1a-106">Операция возвращает ошибку, если указанная проблема не существует для клиента.</span><span class="sxs-lookup"><span data-stu-id="2cc1a-106">The operation returns an error if the specified issue doesn't exist for the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cc1a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2cc1a-107">Permissions</span></span>
<span data-ttu-id="2cc1a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2cc1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cc1a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2cc1a-110">Permission type</span></span>|<span data-ttu-id="2cc1a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2cc1a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cc1a-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2cc1a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2cc1a-113">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cc1a-113">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="2cc1a-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2cc1a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cc1a-115">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cc1a-115">ServiceHealth.Read.All</span></span>|
|<span data-ttu-id="2cc1a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2cc1a-116">Application</span></span>|<span data-ttu-id="2cc1a-117">ServiceHealth.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cc1a-117">ServiceHealth.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cc1a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2cc1a-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/serviceAnnouncement/issues/{serviceHealthIssueId}/incidentReport
```

## <a name="request-headers"></a><span data-ttu-id="2cc1a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2cc1a-119">Request headers</span></span>
|<span data-ttu-id="2cc1a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2cc1a-120">Name</span></span>|<span data-ttu-id="2cc1a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2cc1a-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2cc1a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2cc1a-122">Authorization</span></span>|<span data-ttu-id="2cc1a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2cc1a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cc1a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2cc1a-125">Request body</span></span>
<span data-ttu-id="2cc1a-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2cc1a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cc1a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cc1a-127">Response</span></span>

<span data-ttu-id="2cc1a-128">В случае успешной работы эта функция возвращает код отклика и поток файлов `200 OK` в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2cc1a-128">If successful, this function returns a `200 OK` response code and a file stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cc1a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2cc1a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cc1a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2cc1a-130">Request</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["MO248163"],
  "name": "servicehealthissue_incidentreport"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/serviceAnnouncement/issues/MO248163/incidentReport
```


### <a name="response"></a><span data-ttu-id="2cc1a-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2cc1a-131">Response</span></span>
><span data-ttu-id="2cc1a-132">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2cc1a-132">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": "Stream"
}
```

