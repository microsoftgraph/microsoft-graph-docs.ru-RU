---
title: Перечисление contract
description: Получение списка объектов contract, сопоставленных с клиентом партнера.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b4003bf2aaa910d3ad33e299a9fdb01f47229d1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932982"
---
# <a name="list-contracts"></a><span data-ttu-id="1db55-103">Перечисление contract</span><span class="sxs-lookup"><span data-stu-id="1db55-103">List contracts</span></span>

<span data-ttu-id="1db55-104">Получение списка объектов [contract](../resources/contract.md), сопоставленных с клиентом партнера.</span><span class="sxs-lookup"><span data-stu-id="1db55-104">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="1db55-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1db55-105">Permissions</span></span>

<span data-ttu-id="1db55-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1db55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1db55-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1db55-108">Permission type</span></span>      | <span data-ttu-id="1db55-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1db55-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1db55-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1db55-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1db55-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1db55-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1db55-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1db55-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1db55-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1db55-113">Not supported.</span></span>    |
|<span data-ttu-id="1db55-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1db55-114">Application</span></span> | <span data-ttu-id="1db55-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1db55-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1db55-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1db55-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1db55-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1db55-117">Optional query parameters</span></span>

<span data-ttu-id="1db55-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1db55-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="1db55-119">Для свойств customerId, defaultDomainName и displayName поддерживается фильтрация.</span><span class="sxs-lookup"><span data-stu-id="1db55-119">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1db55-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1db55-120">Request headers</span></span>

| <span data-ttu-id="1db55-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1db55-121">Name</span></span>      |<span data-ttu-id="1db55-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1db55-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1db55-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1db55-123">Authorization</span></span>  | <span data-ttu-id="1db55-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1db55-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1db55-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1db55-126">Request body</span></span>

<span data-ttu-id="1db55-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1db55-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1db55-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1db55-128">Response</span></span>

<span data-ttu-id="1db55-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contract](../resources/contract.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1db55-129">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1db55-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1db55-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1db55-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1db55-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts
```

##### <a name="response"></a><span data-ttu-id="1db55-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="1db55-132">Response</span></span>

<span data-ttu-id="1db55-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1db55-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
      "contractType": "contractType-value",
      "customerId": "customerId-value",
      "defaultDomainName": "defaultDomainName-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
