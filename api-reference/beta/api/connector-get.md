---
title: Получение соединителя
description: Извлечение свойств объекта соединителя.
localization_priority: Normal
ms.openlocfilehash: 59a27a24dbb0f91881c4be71c0715ce0c648c4d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833336"
---
# <a name="get-connector"></a><span data-ttu-id="2925c-103">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="2925c-103">Get connector</span></span>

> <span data-ttu-id="2925c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2925c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2925c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2925c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2925c-106">Извлечение свойств объекта соединителя.</span><span class="sxs-lookup"><span data-stu-id="2925c-106">Retrieve the properties of a connector object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2925c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2925c-107">Permissions</span></span>
<span data-ttu-id="2925c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2925c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2925c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2925c-110">Permission type</span></span>      | <span data-ttu-id="2925c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2925c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2925c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2925c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2925c-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2925c-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2925c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2925c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2925c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2925c-115">Not supported.</span></span>    |
|<span data-ttu-id="2925c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2925c-116">Application</span></span> | <span data-ttu-id="2925c-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2925c-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2925c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2925c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/members/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2925c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2925c-119">Optional query parameters</span></span>
<span data-ttu-id="2925c-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2925c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2925c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2925c-121">Request headers</span></span>
| <span data-ttu-id="2925c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2925c-122">Name</span></span>      |<span data-ttu-id="2925c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2925c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2925c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2925c-124">Authorization</span></span>  | <span data-ttu-id="2925c-125">Носителя.</span><span class="sxs-lookup"><span data-stu-id="2925c-125">Bearer.</span></span> <span data-ttu-id="2925c-126">Обязательное</span><span class="sxs-lookup"><span data-stu-id="2925c-126">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="2925c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2925c-127">Request body</span></span>
<span data-ttu-id="2925c-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2925c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2925c-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2925c-129">Response</span></span>

<span data-ttu-id="2925c-130">Успешно завершена, этот метод возвращает `200 OK` объект [соединителя](../resources/connector.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2925c-130">If successful, this method returns a `200 OK` response code and [connector](../resources/connector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2925c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2925c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2925c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2925c-132">Request</span></span>
<span data-ttu-id="2925c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2925c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors/{id}
```
##### <a name="response"></a><span data-ttu-id="2925c-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2925c-134">Response</span></span>
<span data-ttu-id="2925c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2925c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
