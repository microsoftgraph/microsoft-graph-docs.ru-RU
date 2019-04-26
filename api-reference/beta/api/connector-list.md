---
title: Список соединителей
description: Получение списка объектов Connector.
localization_priority: Normal
ms.openlocfilehash: 69e70bbf0f247b4d702f9cea2e69e2cddcce6272
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327688"
---
# <a name="list-connectors"></a><span data-ttu-id="e40cb-103">Список соединителей</span><span class="sxs-lookup"><span data-stu-id="e40cb-103">List connectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e40cb-104">Получение списка объектов Connector.</span><span class="sxs-lookup"><span data-stu-id="e40cb-104">Retrieve a list of connector objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e40cb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e40cb-105">Permissions</span></span>
<span data-ttu-id="e40cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e40cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e40cb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e40cb-108">Permission type</span></span>      | <span data-ttu-id="e40cb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e40cb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e40cb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e40cb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e40cb-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e40cb-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e40cb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e40cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e40cb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e40cb-113">Not supported.</span></span>    |
|<span data-ttu-id="e40cb-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="e40cb-114">Application</span></span> | <span data-ttu-id="e40cb-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e40cb-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e40cb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e40cb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e40cb-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e40cb-117">Optional query parameters</span></span>
<span data-ttu-id="e40cb-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e40cb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e40cb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e40cb-119">Request headers</span></span>
| <span data-ttu-id="e40cb-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e40cb-120">Name</span></span>      |<span data-ttu-id="e40cb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e40cb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e40cb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e40cb-122">Authorization</span></span>  | <span data-ttu-id="e40cb-123">Носителя.</span><span class="sxs-lookup"><span data-stu-id="e40cb-123">Bearer.</span></span> <span data-ttu-id="e40cb-124">Обязательный</span><span class="sxs-lookup"><span data-stu-id="e40cb-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="e40cb-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e40cb-125">Request body</span></span>
<span data-ttu-id="e40cb-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e40cb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e40cb-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="e40cb-127">Response</span></span>

<span data-ttu-id="e40cb-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Connector](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e40cb-128">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e40cb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="e40cb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e40cb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e40cb-130">Request</span></span>
<span data-ttu-id="e40cb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e40cb-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors
```
##### <a name="response"></a><span data-ttu-id="e40cb-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e40cb-132">Response</span></span>
<span data-ttu-id="e40cb-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e40cb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "value": [
    {
      "id": "id-value",
      "machineName": "machineName-value",
      "externalIp": "externalIp-value",
      "status": "status-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
