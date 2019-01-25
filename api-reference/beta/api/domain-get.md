---
title: Получение домена
description: Получение свойств и связей объекта домена.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 03dcc7f5eff084ec79cb39a60688aadfaf0d63fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514539"
---
# <a name="get-domain"></a><span data-ttu-id="bafbd-103">Получение домена</span><span class="sxs-lookup"><span data-stu-id="bafbd-103">Get domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bafbd-104">Получение свойств и связей объекта домена.</span><span class="sxs-lookup"><span data-stu-id="bafbd-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bafbd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bafbd-105">Permissions</span></span>

<span data-ttu-id="bafbd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bafbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bafbd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bafbd-108">Permission type</span></span>      | <span data-ttu-id="bafbd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bafbd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bafbd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bafbd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bafbd-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bafbd-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="bafbd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bafbd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bafbd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bafbd-113">Not supported.</span></span>    |
|<span data-ttu-id="bafbd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bafbd-114">Application</span></span> | <span data-ttu-id="bafbd-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bafbd-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bafbd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bafbd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="bafbd-117">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="bafbd-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="bafbd-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bafbd-118">Optional query parameters</span></span>

<span data-ttu-id="bafbd-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bafbd-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bafbd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bafbd-120">Request headers</span></span>

| <span data-ttu-id="bafbd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="bafbd-121">Name</span></span>      |<span data-ttu-id="bafbd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bafbd-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bafbd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bafbd-123">Authorization</span></span>  | <span data-ttu-id="bafbd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bafbd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bafbd-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bafbd-126">Content-Type</span></span>  | <span data-ttu-id="bafbd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bafbd-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bafbd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bafbd-128">Request body</span></span>
<span data-ttu-id="bafbd-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bafbd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bafbd-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="bafbd-130">Response</span></span>

<span data-ttu-id="bafbd-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bafbd-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bafbd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bafbd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bafbd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bafbd-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="bafbd-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="bafbd-134">Response</span></span>
<span data-ttu-id="bafbd-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bafbd-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
