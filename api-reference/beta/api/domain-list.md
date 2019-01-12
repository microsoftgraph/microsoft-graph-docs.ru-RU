---
title: Перечисление доменов
description: Получение списка объектов домена.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c2872ccc8e15bafc7f086d72d663a5bf68dfce86
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964972"
---
# <a name="list-domains"></a><span data-ttu-id="cf5f8-103">Перечисление доменов</span><span class="sxs-lookup"><span data-stu-id="cf5f8-103">List domains</span></span>

> <span data-ttu-id="cf5f8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cf5f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf5f8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf5f8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cf5f8-106">Получение списка объектов домена.</span><span class="sxs-lookup"><span data-stu-id="cf5f8-106">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf5f8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf5f8-107">Permissions</span></span>
<span data-ttu-id="cf5f8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf5f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf5f8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf5f8-110">Permission type</span></span>      | <span data-ttu-id="cf5f8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf5f8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf5f8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf5f8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cf5f8-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf5f8-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="cf5f8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf5f8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf5f8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf5f8-115">Not supported.</span></span>    |
|<span data-ttu-id="cf5f8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf5f8-116">Application</span></span> | <span data-ttu-id="cf5f8-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf5f8-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf5f8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf5f8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cf5f8-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cf5f8-119">Optional query parameters</span></span>
<span data-ttu-id="cf5f8-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cf5f8-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf5f8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf5f8-121">Request headers</span></span>
| <span data-ttu-id="cf5f8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cf5f8-122">Name</span></span>      |<span data-ttu-id="cf5f8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cf5f8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cf5f8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf5f8-124">Authorization</span></span>  | <span data-ttu-id="cf5f8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf5f8-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="cf5f8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="cf5f8-127">Accept</span></span>         | <span data-ttu-id="cf5f8-128">application/json;</span><span class="sxs-lookup"><span data-stu-id="cf5f8-128">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf5f8-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cf5f8-129">Request body</span></span>
<span data-ttu-id="cf5f8-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf5f8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf5f8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf5f8-131">Response</span></span>

<span data-ttu-id="cf5f8-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cf5f8-132">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf5f8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cf5f8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf5f8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf5f8-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/beta/domains
```
##### <a name="response"></a><span data-ttu-id="cf5f8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf5f8-135">Response</span></span>
<span data-ttu-id="cf5f8-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf5f8-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
