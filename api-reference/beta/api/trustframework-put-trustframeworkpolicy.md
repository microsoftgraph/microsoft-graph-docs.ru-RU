---
title: Обновление Трустфрамеворкполици
description: 'Эта операция обновляет существующий объект Трустфрамеворкполици или, если таковой не существует, создает его. '
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1cb40c5a70056990bfa7d00443289bbcd565707d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335089"
---
# <a name="update-or-create-trustframeworkpolicy"></a><span data-ttu-id="d48f9-103">Обновление или создание Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="d48f9-103">Update or create trustFrameworkPolicy</span></span>

><span data-ttu-id="d48f9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d48f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d48f9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d48f9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d48f9-106">Обновите существующий [трустфрамеворкполици](../resources/trustframeworkpolicy.md) или создайте его, если он не существует.</span><span class="sxs-lookup"><span data-stu-id="d48f9-106">Update an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) or create one if it does not exist.</span></span>

## <a name="permissions"></a><span data-ttu-id="d48f9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d48f9-107">Permissions</span></span>

<span data-ttu-id="d48f9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d48f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="d48f9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d48f9-110">Permission type</span></span>      | <span data-ttu-id="d48f9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d48f9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d48f9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d48f9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d48f9-113">Policy. ReadWrite. Трустфрамеворк, Policy. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d48f9-113">Policy.ReadWrite.TrustFramework, Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="d48f9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d48f9-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d48f9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d48f9-115">Not supported.</span></span>|
|<span data-ttu-id="d48f9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d48f9-116">Application</span></span>|<span data-ttu-id="d48f9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d48f9-117">Not supported.</span></span>|

<span data-ttu-id="d48f9-118">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="d48f9-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="d48f9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d48f9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/policies/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="d48f9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d48f9-120">Request headers</span></span>

|<span data-ttu-id="d48f9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d48f9-121">Name</span></span>|<span data-ttu-id="d48f9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d48f9-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d48f9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d48f9-123">Authorization</span></span>|<span data-ttu-id="d48f9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d48f9-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d48f9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d48f9-126">Content-Type</span></span>|<span data-ttu-id="d48f9-127">Application/XML.</span><span class="sxs-lookup"><span data-stu-id="d48f9-127">application/xml.</span></span> <span data-ttu-id="d48f9-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d48f9-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d48f9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d48f9-129">Request body</span></span>

<span data-ttu-id="d48f9-130">В тексте запроса предоставьте XML-представление объекта [трустфрамеворкполици](../resources/trustframeworkpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="d48f9-130">In the request body, provide an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span> 

><span data-ttu-id="d48f9-131">**Note:** тип контента должен быть `application/xml`.</span><span class="sxs-lookup"><span data-stu-id="d48f9-131">**Note:** the content type must be `application/xml`.</span></span>

## <a name="response"></a><span data-ttu-id="d48f9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d48f9-132">Response</span></span>

<span data-ttu-id="d48f9-133">Ответ будет одним из следующих вариантов:</span><span class="sxs-lookup"><span data-stu-id="d48f9-133">The response will be one of the following:</span></span>
- <span data-ttu-id="d48f9-134">Если [трустфрамеворкполици](../resources/trustframeworkpolicy.md) существует, успешный запрос возвращает код `200 OK` отклика.</span><span class="sxs-lookup"><span data-stu-id="d48f9-134">If a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) exists, a successful request returns a `200 OK` response code.</span></span>
- <span data-ttu-id="d48f9-135">Если [трустфрамеворкполици](../resources/trustframeworkpolicy.md) не существует, успешный запрос возвращает код `201 Created` отклика.</span><span class="sxs-lookup"><span data-stu-id="d48f9-135">If a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) does not exist, a successful request returns a `201 Created` response code.</span></span>
- <span data-ttu-id="d48f9-136">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="d48f9-136">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="d48f9-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d48f9-137">Example</span></span>

<span data-ttu-id="d48f9-138">В следующем примере показано, как обновить объект **трустфрамеворкполици**.</span><span class="sxs-lookup"><span data-stu-id="d48f9-138">The following example updates a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="d48f9-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d48f9-139">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="d48f9-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d48f9-140">Response</span></span>

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
