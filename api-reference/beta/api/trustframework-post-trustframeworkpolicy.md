---
title: Создание Трустфрамеворкполици
description: Эта операция создает новый объект Трустфрамеворкполици в клиенте Azure AD B2C.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b3e06b35d838817e3214ea10d22c11fe8d19d59f
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215919"
---
# <a name="create-trustframeworkpolicy"></a><span data-ttu-id="f835b-103">Создание Трустфрамеворкполици</span><span class="sxs-lookup"><span data-stu-id="f835b-103">Create trustFrameworkPolicy</span></span>

<span data-ttu-id="f835b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f835b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f835b-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f835b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f835b-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f835b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f835b-107">Создание нового объекта [трустфрамеворкполици](../resources/trustframeworkpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f835b-107">Create new [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f835b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f835b-108">Permissions</span></span>

<span data-ttu-id="f835b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f835b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="f835b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f835b-111">Permission type</span></span>      | <span data-ttu-id="f835b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f835b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f835b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f835b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f835b-114">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="f835b-114">Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="f835b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f835b-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f835b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f835b-116">Not supported.</span></span>|
|<span data-ttu-id="f835b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f835b-117">Application</span></span>|<span data-ttu-id="f835b-118">Policy.ReadWrite.TrustFramework</span><span class="sxs-lookup"><span data-stu-id="f835b-118">Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="f835b-119">Рабочая или учебная учетная запись должна быть глобальным администратором клиента.</span><span class="sxs-lookup"><span data-stu-id="f835b-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="f835b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f835b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /trustFramework/policies
```

## <a name="request-headers"></a><span data-ttu-id="f835b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f835b-121">Request headers</span></span>

|<span data-ttu-id="f835b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f835b-122">Name</span></span>|<span data-ttu-id="f835b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f835b-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="f835b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f835b-124">Authorization</span></span>|<span data-ttu-id="f835b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f835b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f835b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f835b-127">Content-Type</span></span>|<span data-ttu-id="f835b-128">Application/XML.</span><span class="sxs-lookup"><span data-stu-id="f835b-128">application/xml.</span></span> <span data-ttu-id="f835b-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f835b-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f835b-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f835b-130">Request body</span></span>

<span data-ttu-id="f835b-131">В тексте запроса предоставьте XML-представление объекта [трустфрамеворкполици](../resources/trustframeworkpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f835b-131">In the request body, provide an XML representation of the [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object.</span></span> <span data-ttu-id="f835b-132">Необходимый тип контента — `application/xml`.</span><span class="sxs-lookup"><span data-stu-id="f835b-132">The content type must be `application/xml`.</span></span>

## <a name="response"></a><span data-ttu-id="f835b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f835b-133">Response</span></span>

<span data-ttu-id="f835b-134">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [трустфрамеворкполици](../resources/trustframeworkpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f835b-134">If successful, this method returns a `201 Created` response code and [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) object in the response body.</span></span> <span data-ttu-id="f835b-135">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="f835b-135">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="example"></a><span data-ttu-id="f835b-136">Пример</span><span class="sxs-lookup"><span data-stu-id="f835b-136">Example</span></span>

<span data-ttu-id="f835b-137">В следующем примере создается объект **трустфрамеворкполици**.</span><span class="sxs-lookup"><span data-stu-id="f835b-137">The following example creates a **trustFrameworkPolicy**.</span></span>

##### <a name="request"></a><span data-ttu-id="f835b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="f835b-138">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="f835b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f835b-139">Response</span></span>

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
