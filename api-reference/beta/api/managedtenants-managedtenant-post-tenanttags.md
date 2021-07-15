---
title: Создание tenantTag
description: Создание нового объекта tenantTag.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e04335b011c3572ce352e9a683c8bb6440343f73
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442091"
---
# <a name="create-tenanttag"></a><span data-ttu-id="53b2e-103">Создание tenantTag</span><span class="sxs-lookup"><span data-stu-id="53b2e-103">Create tenantTag</span></span>
<span data-ttu-id="53b2e-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="53b2e-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53b2e-105">Создание нового [объекта tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="53b2e-105">Create a new [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53b2e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53b2e-106">Permissions</span></span>
<span data-ttu-id="53b2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53b2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53b2e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53b2e-109">Permission type</span></span>|<span data-ttu-id="53b2e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53b2e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53b2e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53b2e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53b2e-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="53b2e-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="53b2e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53b2e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53b2e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53b2e-114">Not supported.</span></span>|
|<span data-ttu-id="53b2e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53b2e-115">Application</span></span>|<span data-ttu-id="53b2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53b2e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53b2e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53b2e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantTags
```

## <a name="request-headers"></a><span data-ttu-id="53b2e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53b2e-118">Request headers</span></span>
|<span data-ttu-id="53b2e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="53b2e-119">Name</span></span>|<span data-ttu-id="53b2e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="53b2e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="53b2e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53b2e-121">Authorization</span></span>|<span data-ttu-id="53b2e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53b2e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="53b2e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53b2e-124">Content-Type</span></span>|<span data-ttu-id="53b2e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53b2e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="53b2e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53b2e-127">Request body</span></span>
<span data-ttu-id="53b2e-128">В теле запроса поставляем представление JSON объекта [tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="53b2e-128">In the request body, supply a JSON representation of the [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

<span data-ttu-id="53b2e-129">В следующей таблице показаны свойства, необходимые при создании [tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="53b2e-129">The following table shows the properties that are required when you create the [tenantTag](../resources/managedtenants-tenanttag.md).</span></span>

|<span data-ttu-id="53b2e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="53b2e-130">Property</span></span>|<span data-ttu-id="53b2e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="53b2e-131">Type</span></span>|<span data-ttu-id="53b2e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="53b2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53b2e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="53b2e-133">displayName</span></span>|<span data-ttu-id="53b2e-134">String</span><span class="sxs-lookup"><span data-stu-id="53b2e-134">String</span></span>|<span data-ttu-id="53b2e-135">Имя отображения тега клиента.</span><span class="sxs-lookup"><span data-stu-id="53b2e-135">The display name for the tenant tag.</span></span>|
|<span data-ttu-id="53b2e-136">description</span><span class="sxs-lookup"><span data-stu-id="53b2e-136">description</span></span>|<span data-ttu-id="53b2e-137">String</span><span class="sxs-lookup"><span data-stu-id="53b2e-137">String</span></span>|<span data-ttu-id="53b2e-138">Описание тега клиента.</span><span class="sxs-lookup"><span data-stu-id="53b2e-138">The description for the tenant tag.</span></span>|

## <a name="response"></a><span data-ttu-id="53b2e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="53b2e-139">Response</span></span>

<span data-ttu-id="53b2e-140">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект tenantTag](../resources/managedtenants-tenanttag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="53b2e-140">If successful, this method returns a `201 Created` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53b2e-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="53b2e-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53b2e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="53b2e-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="53b2e-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="53b2e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tenanttag_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags
Content-Type: application/json
Content-length: 382

{
  "displayName": "Support",
  "description": "Tenants that have purchased extended support"
}
```
# <a name="c"></a>[<span data-ttu-id="53b2e-144">C#</span><span class="sxs-lookup"><span data-stu-id="53b2e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tenanttag-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53b2e-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53b2e-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tenanttag-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53b2e-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53b2e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tenanttag-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53b2e-147">Java</span><span class="sxs-lookup"><span data-stu-id="53b2e-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tenanttag-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="53b2e-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="53b2e-148">Response</span></span>
><span data-ttu-id="53b2e-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="53b2e-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantTags/$entity",
  "id": "11103b2b-0e28-456b-901d-45f98890ab1d",
  "displayName": "Support",
  "description": "Tenants that have purchased extended support",
  "tenantIds": [],
  "isDeleted": null,
  "createdDateTime": "2021-07-11T19:31:49.807267Z",
  "createdByUserId": "cad28f13-0158-43c5-9c59-952f2caa62c0",
  "lastActionDateTime": "2021-07-11T19:31:49.8072716Z",
  "lastActionByUserId": "cad28f13-0158-43c5-9c59-952f2caa62c0"
}
```
