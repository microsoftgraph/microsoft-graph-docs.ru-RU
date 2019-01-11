---
title: Перечисление contract
description: Получение списка объектов contract, сопоставленных с клиентом партнера.
localization_priority: Normal
ms.openlocfilehash: e1d3fa539a29a84a61c5e715edcfa773a7a705b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866131"
---
# <a name="list-contracts"></a><span data-ttu-id="283e6-103">Перечисление contract</span><span class="sxs-lookup"><span data-stu-id="283e6-103">List contracts</span></span>

> <span data-ttu-id="283e6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="283e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="283e6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="283e6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="283e6-106">Получение списка объектов [contract](../resources/contract.md), сопоставленных с клиентом партнера.</span><span class="sxs-lookup"><span data-stu-id="283e6-106">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="283e6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="283e6-107">Permissions</span></span>

<span data-ttu-id="283e6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="283e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="283e6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="283e6-110">Permission type</span></span>      | <span data-ttu-id="283e6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="283e6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="283e6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="283e6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="283e6-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="283e6-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="283e6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="283e6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="283e6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="283e6-115">Not supported.</span></span>    |
|<span data-ttu-id="283e6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="283e6-116">Application</span></span> | <span data-ttu-id="283e6-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="283e6-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="283e6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="283e6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="283e6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="283e6-119">Optional query parameters</span></span>

<span data-ttu-id="283e6-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="283e6-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="283e6-121">Для свойств customerId, defaultDomainName и displayName поддерживается фильтрация.</span><span class="sxs-lookup"><span data-stu-id="283e6-121">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="283e6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="283e6-122">Request headers</span></span>

| <span data-ttu-id="283e6-123">Имя</span><span class="sxs-lookup"><span data-stu-id="283e6-123">Name</span></span>      |<span data-ttu-id="283e6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="283e6-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="283e6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="283e6-125">Authorization</span></span>  | <span data-ttu-id="283e6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="283e6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="283e6-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="283e6-128">Request body</span></span>

<span data-ttu-id="283e6-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="283e6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="283e6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="283e6-130">Response</span></span>

<span data-ttu-id="283e6-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contract](../resources/contract.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="283e6-131">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="283e6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="283e6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="283e6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="283e6-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/beta/contracts
```

##### <a name="response"></a><span data-ttu-id="283e6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="283e6-134">Response</span></span>

<span data-ttu-id="283e6-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="283e6-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract",
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
