---
title: Соглашения по списку
description: Получение списка объектов соглашения.
localization_priority: Normal
ms.openlocfilehash: 3ae255a386986b5627aed99f29dca5bfb9934e30
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859922"
---
# <a name="list-agreements"></a><span data-ttu-id="ccd35-103">Соглашения по списку</span><span class="sxs-lookup"><span data-stu-id="ccd35-103">List agreements</span></span>

> <span data-ttu-id="ccd35-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ccd35-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ccd35-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccd35-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ccd35-106">Получение списка объектов [соглашения](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="ccd35-106">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ccd35-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ccd35-107">Permissions</span></span>
<span data-ttu-id="ccd35-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccd35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccd35-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ccd35-110">Permission type</span></span>                        | <span data-ttu-id="ccd35-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ccd35-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccd35-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ccd35-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ccd35-113">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccd35-113">Agreement.Read.All</span></span> |
|<span data-ttu-id="ccd35-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ccd35-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccd35-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccd35-115">Not supported.</span></span> |
|<span data-ttu-id="ccd35-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ccd35-116">Application</span></span>                            | <span data-ttu-id="ccd35-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ccd35-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccd35-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ccd35-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="ccd35-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccd35-119">Request headers</span></span>
| <span data-ttu-id="ccd35-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ccd35-120">Name</span></span>         | <span data-ttu-id="ccd35-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ccd35-121">Type</span></span>        | <span data-ttu-id="ccd35-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ccd35-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ccd35-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccd35-123">Authorization</span></span> | <span data-ttu-id="ccd35-124">string</span><span class="sxs-lookup"><span data-stu-id="ccd35-124">string</span></span> | <span data-ttu-id="ccd35-125">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="ccd35-125">Bearer \{token\}.</span></span> <span data-ttu-id="ccd35-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ccd35-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccd35-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ccd35-127">Request body</span></span>
<span data-ttu-id="ccd35-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ccd35-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ccd35-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ccd35-129">Response</span></span>
<span data-ttu-id="ccd35-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [соглашения](../resources/agreement.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ccd35-130">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ccd35-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ccd35-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ccd35-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ccd35-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
##### <a name="response"></a><span data-ttu-id="ccd35-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ccd35-133">Response</span></span>
><span data-ttu-id="ccd35-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ccd35-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
