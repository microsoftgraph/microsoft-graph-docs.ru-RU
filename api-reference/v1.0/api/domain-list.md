---
title: Перечисление доменов
description: Получение списка объектов домена.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4039995fc8b588b3a6a318b457e0eaba28b8dfa6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927351"
---
# <a name="list-domains"></a><span data-ttu-id="024c7-103">Перечисление доменов</span><span class="sxs-lookup"><span data-stu-id="024c7-103">List domains</span></span>

<span data-ttu-id="024c7-104">Получение списка объектов домена.</span><span class="sxs-lookup"><span data-stu-id="024c7-104">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="024c7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="024c7-105">Permissions</span></span>
<span data-ttu-id="024c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="024c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="024c7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="024c7-108">Permission type</span></span>      | <span data-ttu-id="024c7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="024c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="024c7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="024c7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="024c7-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="024c7-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="024c7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="024c7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="024c7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="024c7-113">Not supported.</span></span>    |
|<span data-ttu-id="024c7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="024c7-114">Application</span></span> | <span data-ttu-id="024c7-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="024c7-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="024c7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="024c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="024c7-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="024c7-117">Optional query parameters</span></span>
<span data-ttu-id="024c7-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="024c7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="024c7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="024c7-119">Request headers</span></span>
| <span data-ttu-id="024c7-120">Имя</span><span class="sxs-lookup"><span data-stu-id="024c7-120">Name</span></span>      |<span data-ttu-id="024c7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="024c7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="024c7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="024c7-122">Authorization</span></span>  | <span data-ttu-id="024c7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="024c7-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="024c7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="024c7-125">Accept</span></span>         | <span data-ttu-id="024c7-126">application/json;</span><span class="sxs-lookup"><span data-stu-id="024c7-126">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="024c7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="024c7-127">Request body</span></span>
<span data-ttu-id="024c7-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="024c7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="024c7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="024c7-129">Response</span></span>

<span data-ttu-id="024c7-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="024c7-130">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="024c7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="024c7-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="024c7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="024c7-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains
```
##### <a name="response"></a><span data-ttu-id="024c7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="024c7-133">Response</span></span>
<span data-ttu-id="024c7-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="024c7-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "contoso.com",
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
<!-- {
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
