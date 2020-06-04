---
title: Получение соединителя
description: Получение свойств объекта Connector.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f681179fbcc0f18890375d97f79cc2ccd0643cbc
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556089"
---
# <a name="get-connector"></a><span data-ttu-id="3432f-103">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="3432f-103">Get connector</span></span>

<span data-ttu-id="3432f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3432f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3432f-105">Получение свойств и связей объекта [Connector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="3432f-105">Retrieve the properties and relationships of a [connector](../resources/connector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3432f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3432f-106">Permissions</span></span>
<span data-ttu-id="3432f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3432f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3432f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3432f-109">Permission type</span></span>      | <span data-ttu-id="3432f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3432f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3432f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3432f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3432f-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3432f-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3432f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3432f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3432f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3432f-114">Not supported.</span></span>    |
|<span data-ttu-id="3432f-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="3432f-115">Application</span></span> | <span data-ttu-id="3432f-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3432f-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3432f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3432f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3432f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3432f-118">Optional query parameters</span></span>
<span data-ttu-id="3432f-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3432f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3432f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3432f-120">Request headers</span></span>
| <span data-ttu-id="3432f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3432f-121">Name</span></span>      |<span data-ttu-id="3432f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3432f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3432f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3432f-123">Authorization</span></span>  | <span data-ttu-id="3432f-124">Носителя.</span><span class="sxs-lookup"><span data-stu-id="3432f-124">Bearer.</span></span> <span data-ttu-id="3432f-125">Обязательное</span><span class="sxs-lookup"><span data-stu-id="3432f-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="3432f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3432f-126">Request body</span></span>
<span data-ttu-id="3432f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3432f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3432f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3432f-128">Response</span></span>

<span data-ttu-id="3432f-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Connector](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3432f-129">If successful, this method returns a `200 OK` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3432f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3432f-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3432f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3432f-131">Request</span></span>

<span data-ttu-id="3432f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3432f-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}
```
##### <a name="response"></a><span data-ttu-id="3432f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3432f-133">Response</span></span>
<span data-ttu-id="3432f-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3432f-134">The following is an example of the response.</span></span> <span data-ttu-id="3432f-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3432f-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3432f-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3432f-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 124

{
  "id": "id-value",
  "machineName": "machineName-value",
  "externalIp": "externalIp-value",
  "status": "status-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
