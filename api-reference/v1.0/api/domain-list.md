---
title: Перечисление доменов
description: Получение списка объектов домена.
ms.openlocfilehash: 51c9e4035c44567589ba2f9c7b86453e48db6a9f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025584"
---
# <a name="list-domains"></a><span data-ttu-id="e4bce-103">Перечисление доменов</span><span class="sxs-lookup"><span data-stu-id="e4bce-103">List domains</span></span>

<span data-ttu-id="e4bce-104">Получение списка объектов домена.</span><span class="sxs-lookup"><span data-stu-id="e4bce-104">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4bce-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4bce-105">Permissions</span></span>
<span data-ttu-id="e4bce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4bce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4bce-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4bce-108">Permission type</span></span>      | <span data-ttu-id="e4bce-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4bce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4bce-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4bce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e4bce-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4bce-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="e4bce-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4bce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4bce-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4bce-113">Not supported.</span></span>    |
|<span data-ttu-id="e4bce-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4bce-114">Application</span></span> | <span data-ttu-id="e4bce-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4bce-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4bce-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4bce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e4bce-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e4bce-117">Optional query parameters</span></span>
<span data-ttu-id="e4bce-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e4bce-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4bce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4bce-119">Request headers</span></span>
| <span data-ttu-id="e4bce-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e4bce-120">Name</span></span>      |<span data-ttu-id="e4bce-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e4bce-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e4bce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4bce-122">Authorization</span></span>  | <span data-ttu-id="e4bce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4bce-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e4bce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e4bce-125">Accept</span></span>         | <span data-ttu-id="e4bce-126">application/json;</span><span class="sxs-lookup"><span data-stu-id="e4bce-126">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4bce-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4bce-127">Request body</span></span>
<span data-ttu-id="e4bce-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4bce-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4bce-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4bce-129">Response</span></span>

<span data-ttu-id="e4bce-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e4bce-130">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e4bce-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e4bce-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4bce-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4bce-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains
```
##### <a name="response"></a><span data-ttu-id="e4bce-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4bce-133">Response</span></span>
<span data-ttu-id="e4bce-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4bce-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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