---
title: Получение Трустфрамеворкполици
description: Эта операция возвращает существующий контент Трустфрамеворкполици из клиента Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e4e0a10c0a4c230c172230eecfce177deb4a4d91
ms.sourcegitcommit: d264fa064215879fa88a4680402cd57a470d73db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2019
ms.locfileid: "31989431"
---
# <a name="get-trustframeworkpolicy"></a><span data-ttu-id="fd472-103">Получение Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="fd472-103">Get trustFrameworkPolicy</span></span>

><span data-ttu-id="fd472-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fd472-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd472-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd472-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd472-106">Получение содержимого существующего [трустфрамеворкполици](../resources/trustframeworkpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="fd472-106">Retrieve the contents of an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fd472-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd472-107">Permissions</span></span>

<span data-ttu-id="fd472-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd472-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="fd472-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd472-110">Permission type</span></span>      | <span data-ttu-id="fd472-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd472-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd472-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd472-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd472-113">Policy. Read. Трустфрамеворк, Policy. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="fd472-113">Policy.Read.TrustFramework, Policy.Read.All</span></span>|
|<span data-ttu-id="fd472-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd472-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fd472-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd472-115">Not supported.</span></span>|
|<span data-ttu-id="fd472-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd472-116">Application</span></span>|<span data-ttu-id="fd472-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd472-117">Not supported.</span></span>|

<span data-ttu-id="fd472-118">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="fd472-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="fd472-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd472-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd472-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fd472-120">Optional query parameters</span></span>

<span data-ttu-id="fd472-121">Этот метод поддерживает `$select` `$expand` [параметры запросов OData](/graph/query-parameters) и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="fd472-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd472-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd472-122">Request headers</span></span>

|<span data-ttu-id="fd472-123">Имя</span><span class="sxs-lookup"><span data-stu-id="fd472-123">Name</span></span>|<span data-ttu-id="fd472-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fd472-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="fd472-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd472-125">Authorization</span></span>|<span data-ttu-id="fd472-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd472-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd472-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd472-128">Request body</span></span>

<span data-ttu-id="fd472-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd472-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd472-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd472-130">Response</span></span>

<span data-ttu-id="fd472-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и XML-представление объекта [трустфрамеворкполици](../resources/trustFrameworkpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd472-131">If successful, this method returns a `200 OK` response code and an XML representation of the [trustFrameworkPolicy](../resources/trustFrameworkpolicy.md) in the response body.</span></span>  

><span data-ttu-id="fd472-132">**Note:** тип контента ответа будет иметь `application/xml`значение.</span><span class="sxs-lookup"><span data-stu-id="fd472-132">**Note:** the response content type will be `application/xml`.</span></span>

## <a name="example"></a><span data-ttu-id="fd472-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fd472-133">Example</span></span>

<span data-ttu-id="fd472-134">В приведенном ниже примере возвращается определенный **трустфрамеворкполици**.</span><span class="sxs-lookup"><span data-stu-id="fd472-134">The following example retrieves a specific **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="fd472-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd472-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_trustFramework"
}-->
```http
https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_Test/$value
```

##### <a name="response"></a><span data-ttu-id="fd472-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd472-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFramework.policy"
} -->
```http
HTTP/1.1 200 OK
Content-Type application/xml
<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_Test" PublicPolicyUri="http://tenantName.onmicrosoft.com/B2C_1A_Test">
    .....
    ....
    <!---PolicyContent-->
    ....
    ....
</TrustFrameworkPolicy>
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get trustFramework policy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
