---
title: Получение соединителя
description: Получение свойств объекта Connector.
localization_priority: Normal
ms.openlocfilehash: da0a44864043e013b284e901786ba36a04fb143d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327553"
---
# <a name="get-connector"></a><span data-ttu-id="48563-103">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="48563-103">Get connector</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48563-104">Получение свойств объекта Connector.</span><span class="sxs-lookup"><span data-stu-id="48563-104">Retrieve the properties of a connector object.</span></span>
## <a name="permissions"></a><span data-ttu-id="48563-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48563-105">Permissions</span></span>
<span data-ttu-id="48563-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48563-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48563-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48563-108">Permission type</span></span>      | <span data-ttu-id="48563-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48563-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48563-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48563-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48563-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="48563-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="48563-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48563-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48563-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48563-113">Not supported.</span></span>    |
|<span data-ttu-id="48563-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="48563-114">Application</span></span> | <span data-ttu-id="48563-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48563-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48563-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48563-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/members/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="48563-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="48563-117">Optional query parameters</span></span>
<span data-ttu-id="48563-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="48563-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48563-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48563-119">Request headers</span></span>
| <span data-ttu-id="48563-120">Имя</span><span class="sxs-lookup"><span data-stu-id="48563-120">Name</span></span>      |<span data-ttu-id="48563-121">Описание</span><span class="sxs-lookup"><span data-stu-id="48563-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="48563-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="48563-122">Authorization</span></span>  | <span data-ttu-id="48563-123">Носителя.</span><span class="sxs-lookup"><span data-stu-id="48563-123">Bearer.</span></span> <span data-ttu-id="48563-124">Обязательный</span><span class="sxs-lookup"><span data-stu-id="48563-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="48563-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48563-125">Request body</span></span>
<span data-ttu-id="48563-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="48563-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48563-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="48563-127">Response</span></span>

<span data-ttu-id="48563-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Connector](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48563-128">If successful, this method returns a `200 OK` response code and [connector](../resources/connector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="48563-129">Пример</span><span class="sxs-lookup"><span data-stu-id="48563-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48563-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="48563-130">Request</span></span>
<span data-ttu-id="48563-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48563-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors/{id}
```
##### <a name="response"></a><span data-ttu-id="48563-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="48563-132">Response</span></span>
<span data-ttu-id="48563-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48563-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
