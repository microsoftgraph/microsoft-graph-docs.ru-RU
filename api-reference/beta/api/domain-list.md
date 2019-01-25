---
title: Перечисление доменов
description: Получение списка объектов домена.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7cbc4237d7fad61366102a25b65ffd4718c61d62
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512152"
---
# <a name="list-domains"></a><span data-ttu-id="16185-103">Перечисление доменов</span><span class="sxs-lookup"><span data-stu-id="16185-103">List domains</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16185-104">Получение списка объектов домена.</span><span class="sxs-lookup"><span data-stu-id="16185-104">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="16185-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16185-105">Permissions</span></span>
<span data-ttu-id="16185-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16185-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16185-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16185-108">Permission type</span></span>      | <span data-ttu-id="16185-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16185-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16185-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16185-110">Delegated (work or school account)</span></span> | <span data-ttu-id="16185-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="16185-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="16185-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16185-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16185-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16185-113">Not supported.</span></span>    |
|<span data-ttu-id="16185-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16185-114">Application</span></span> | <span data-ttu-id="16185-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16185-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16185-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16185-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="16185-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="16185-117">Optional query parameters</span></span>
<span data-ttu-id="16185-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="16185-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16185-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16185-119">Request headers</span></span>
| <span data-ttu-id="16185-120">Имя</span><span class="sxs-lookup"><span data-stu-id="16185-120">Name</span></span>      |<span data-ttu-id="16185-121">Описание</span><span class="sxs-lookup"><span data-stu-id="16185-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="16185-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16185-122">Authorization</span></span>  | <span data-ttu-id="16185-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16185-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="16185-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16185-125">Accept</span></span>         | <span data-ttu-id="16185-126">application/json;</span><span class="sxs-lookup"><span data-stu-id="16185-126">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="16185-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="16185-127">Request body</span></span>
<span data-ttu-id="16185-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16185-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16185-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="16185-129">Response</span></span>

<span data-ttu-id="16185-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="16185-130">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="16185-131">Пример</span><span class="sxs-lookup"><span data-stu-id="16185-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16185-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="16185-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/beta/domains
```
##### <a name="response"></a><span data-ttu-id="16185-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="16185-133">Response</span></span>
<span data-ttu-id="16185-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16185-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "name": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
