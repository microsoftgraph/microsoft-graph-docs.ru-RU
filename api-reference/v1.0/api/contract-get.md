---
title: Получение Contract
description: Получение свойств и связей объекта contract.
ms.openlocfilehash: 2542fd551277e0a8d9ef76cfe82c2f8c80ec3d7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027261"
---
# <a name="get-contract"></a><span data-ttu-id="9d3a4-103">Получение Contract</span><span class="sxs-lookup"><span data-stu-id="9d3a4-103">Get Contract</span></span>

<span data-ttu-id="9d3a4-104">Получение свойств и связей объекта [contract](../resources/contract.md).</span><span class="sxs-lookup"><span data-stu-id="9d3a4-104">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d3a4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d3a4-105">Permissions</span></span>

<span data-ttu-id="9d3a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d3a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9d3a4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d3a4-108">Permission type</span></span>      | <span data-ttu-id="9d3a4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d3a4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d3a4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d3a4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9d3a4-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d3a4-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9d3a4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d3a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d3a4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d3a4-113">Not supported.</span></span>    |
|<span data-ttu-id="9d3a4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d3a4-114">Application</span></span> | <span data-ttu-id="9d3a4-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d3a4-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d3a4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d3a4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d3a4-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9d3a4-117">Optional query parameters</span></span>

<span data-ttu-id="9d3a4-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9d3a4-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d3a4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d3a4-119">Request headers</span></span>

| <span data-ttu-id="9d3a4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9d3a4-120">Name</span></span>      |<span data-ttu-id="9d3a4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9d3a4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9d3a4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d3a4-122">Authorization</span></span>  | <span data-ttu-id="9d3a4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d3a4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d3a4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d3a4-125">Request body</span></span>

<span data-ttu-id="9d3a4-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d3a4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d3a4-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d3a4-127">Response</span></span>

<span data-ttu-id="9d3a4-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [Contract](../resources/contract.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9d3a4-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d3a4-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9d3a4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d3a4-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d3a4-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="9d3a4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d3a4-131">Response</span></span>
<span data-ttu-id="9d3a4-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9d3a4-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 186

{
  "contractType": "contractType-value",
  "customerId": "customerId-value",
  "defaultDomainName": "defaultDomainName-value",
  "displayName": "displayName-value",
  "id": "id-value"
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