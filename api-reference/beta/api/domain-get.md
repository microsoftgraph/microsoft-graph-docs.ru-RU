---
title: Получение домена
description: Получение свойств и связей объекта домена.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8086887652412c88372871a5a8d6914372e3f83f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955389"
---
# <a name="get-domain"></a><span data-ttu-id="e6c57-103">Получение домена</span><span class="sxs-lookup"><span data-stu-id="e6c57-103">Get domain</span></span>

> <span data-ttu-id="e6c57-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e6c57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6c57-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6c57-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6c57-106">Получение свойств и связей объекта домена.</span><span class="sxs-lookup"><span data-stu-id="e6c57-106">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6c57-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6c57-107">Permissions</span></span>

<span data-ttu-id="e6c57-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6c57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e6c57-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6c57-110">Permission type</span></span>      | <span data-ttu-id="e6c57-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6c57-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6c57-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6c57-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e6c57-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6c57-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="e6c57-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6c57-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6c57-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6c57-115">Not supported.</span></span>    |
|<span data-ttu-id="e6c57-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6c57-116">Application</span></span> | <span data-ttu-id="e6c57-117">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6c57-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6c57-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6c57-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="e6c57-119">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="e6c57-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="e6c57-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e6c57-120">Optional query parameters</span></span>

<span data-ttu-id="e6c57-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e6c57-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6c57-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6c57-122">Request headers</span></span>

| <span data-ttu-id="e6c57-123">Имя</span><span class="sxs-lookup"><span data-stu-id="e6c57-123">Name</span></span>      |<span data-ttu-id="e6c57-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e6c57-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e6c57-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6c57-125">Authorization</span></span>  | <span data-ttu-id="e6c57-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6c57-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e6c57-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6c57-128">Content-Type</span></span>  | <span data-ttu-id="e6c57-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e6c57-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6c57-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6c57-130">Request body</span></span>
<span data-ttu-id="e6c57-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6c57-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6c57-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6c57-132">Response</span></span>

<span data-ttu-id="e6c57-133">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e6c57-133">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e6c57-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e6c57-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6c57-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6c57-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="e6c57-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6c57-136">Response</span></span>
<span data-ttu-id="e6c57-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6c57-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
