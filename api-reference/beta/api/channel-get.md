---
title: Получение канала
description: Извлечение свойств и связи канала.
ms.openlocfilehash: 977484c57d7d82d13b781f658bb53eea091e2066
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079456"
---
# <a name="get-channel"></a><span data-ttu-id="65cb3-103">Получение канала</span><span class="sxs-lookup"><span data-stu-id="65cb3-103">Get channel</span></span>

> <span data-ttu-id="65cb3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="65cb3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65cb3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65cb3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65cb3-106">Извлечение свойств и связи [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="65cb3-106">Retrieve the properties and relationships of a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="65cb3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65cb3-107">Permissions</span></span>
<span data-ttu-id="65cb3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65cb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65cb3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65cb3-110">Permission type</span></span>      | <span data-ttu-id="65cb3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65cb3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65cb3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65cb3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="65cb3-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65cb3-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="65cb3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65cb3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65cb3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65cb3-115">Not supported.</span></span>    |
|<span data-ttu-id="65cb3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65cb3-116">Application</span></span> | <span data-ttu-id="65cb3-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65cb3-117">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="65cb3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65cb3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}

```

## <a name="optional-query-parameters"></a><span data-ttu-id="65cb3-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="65cb3-119">Optional query parameters</span></span>

<span data-ttu-id="65cb3-120">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="65cb3-120">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65cb3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65cb3-121">Request headers</span></span>
| <span data-ttu-id="65cb3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65cb3-122">Header</span></span>       | <span data-ttu-id="65cb3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="65cb3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="65cb3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65cb3-124">Authorization</span></span>  | <span data-ttu-id="65cb3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65cb3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="65cb3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65cb3-127">Request body</span></span>
<span data-ttu-id="65cb3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="65cb3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65cb3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="65cb3-129">Response</span></span>

<span data-ttu-id="65cb3-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [канала](../resources/channel.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="65cb3-130">If successful, this method returns a `200 OK` response code and a [channel](../resources/channel.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="65cb3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="65cb3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65cb3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="65cb3-132">Request</span></span>
<span data-ttu-id="65cb3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65cb3-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}
```
##### <a name="response"></a><span data-ttu-id="65cb3-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="65cb3-134">Response</span></span>
<span data-ttu-id="65cb3-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="65cb3-135">Here is an example of the response.</span></span> 

><span data-ttu-id="65cb3-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65cb3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "description": "description-value",
    "displayName": "display-name-value",
    "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
