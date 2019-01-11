---
title: Получение конечной точки
description: Извлечение свойств и связи объекта определенной конечной точки.
localization_priority: Normal
ms.openlocfilehash: 77ad5716e8e30a16f95bf62593a6530d5e759861
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820449"
---
# <a name="get-endpoint"></a><span data-ttu-id="5c5ed-103">Получение конечной точки</span><span class="sxs-lookup"><span data-stu-id="5c5ed-103">Get endpoint</span></span>

> <span data-ttu-id="5c5ed-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5c5ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c5ed-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c5ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c5ed-106">Извлечение свойств и связи объекта определенного [конечной точки](../resources/endpoint.md) .</span><span class="sxs-lookup"><span data-stu-id="5c5ed-106">Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c5ed-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c5ed-107">Permissions</span></span>
<span data-ttu-id="5c5ed-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c5ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5c5ed-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c5ed-110">Permission type</span></span>      | <span data-ttu-id="5c5ed-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c5ed-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c5ed-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c5ed-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5c5ed-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5ed-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c5ed-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c5ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c5ed-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c5ed-115">Not supported.</span></span>    |
|<span data-ttu-id="5c5ed-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c5ed-116">Application</span></span> | <span data-ttu-id="5c5ed-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5ed-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c5ed-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c5ed-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5c5ed-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c5ed-119">Optional query parameters</span></span>
<span data-ttu-id="5c5ed-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5c5ed-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c5ed-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c5ed-121">Request headers</span></span>
| <span data-ttu-id="5c5ed-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5c5ed-122">Name</span></span>      |<span data-ttu-id="5c5ed-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5c5ed-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5c5ed-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c5ed-124">Authorization</span></span>  | <span data-ttu-id="5c5ed-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c5ed-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="5c5ed-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c5ed-127">Content-Type</span></span>   | <span data-ttu-id="5c5ed-128">Application/Json</span><span class="sxs-lookup"><span data-stu-id="5c5ed-128">Application/Json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c5ed-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c5ed-129">Request body</span></span>
<span data-ttu-id="5c5ed-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c5ed-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c5ed-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="5c5ed-131">Response</span></span>

<span data-ttu-id="5c5ed-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [конечной точки](../resources/endpoint.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5c5ed-132">If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5c5ed-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5c5ed-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c5ed-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c5ed-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
##### <a name="response"></a><span data-ttu-id="5c5ed-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c5ed-135">Response</span></span>
<span data-ttu-id="5c5ed-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c5ed-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Endpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 208

{
  "capability": "Conversations",
  "providerId": "{Yammer GUID}",
  "providerName": "Yammer",
  "uri": "uri-value",
  "providerResourceId": "Yammer.FeedURL",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Endpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
