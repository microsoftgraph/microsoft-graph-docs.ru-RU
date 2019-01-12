---
title: Перечисление contract
description: Получение списка объектов contract, сопоставленных с клиентом партнера.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6df390cbe742443bf8a996362fa2cf2909ef83f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971076"
---
# <a name="list-contracts"></a><span data-ttu-id="70dc0-103">Перечисление contract</span><span class="sxs-lookup"><span data-stu-id="70dc0-103">List contracts</span></span>

> <span data-ttu-id="70dc0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="70dc0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70dc0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70dc0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="70dc0-106">Получение списка объектов [contract](../resources/contract.md), сопоставленных с клиентом партнера.</span><span class="sxs-lookup"><span data-stu-id="70dc0-106">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="70dc0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70dc0-107">Permissions</span></span>

<span data-ttu-id="70dc0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70dc0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="70dc0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70dc0-110">Permission type</span></span>      | <span data-ttu-id="70dc0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70dc0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70dc0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70dc0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="70dc0-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="70dc0-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="70dc0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70dc0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70dc0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70dc0-115">Not supported.</span></span>    |
|<span data-ttu-id="70dc0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70dc0-116">Application</span></span> | <span data-ttu-id="70dc0-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70dc0-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70dc0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70dc0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70dc0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="70dc0-119">Optional query parameters</span></span>

<span data-ttu-id="70dc0-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="70dc0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="70dc0-121">Для свойств customerId, defaultDomainName и displayName поддерживается фильтрация.</span><span class="sxs-lookup"><span data-stu-id="70dc0-121">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70dc0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70dc0-122">Request headers</span></span>

| <span data-ttu-id="70dc0-123">Имя</span><span class="sxs-lookup"><span data-stu-id="70dc0-123">Name</span></span>      |<span data-ttu-id="70dc0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="70dc0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="70dc0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70dc0-125">Authorization</span></span>  | <span data-ttu-id="70dc0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70dc0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70dc0-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="70dc0-128">Request body</span></span>

<span data-ttu-id="70dc0-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70dc0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70dc0-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="70dc0-130">Response</span></span>

<span data-ttu-id="70dc0-131">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [Contract](../resources/contract.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="70dc0-131">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70dc0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="70dc0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70dc0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="70dc0-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/beta/contracts
```

##### <a name="response"></a><span data-ttu-id="70dc0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="70dc0-134">Response</span></span>

<span data-ttu-id="70dc0-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="70dc0-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
