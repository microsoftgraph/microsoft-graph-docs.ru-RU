---
title: Обновление Трустфрамеворкполици
description: 'Эта операция обновляет существующий объект Трустфрамеворкполици или, если таковой не существует, создает его. '
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f5aa7f489faecb053ddad2734c1318c3cba7ed71
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977449"
---
# <a name="update-or-create-trustframeworkpolicy"></a><span data-ttu-id="3160b-103">Обновление или создание Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="3160b-103">Update or create trustFrameworkPolicy</span></span>

><span data-ttu-id="3160b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3160b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3160b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3160b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3160b-106">Обновите существующий [трустфрамеворкполици](../resources/trustframeworkpolicy.md) или создайте его, если он не существует.</span><span class="sxs-lookup"><span data-stu-id="3160b-106">Update an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) or create one if it does not exist.</span></span>

## <a name="permissions"></a><span data-ttu-id="3160b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3160b-107">Permissions</span></span>

<span data-ttu-id="3160b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3160b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="3160b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3160b-110">Permission type</span></span>      | <span data-ttu-id="3160b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3160b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3160b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3160b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3160b-113">Policy. ReadWrite. Трустфрамеворк, Policy. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3160b-113">Policy.ReadWrite.TrustFramework, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="3160b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3160b-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3160b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3160b-115">Not supported.</span></span>|
|<span data-ttu-id="3160b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3160b-116">Application</span></span>|<span data-ttu-id="3160b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3160b-117">Not supported.</span></span>|

<span data-ttu-id="3160b-118">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="3160b-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="3160b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3160b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/policies/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="3160b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3160b-120">Request headers</span></span>

|<span data-ttu-id="3160b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3160b-121">Name</span></span>|<span data-ttu-id="3160b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3160b-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3160b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3160b-123">Authorization</span></span>|<span data-ttu-id="3160b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3160b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3160b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3160b-126">Content-Type</span></span>|<span data-ttu-id="3160b-127">Application/XML.</span><span class="sxs-lookup"><span data-stu-id="3160b-127">application/xml.</span></span> <span data-ttu-id="3160b-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3160b-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3160b-129">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="3160b-129">Request body</span></span>

<span data-ttu-id="3160b-130">В тексте запроса предоставьте XML-представление объекта [трустфрамеворкполици](../resources/trustframeworkpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="3160b-130">In the request body, provide an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span> 

><span data-ttu-id="3160b-131">**Note:** тип контента должен быть `application/xml`.</span><span class="sxs-lookup"><span data-stu-id="3160b-131">**Note:** the content type must be `application/xml`.</span></span>

## <a name="response"></a><span data-ttu-id="3160b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3160b-132">Response</span></span>

<span data-ttu-id="3160b-133">Ответ будет одним из следующих вариантов:</span><span class="sxs-lookup"><span data-stu-id="3160b-133">The response will be one of the following:</span></span>
- <span data-ttu-id="3160b-134">Если [трустфрамеворкполици](../resources/trustframeworkpolicy.md) существует, успешный запрос возвращает код `200 OK` отклика.</span><span class="sxs-lookup"><span data-stu-id="3160b-134">If a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) exists, a successful request returns a `200 OK` response code.</span></span>
- <span data-ttu-id="3160b-135">Если [трустфрамеворкполици](../resources/trustframeworkpolicy.md) не существует, успешный запрос возвращает код `201 Created` отклика.</span><span class="sxs-lookup"><span data-stu-id="3160b-135">If a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) does not exist, a successful request returns a `201 Created` response code.</span></span>
- <span data-ttu-id="3160b-136">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="3160b-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="3160b-137">Пример</span><span class="sxs-lookup"><span data-stu-id="3160b-137">Example</span></span>

<span data-ttu-id="3160b-138">В следующем примере показано, как обновить объект **трустфрамеворкполици**.</span><span class="sxs-lookup"><span data-stu-id="3160b-138">The following example updates a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="3160b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="3160b-139">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_trustframeworkpolicy"
}-->
```http
PUT https://graph.microsoft.com/beta/trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base/$value
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```

##### <a name="response"></a><span data-ttu-id="3160b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3160b-140">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true
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
  "description": "Update trustframeworkpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
