---
title: Получение соглашения
description: Извлечение свойств и связей объекта соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 1ba280d6899574303385e3b71959268a7d71c787
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471602"
---
# <a name="get-agreement"></a><span data-ttu-id="75934-103">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="75934-103">Get agreement</span></span>

<span data-ttu-id="75934-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75934-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75934-105">Извлечение свойств и связей объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="75934-105">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="75934-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75934-106">Permissions</span></span>
<span data-ttu-id="75934-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75934-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75934-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75934-109">Permission type</span></span>                        | <span data-ttu-id="75934-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75934-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="75934-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75934-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="75934-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="75934-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="75934-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75934-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75934-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75934-114">Not supported.</span></span> |
|<span data-ttu-id="75934-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75934-115">Application</span></span>                            | <span data-ttu-id="75934-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75934-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75934-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75934-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements/{id}
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="75934-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75934-118">Request headers</span></span>
| <span data-ttu-id="75934-119">Имя</span><span class="sxs-lookup"><span data-stu-id="75934-119">Name</span></span>         | <span data-ttu-id="75934-120">Тип</span><span class="sxs-lookup"><span data-stu-id="75934-120">Type</span></span>        | <span data-ttu-id="75934-121">Описание</span><span class="sxs-lookup"><span data-stu-id="75934-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="75934-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="75934-122">Authorization</span></span> | <span data-ttu-id="75934-123">string</span><span class="sxs-lookup"><span data-stu-id="75934-123">string</span></span> | <span data-ttu-id="75934-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75934-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75934-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75934-126">Request body</span></span>
<span data-ttu-id="75934-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75934-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="75934-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="75934-128">Response</span></span>
<span data-ttu-id="75934-129">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` соглашения в тексте ответа. [](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="75934-129">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="75934-130">Пример</span><span class="sxs-lookup"><span data-stu-id="75934-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75934-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="75934-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}?$expand=files
```

##### <a name="response"></a><span data-ttu-id="75934-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="75934-132">Response</span></span>
><span data-ttu-id="75934-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75934-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
