---
title: Получение Трустфрамеворкполици
description: Эта операция возвращает существующий контент Трустфрамеворкполици из клиента Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b8a7c2a9d38d5da3ef38d2a724b3fa1b015a4efd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452070"
---
# <a name="get-trustframeworkpolicy"></a><span data-ttu-id="293c2-103">Получение Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="293c2-103">Get trustFrameworkPolicy</span></span>

<span data-ttu-id="293c2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="293c2-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="293c2-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="293c2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="293c2-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="293c2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="293c2-107">Получение содержимого существующего [трустфрамеворкполици](../resources/trustframeworkpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="293c2-107">Retrieve the contents of an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="293c2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="293c2-108">Permissions</span></span>

<span data-ttu-id="293c2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="293c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="293c2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="293c2-111">Permission type</span></span>      | <span data-ttu-id="293c2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="293c2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="293c2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="293c2-113">Delegated (work or school account)</span></span>| <span data-ttu-id="293c2-114">Policy. Read. ALL, Policy. ReadWrite. Трустфрамеворк</span><span class="sxs-lookup"><span data-stu-id="293c2-114">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="293c2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="293c2-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="293c2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="293c2-116">Not supported.</span></span>|
|<span data-ttu-id="293c2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="293c2-117">Application</span></span>|<span data-ttu-id="293c2-118">Policy. Read. ALL, Policy. ReadWrite. Трустфрамеворк</span><span class="sxs-lookup"><span data-stu-id="293c2-118">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="293c2-119">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="293c2-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="293c2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="293c2-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="293c2-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="293c2-121">Optional query parameters</span></span>

<span data-ttu-id="293c2-122">Этот метод поддерживает `$select` `$expand` [параметры запросов OData](/graph/query-parameters) и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="293c2-122">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="293c2-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="293c2-123">Request headers</span></span>

|<span data-ttu-id="293c2-124">Имя</span><span class="sxs-lookup"><span data-stu-id="293c2-124">Name</span></span>|<span data-ttu-id="293c2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="293c2-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="293c2-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="293c2-126">Authorization</span></span>|<span data-ttu-id="293c2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="293c2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="293c2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="293c2-129">Request body</span></span>

<span data-ttu-id="293c2-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="293c2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="293c2-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="293c2-131">Response</span></span>

<span data-ttu-id="293c2-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и XML-представление объекта [трустфрамеворкполици](../resources/trustframeworkpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="293c2-132">If successful, this method returns a `200 OK` response code and an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) in the response body.</span></span>  

><span data-ttu-id="293c2-133">**Note:** тип контента ответа будет иметь `application/xml`значение.</span><span class="sxs-lookup"><span data-stu-id="293c2-133">**Note:** the response content type will be `application/xml`.</span></span>

## <a name="example"></a><span data-ttu-id="293c2-134">Пример</span><span class="sxs-lookup"><span data-stu-id="293c2-134">Example</span></span>

<span data-ttu-id="293c2-135">В приведенном ниже примере возвращается определенный **трустфрамеворкполици**.</span><span class="sxs-lookup"><span data-stu-id="293c2-135">The following example retrieves a specific **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="293c2-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="293c2-136">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_trustFramework"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_Test/$value
```

##### <a name="response"></a><span data-ttu-id="293c2-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="293c2-137">Response</span></span>

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
