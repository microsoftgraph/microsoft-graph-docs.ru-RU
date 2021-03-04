---
title: Обновление trustFrameworkPolicy
description: 'Эта операция обновляет существующий объект trustFrameworkPolicy, или если его не существует, она создает его. '
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2305c7dfde39d742ce1694c030f395f59f6fb7bb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443288"
---
# <a name="update-or-create-trustframeworkpolicy"></a><span data-ttu-id="761b8-103">Обновление или создание trustFrameworkPolicy</span><span class="sxs-lookup"><span data-stu-id="761b8-103">Update or create trustFrameworkPolicy</span></span>

<span data-ttu-id="761b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="761b8-104">Namespace: microsoft.graph</span></span>

><span data-ttu-id="761b8-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="761b8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="761b8-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="761b8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="761b8-107">Обнови [существующее довериеFrameworkPolicy](../resources/trustframeworkpolicy.md) или создайте его, если оно не существует.</span><span class="sxs-lookup"><span data-stu-id="761b8-107">Update an existing [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) or create one if it does not exist.</span></span>

## <a name="permissions"></a><span data-ttu-id="761b8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="761b8-108">Permissions</span></span>

<span data-ttu-id="761b8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="761b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="761b8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="761b8-111">Permission type</span></span>      | <span data-ttu-id="761b8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="761b8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="761b8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="761b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="761b8-114">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="761b8-114">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="761b8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="761b8-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="761b8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="761b8-116">Not supported.</span></span>|
|<span data-ttu-id="761b8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="761b8-117">Application</span></span>|<span data-ttu-id="761b8-118">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="761b8-118">Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="761b8-119">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="761b8-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="761b8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="761b8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/policies/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="761b8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="761b8-121">Request headers</span></span>

|<span data-ttu-id="761b8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="761b8-122">Name</span></span>|<span data-ttu-id="761b8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="761b8-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="761b8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="761b8-124">Authorization</span></span>|<span data-ttu-id="761b8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="761b8-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="761b8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="761b8-127">Content-Type</span></span>|<span data-ttu-id="761b8-128">application/xml.</span><span class="sxs-lookup"><span data-stu-id="761b8-128">application/xml.</span></span> <span data-ttu-id="761b8-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="761b8-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="761b8-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="761b8-130">Request body</span></span>

<span data-ttu-id="761b8-131">В теле запроса укажи XML-представление [объекта trustFrameworkPolicy.](../resources/trustframeworkpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="761b8-131">In the request body, provide an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span> 

><span data-ttu-id="761b8-132">**Примечание:** тип контента должен быть `application/xml` .</span><span class="sxs-lookup"><span data-stu-id="761b8-132">**Note:** the content type must be `application/xml`.</span></span>

## <a name="response"></a><span data-ttu-id="761b8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="761b8-133">Response</span></span>

<span data-ttu-id="761b8-134">Ответ будет одним из следующих:</span><span class="sxs-lookup"><span data-stu-id="761b8-134">The response will be one of the following:</span></span>
- <span data-ttu-id="761b8-135">Если существует [trustFrameworkPolicy,](../resources/trustframeworkpolicy.md) успешный запрос возвращает `200 OK` код ответа.</span><span class="sxs-lookup"><span data-stu-id="761b8-135">If a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) exists, a successful request returns a `200 OK` response code.</span></span>
- <span data-ttu-id="761b8-136">Если [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) не существует, успешный запрос возвращает `201 Created` код ответа.</span><span class="sxs-lookup"><span data-stu-id="761b8-136">If a [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) does not exist, a successful request returns a `201 Created` response code.</span></span>
- <span data-ttu-id="761b8-137">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="761b8-137">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="761b8-138">Пример</span><span class="sxs-lookup"><span data-stu-id="761b8-138">Example</span></span>

<span data-ttu-id="761b8-139">В следующем примере **обновляется trustFrameworkPolicy.**</span><span class="sxs-lookup"><span data-stu-id="761b8-139">The following example updates a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="761b8-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="761b8-140">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="761b8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="761b8-141">Response</span></span>

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


