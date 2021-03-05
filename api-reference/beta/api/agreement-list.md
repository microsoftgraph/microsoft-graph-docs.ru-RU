---
title: Список соглашений
description: Извлечение списка объектов соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 13bc5308f12ce83e03177f79df1264cca9b35bf1
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471585"
---
# <a name="list-agreements"></a><span data-ttu-id="8b21b-103">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="8b21b-103">List agreements</span></span>

<span data-ttu-id="8b21b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b21b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b21b-105">Извлечение списка [объектов](../resources/agreement.md) соглашения.</span><span class="sxs-lookup"><span data-stu-id="8b21b-105">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b21b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b21b-106">Permissions</span></span>
<span data-ttu-id="8b21b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b21b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b21b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b21b-109">Permission type</span></span>                        | <span data-ttu-id="8b21b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b21b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b21b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b21b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8b21b-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b21b-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="8b21b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b21b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b21b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b21b-114">Not supported.</span></span> |
|<span data-ttu-id="8b21b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b21b-115">Application</span></span>                            | <span data-ttu-id="8b21b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b21b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b21b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b21b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="8b21b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b21b-118">Request headers</span></span>
| <span data-ttu-id="8b21b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8b21b-119">Name</span></span>         | <span data-ttu-id="8b21b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8b21b-120">Type</span></span>        | <span data-ttu-id="8b21b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8b21b-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8b21b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b21b-122">Authorization</span></span> | <span data-ttu-id="8b21b-123">string</span><span class="sxs-lookup"><span data-stu-id="8b21b-123">string</span></span> | <span data-ttu-id="8b21b-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b21b-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b21b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b21b-126">Request body</span></span>
<span data-ttu-id="8b21b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b21b-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8b21b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b21b-128">Response</span></span>
<span data-ttu-id="8b21b-129">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` соглашения в тексте отклика. [](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="8b21b-129">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b21b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8b21b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b21b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b21b-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements
```

##### <a name="response"></a><span data-ttu-id="8b21b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b21b-132">Response</span></span>
><span data-ttu-id="8b21b-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b21b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
