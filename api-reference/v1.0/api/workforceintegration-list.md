---
title: Список Воркфорцеинтегратионс
description: Получение списка объектов Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6f5e37feb028e5929bdb48ccf54b62083de9cbc9
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154047"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="b3662-103">Список Воркфорцеинтегратионс</span><span class="sxs-lookup"><span data-stu-id="b3662-103">List workforceIntegrations</span></span>

<span data-ttu-id="b3662-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3662-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3662-105">Получение списка объектов [воркфорцеинтегратион](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="b3662-105">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3662-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b3662-106">Permissions</span></span>

<span data-ttu-id="b3662-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3662-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3662-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b3662-109">Permission type</span></span>                        | <span data-ttu-id="b3662-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b3662-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b3662-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b3662-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="b3662-112">Воркфорцеинтегратион. Read. ALL, Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b3662-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="b3662-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b3662-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3662-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3662-114">Not supported.</span></span> |
| <span data-ttu-id="b3662-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b3662-115">Application</span></span>                            | <span data-ttu-id="b3662-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3662-116">Not supported.</span></span> |

> <span data-ttu-id="b3662-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="b3662-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b3662-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="b3662-118">Global admins can access groups that they are not a member of.</span></span>


## <a name="http-request"></a><span data-ttu-id="b3662-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b3662-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3662-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b3662-120">Optional query parameters</span></span>

<span data-ttu-id="b3662-121">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b3662-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b3662-122">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b3662-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3662-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b3662-123">Request headers</span></span>

| <span data-ttu-id="b3662-124">Имя</span><span class="sxs-lookup"><span data-stu-id="b3662-124">Name</span></span>      |<span data-ttu-id="b3662-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b3662-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b3662-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b3662-126">Authorization</span></span> | <span data-ttu-id="b3662-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b3662-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3662-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b3662-129">Request body</span></span>

<span data-ttu-id="b3662-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b3662-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3662-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3662-131">Response</span></span>

<span data-ttu-id="b3662-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [воркфорцеинтегратион](../resources/workforceintegration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b3662-132">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3662-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="b3662-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3662-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b3662-134">Request</span></span>

<span data-ttu-id="b3662-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b3662-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations
```

---


### <a name="response"></a><span data-ttu-id="b3662-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b3662-136">Response</span></span>

<span data-ttu-id="b3662-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b3662-137">The following is an example of the response.</span></span>

> <span data-ttu-id="b3662-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b3662-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "displayName-value",
      "apiVersion": 99,
      "encryption": {
        "protocol": "protocol-value",
        "secret": "secret-value"
      },
      "isActive": true,
      "url": "url-value",
      "supportedEntities": "supportedEntities-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List workforceIntegrations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
