---
title: Get trustFrameworkPolicy
description: Эта операция извлекает существующий контент trustFrameworkPolicy из клиента Azure AD B2C.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bbfa30131d2f17ab046f2ef6c1b997c8fca739b4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444926"
---
# <a name="get-trustframeworkpolicy"></a><span data-ttu-id="69633-103">Get trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="69633-103">Get trustFrameworkPolicy</span></span>

<span data-ttu-id="69633-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69633-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="69633-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="69633-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69633-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69633-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="69633-107">Извлечение содержимого существующего [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="69633-107">Retrieve the contents of an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="69633-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69633-108">Permissions</span></span>

<span data-ttu-id="69633-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="69633-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="69633-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69633-111">Permission type</span></span>      | <span data-ttu-id="69633-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69633-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69633-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69633-113">Delegated (work or school account)</span></span>| <span data-ttu-id="69633-114">Policy.Read.All, Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="69633-114">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="69633-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69633-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="69633-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69633-116">Not supported.</span></span>|
|<span data-ttu-id="69633-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="69633-117">Application</span></span>|<span data-ttu-id="69633-118">Policy.Read.All, Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="69633-118">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="69633-119">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="69633-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="69633-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69633-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69633-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="69633-121">Optional query parameters</span></span>

<span data-ttu-id="69633-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="69633-122">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69633-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69633-123">Request headers</span></span>

|<span data-ttu-id="69633-124">Имя</span><span class="sxs-lookup"><span data-stu-id="69633-124">Name</span></span>|<span data-ttu-id="69633-125">Описание</span><span class="sxs-lookup"><span data-stu-id="69633-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="69633-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69633-126">Authorization</span></span>|<span data-ttu-id="69633-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69633-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="69633-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69633-129">Request body</span></span>

<span data-ttu-id="69633-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69633-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69633-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="69633-131">Response</span></span>

<span data-ttu-id="69633-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` XML-представление [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="69633-132">If successful, this method returns a `200 OK` response code and an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) in the response body.</span></span>  

><span data-ttu-id="69633-133">**Примечание:** тип контента ответа будет `application/xml` .</span><span class="sxs-lookup"><span data-stu-id="69633-133">**Note:** the response content type will be `application/xml`.</span></span>

## <a name="example"></a><span data-ttu-id="69633-134">Пример</span><span class="sxs-lookup"><span data-stu-id="69633-134">Example</span></span>

<span data-ttu-id="69633-135">В следующем примере извлекается определенное **довериеFrameworkPolicy**.</span><span class="sxs-lookup"><span data-stu-id="69633-135">The following example retrieves a specific **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="69633-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="69633-136">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_trustFramework"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_Test/$value
```

##### <a name="response"></a><span data-ttu-id="69633-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="69633-137">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/xml

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


