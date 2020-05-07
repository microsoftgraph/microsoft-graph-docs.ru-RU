---
title: Получение Воркфорцеинтегратион
description: Получение свойств и связей объекта Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6e5c0909da255879bd09d8ddd3cb9011b68992bc
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154054"
---
# <a name="get-workforceintegration"></a><span data-ttu-id="ca106-103">Получение Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="ca106-103">Get workforceIntegration</span></span>

<span data-ttu-id="ca106-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca106-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ca106-105">Получение свойств и связей объекта [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="ca106-105">Retrieve the properties and relationships of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca106-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca106-106">Permissions</span></span>

<span data-ttu-id="ca106-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca106-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca106-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca106-109">Permission type</span></span>                        | <span data-ttu-id="ca106-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca106-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ca106-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca106-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca106-112">Воркфорцеинтегратион. Read. ALL, Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ca106-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="ca106-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca106-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca106-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca106-114">Not supported.</span></span> |
| <span data-ttu-id="ca106-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca106-115">Application</span></span>                            | <span data-ttu-id="ca106-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca106-116">Not supported.</span></span> |

> <span data-ttu-id="ca106-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="ca106-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ca106-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="ca106-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ca106-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca106-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations/workforceIntegrationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca106-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ca106-120">Optional query parameters</span></span>

<span data-ttu-id="ca106-121">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ca106-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ca106-122">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ca106-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca106-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca106-123">Request headers</span></span>

| <span data-ttu-id="ca106-124">Имя</span><span class="sxs-lookup"><span data-stu-id="ca106-124">Name</span></span>      |<span data-ttu-id="ca106-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ca106-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ca106-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca106-126">Authorization</span></span> | <span data-ttu-id="ca106-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca106-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca106-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca106-129">Request body</span></span>

<span data-ttu-id="ca106-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca106-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca106-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca106-131">Response</span></span>

<span data-ttu-id="ca106-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca106-132">If successful, this method returns a `200 OK` response code and the requested [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca106-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="ca106-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ca106-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca106-134">Request</span></span>

<span data-ttu-id="ca106-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca106-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceintegrationid}
```

---


### <a name="response"></a><span data-ttu-id="ca106-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca106-136">Response</span></span>

<span data-ttu-id="ca106-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ca106-137">The following is an example of the response.</span></span>

> <span data-ttu-id="ca106-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca106-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "KronosWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://contosoWorkforceIntegration.com/Contoso/",
  "supportedEntities": "shift"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
