---
title: Получение соглашения
description: Извлечение свойств и связей объекта соглашения.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 0218eeb4be68ded4d6e644ac0998be563c239b83
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722694"
---
# <a name="get-agreement"></a><span data-ttu-id="b5fc9-103">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="b5fc9-103">Get agreement</span></span>

<span data-ttu-id="b5fc9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5fc9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5fc9-105">Извлечение свойств и связей объекта [соглашения.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="b5fc9-105">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5fc9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5fc9-106">Permissions</span></span>
<span data-ttu-id="b5fc9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5fc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5fc9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5fc9-109">Permission type</span></span>                        | <span data-ttu-id="b5fc9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5fc9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5fc9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5fc9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5fc9-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5fc9-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="b5fc9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5fc9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5fc9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5fc9-114">Not supported.</span></span> |
|<span data-ttu-id="b5fc9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5fc9-115">Application</span></span>                            | <span data-ttu-id="b5fc9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5fc9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5fc9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5fc9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5fc9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b5fc9-118">Optional query parameters</span></span>
<span data-ttu-id="b5fc9-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b5fc9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5fc9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5fc9-120">Request headers</span></span>
| <span data-ttu-id="b5fc9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b5fc9-121">Name</span></span>         | <span data-ttu-id="b5fc9-122">Тип</span><span class="sxs-lookup"><span data-stu-id="b5fc9-122">Type</span></span>        | <span data-ttu-id="b5fc9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b5fc9-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b5fc9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5fc9-124">Authorization</span></span> | <span data-ttu-id="b5fc9-125">string</span><span class="sxs-lookup"><span data-stu-id="b5fc9-125">string</span></span> | <span data-ttu-id="b5fc9-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5fc9-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5fc9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5fc9-128">Request body</span></span>
<span data-ttu-id="b5fc9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5fc9-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b5fc9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5fc9-130">Response</span></span>
<span data-ttu-id="b5fc9-131">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` соглашения в тексте ответа. [](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="b5fc9-131">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5fc9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b5fc9-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5fc9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5fc9-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be?$expand=files
```

### <a name="response"></a><span data-ttu-id="b5fc9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5fc9-134">Response</span></span>
><span data-ttu-id="b5fc9-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5fc9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "id": "093b947f-8363-4979-a47d-4c52b33ee1be",
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
