---
title: Получение соглашения
description: Извлечение свойств и связи объекта соглашения.
ms.openlocfilehash: 9887ed39bcb2a63980388e5265bb56d6500625d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076318"
---
# <a name="get-agreement"></a><span data-ttu-id="94aa9-103">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="94aa9-103">Get agreement</span></span>

> <span data-ttu-id="94aa9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="94aa9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94aa9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94aa9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94aa9-106">Извлечение свойств и связи объекта [соглашения](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="94aa9-106">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="94aa9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94aa9-107">Permissions</span></span>
<span data-ttu-id="94aa9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94aa9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94aa9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94aa9-110">Permission type</span></span>                        | <span data-ttu-id="94aa9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94aa9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="94aa9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94aa9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="94aa9-113">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="94aa9-113">Agreement.Read.All</span></span> |
|<span data-ttu-id="94aa9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94aa9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94aa9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94aa9-115">Not supported.</span></span> |
|<span data-ttu-id="94aa9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94aa9-116">Application</span></span>                            | <span data-ttu-id="94aa9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94aa9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94aa9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94aa9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="94aa9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94aa9-119">Request headers</span></span>
| <span data-ttu-id="94aa9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="94aa9-120">Name</span></span>         | <span data-ttu-id="94aa9-121">Тип</span><span class="sxs-lookup"><span data-stu-id="94aa9-121">Type</span></span>        | <span data-ttu-id="94aa9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="94aa9-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="94aa9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94aa9-123">Authorization</span></span> | <span data-ttu-id="94aa9-124">string</span><span class="sxs-lookup"><span data-stu-id="94aa9-124">string</span></span> | <span data-ttu-id="94aa9-125">Носителя \{маркеров\}.</span><span class="sxs-lookup"><span data-stu-id="94aa9-125">Bearer \{token\}.</span></span> <span data-ttu-id="94aa9-126">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="94aa9-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94aa9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94aa9-127">Request body</span></span>
<span data-ttu-id="94aa9-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94aa9-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="94aa9-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="94aa9-129">Response</span></span>
<span data-ttu-id="94aa9-130">Успешно завершена, этот метод возвращает `200 OK` объект [соглашение](../resources/agreement.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="94aa9-130">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94aa9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="94aa9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94aa9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="94aa9-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
##### <a name="response"></a><span data-ttu-id="94aa9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="94aa9-133">Response</span></span>
><span data-ttu-id="94aa9-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="94aa9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "id-value",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
