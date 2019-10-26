---
title: Создание Трустфрамеворкполици
description: Эта операция создает новый объект Трустфрамеворкполици в клиенте Azure AD B2C.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 39dd9cbc14ae0dc6040618619595dd4cceb0dadc
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734467"
---
# <a name="create-trustframeworkpolicy"></a><span data-ttu-id="66e0c-103">Создание Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="66e0c-103">Create trustFrameworkPolicy</span></span>

> <span data-ttu-id="66e0c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="66e0c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66e0c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66e0c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66e0c-106">Создание нового объекта [трустфрамеворкполици](../resources/trustframeworkpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="66e0c-106">Create new [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="66e0c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66e0c-107">Permissions</span></span>

<span data-ttu-id="66e0c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="66e0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="66e0c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66e0c-110">Permission type</span></span>      | <span data-ttu-id="66e0c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66e0c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66e0c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66e0c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66e0c-113">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="66e0c-113">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="66e0c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66e0c-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="66e0c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66e0c-115">Not supported.</span></span>|
|<span data-ttu-id="66e0c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66e0c-116">Application</span></span>|<span data-ttu-id="66e0c-117">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="66e0c-117">Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="66e0c-118">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="66e0c-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="66e0c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66e0c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /trustFramework/policies
```

## <a name="request-headers"></a><span data-ttu-id="66e0c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66e0c-120">Request headers</span></span>

|<span data-ttu-id="66e0c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="66e0c-121">Name</span></span>|<span data-ttu-id="66e0c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="66e0c-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="66e0c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66e0c-123">Authorization</span></span>|<span data-ttu-id="66e0c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66e0c-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="66e0c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66e0c-126">Content-Type</span></span>|<span data-ttu-id="66e0c-127">Application/XML.</span><span class="sxs-lookup"><span data-stu-id="66e0c-127">application/xml.</span></span> <span data-ttu-id="66e0c-128">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="66e0c-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="66e0c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66e0c-129">Request body</span></span>

<span data-ttu-id="66e0c-130">В тексте запроса предоставьте XML-представление объекта [трустфрамеворкполици](../resources/trustframeworkpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="66e0c-130">In the request body, provide an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span> <span data-ttu-id="66e0c-131">Необходимый тип контента — `application/xml`.</span><span class="sxs-lookup"><span data-stu-id="66e0c-131">The content type must be `application/xml`.</span></span>

## <a name="response"></a><span data-ttu-id="66e0c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="66e0c-132">Response</span></span>

<span data-ttu-id="66e0c-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [трустфрамеворкполици](../resources/trustframeworkpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66e0c-133">If successful, this method returns a `201 Created` response code and [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object in the response body.</span></span> <span data-ttu-id="66e0c-134">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="66e0c-134">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="66e0c-135">Пример</span><span class="sxs-lookup"><span data-stu-id="66e0c-135">Example</span></span>

<span data-ttu-id="66e0c-136">В следующем примере создается объект **трустфрамеворкполици**.</span><span class="sxs-lookup"><span data-stu-id="66e0c-136">The following example creates a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="66e0c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="66e0c-137">Request</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "name": "create_trustframeworkpolicy_from_trustframeworkpolicy"
}-->
```http
POST https://graph.microsoft.com/beta/trustFramework/policies
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```

##### <a name="response"></a><span data-ttu-id="66e0c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="66e0c-138">Response</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/xml
Location: /trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base/

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base" PublicPolicyUri="http://tenantName.onmicrosoft.com/B2C_1A_Test">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
