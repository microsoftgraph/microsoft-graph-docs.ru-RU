---
title: Получение соединителя
description: Получение свойств объекта Connector.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: b8e8fc8bc23726c31244c989dc2821e56bb36908
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437793"
---
# <a name="get-connector"></a><span data-ttu-id="43828-103">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="43828-103">Get connector</span></span>

<span data-ttu-id="43828-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="43828-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43828-105">Получение свойств объекта Connector.</span><span class="sxs-lookup"><span data-stu-id="43828-105">Retrieve the properties of a connector object.</span></span>
## <a name="permissions"></a><span data-ttu-id="43828-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43828-106">Permissions</span></span>
<span data-ttu-id="43828-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43828-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43828-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43828-109">Permission type</span></span>      | <span data-ttu-id="43828-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43828-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43828-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43828-111">Delegated (work or school account)</span></span> | <span data-ttu-id="43828-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="43828-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="43828-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43828-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43828-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43828-114">Not supported.</span></span>    |
|<span data-ttu-id="43828-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43828-115">Application</span></span> | <span data-ttu-id="43828-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43828-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43828-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43828-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/members/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="43828-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="43828-118">Optional query parameters</span></span>
<span data-ttu-id="43828-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="43828-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43828-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43828-120">Request headers</span></span>
| <span data-ttu-id="43828-121">Имя</span><span class="sxs-lookup"><span data-stu-id="43828-121">Name</span></span>      |<span data-ttu-id="43828-122">Описание</span><span class="sxs-lookup"><span data-stu-id="43828-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="43828-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43828-123">Authorization</span></span>  | <span data-ttu-id="43828-124">Носителя.</span><span class="sxs-lookup"><span data-stu-id="43828-124">Bearer.</span></span> <span data-ttu-id="43828-125">Обязательна</span><span class="sxs-lookup"><span data-stu-id="43828-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="43828-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43828-126">Request body</span></span>
<span data-ttu-id="43828-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="43828-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43828-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="43828-128">Response</span></span>

<span data-ttu-id="43828-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Connector](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43828-129">If successful, this method returns a `200 OK` response code and [connector](../resources/connector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="43828-130">Пример</span><span class="sxs-lookup"><span data-stu-id="43828-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="43828-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="43828-131">Request</span></span>
<span data-ttu-id="43828-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43828-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors/{id}
```
##### <a name="response"></a><span data-ttu-id="43828-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="43828-133">Response</span></span>
<span data-ttu-id="43828-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43828-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
