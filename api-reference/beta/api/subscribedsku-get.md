---
title: Вывод объекта SubscribedSku
description: Получение определенной коммерческой подписки, приобретенной организацией.
localization_priority: Normal
ms.openlocfilehash: a031e22e937f1c2b88538c70eb9456fb8c57b277
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863464"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="3b7ee-103">Вывод объекта SubscribedSku</span><span class="sxs-lookup"><span data-stu-id="3b7ee-103">Get subscribedSku</span></span>

> <span data-ttu-id="3b7ee-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3b7ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b7ee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b7ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3b7ee-106">Получение определенной коммерческой подписки, приобретенной организацией.</span><span class="sxs-lookup"><span data-stu-id="3b7ee-106">Retrieve a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b7ee-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b7ee-107">Permissions</span></span>
<span data-ttu-id="3b7ee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b7ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3b7ee-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b7ee-110">Permission type</span></span>      | <span data-ttu-id="3b7ee-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b7ee-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b7ee-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b7ee-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3b7ee-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3b7ee-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3b7ee-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b7ee-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b7ee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b7ee-115">Not supported.</span></span>    |
|<span data-ttu-id="3b7ee-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b7ee-116">Application</span></span> | <span data-ttu-id="3b7ee-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b7ee-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3b7ee-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b7ee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3b7ee-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3b7ee-119">Optional query parameters</span></span>
<span data-ttu-id="3b7ee-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3b7ee-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3b7ee-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b7ee-121">Request headers</span></span>
| <span data-ttu-id="3b7ee-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3b7ee-122">Name</span></span>       | <span data-ttu-id="3b7ee-123">Тип</span><span class="sxs-lookup"><span data-stu-id="3b7ee-123">Type</span></span> | <span data-ttu-id="3b7ee-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3b7ee-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3b7ee-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b7ee-125">Authorization</span></span>  | <span data-ttu-id="3b7ee-126">string</span><span class="sxs-lookup"><span data-stu-id="3b7ee-126">string</span></span>  | <span data-ttu-id="3b7ee-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b7ee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b7ee-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3b7ee-129">Request body</span></span>
<span data-ttu-id="3b7ee-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3b7ee-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b7ee-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b7ee-131">Response</span></span>

<span data-ttu-id="3b7ee-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscribedSku](../resources/subscribedsku.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b7ee-132">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b7ee-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3b7ee-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b7ee-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b7ee-134">Request</span></span>
<span data-ttu-id="3b7ee-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b7ee-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/beta/subscribedSkus/{id}
```
##### <a name="response"></a><span data-ttu-id="3b7ee-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b7ee-136">Response</span></span>
<span data-ttu-id="3b7ee-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3b7ee-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 450

{
  "capabilityStatus": "capabilityStatus-value",
  "consumedUnits": 99,
  "prepaidUnits": {
    "enabled": 99,
    "suspended": 99,
    "warning": 99
  },
  "servicePlans": [
    {
      "servicePlanId": "servicePlanId-value",
      "servicePlanName": "servicePlanName-value",
      "provisioningStatus": "provisioningStatus-value",
      "appliesTo": "appliesTo-value"
    }
  ],
  "skuId": "skuId-value",
  "skuPartNumber": "skuPartNumber-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscribedSku",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
