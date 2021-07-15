---
title: Обновление tenantTag
description: Обновление свойств объекта tenantTag.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 367fd71e769ae2fa4cd73b0f25f120b22fa5f0d9
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442735"
---
# <a name="update-tenanttag"></a><span data-ttu-id="6a6b5-103">Обновление tenantTag</span><span class="sxs-lookup"><span data-stu-id="6a6b5-103">Update tenantTag</span></span>
<span data-ttu-id="6a6b5-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="6a6b5-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a6b5-105">Обновление свойств объекта [tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="6a6b5-105">Update the properties of a [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a6b5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a6b5-106">Permissions</span></span>
<span data-ttu-id="6a6b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a6b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a6b5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a6b5-109">Permission type</span></span>|<span data-ttu-id="6a6b5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a6b5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a6b5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a6b5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6a6b5-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="6a6b5-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="6a6b5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a6b5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a6b5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-114">Not supported.</span></span>|
|<span data-ttu-id="6a6b5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a6b5-115">Application</span></span>|<span data-ttu-id="6a6b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a6b5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a6b5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```

## <a name="request-headers"></a><span data-ttu-id="6a6b5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a6b5-118">Request headers</span></span>
|<span data-ttu-id="6a6b5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6a6b5-119">Name</span></span>|<span data-ttu-id="6a6b5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6a6b5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6a6b5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a6b5-121">Authorization</span></span>|<span data-ttu-id="6a6b5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6a6b5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6a6b5-124">Content-Type</span></span>|<span data-ttu-id="6a6b5-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a6b5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a6b5-127">Request body</span></span>
<span data-ttu-id="6a6b5-128">В теле запроса укажи значения для соответствующих [полей tenantTag,](../resources/managedtenants-tenanttag.md) которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-128">In the request body, supply the values for relevant [tenantTag](../resources/managedtenants-tenanttag.md) fields that should be updated.</span></span> <span data-ttu-id="6a6b5-129">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6a6b5-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="6a6b5-131">Следующие свойства можно обновить:</span><span class="sxs-lookup"><span data-stu-id="6a6b5-131">Following properties can be updated:</span></span>

| <span data-ttu-id="6a6b5-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a6b5-132">Property</span></span>     | <span data-ttu-id="6a6b5-133">Тип</span><span class="sxs-lookup"><span data-stu-id="6a6b5-133">Type</span></span>        | <span data-ttu-id="6a6b5-134">Описание</span><span class="sxs-lookup"><span data-stu-id="6a6b5-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6a6b5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6a6b5-135">displayName</span></span>|<span data-ttu-id="6a6b5-136">String</span><span class="sxs-lookup"><span data-stu-id="6a6b5-136">String</span></span>|<span data-ttu-id="6a6b5-137">Имя отображения тега клиента.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-137">The display name for the tenant tag.</span></span>|
|<span data-ttu-id="6a6b5-138">description</span><span class="sxs-lookup"><span data-stu-id="6a6b5-138">description</span></span>|<span data-ttu-id="6a6b5-139">String</span><span class="sxs-lookup"><span data-stu-id="6a6b5-139">String</span></span>|<span data-ttu-id="6a6b5-140">Описание тега клиента.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-140">The description for the tenant tag.</span></span>|
|<span data-ttu-id="6a6b5-141">клиенты</span><span class="sxs-lookup"><span data-stu-id="6a6b5-141">tenants</span></span>|<span data-ttu-id="6a6b5-142">[коллекция microsoft.graph.managedTenants.tenantInfo](../resources/managedtenants-tenantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="6a6b5-142">[microsoft.graph.managedTenants.tenantInfo](../resources/managedtenants-tenantinfo.md) collection</span></span>|<span data-ttu-id="6a6b5-143">Коллекция управляемых клиентов, связанных с тегом клиента.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-143">The collection of managed tenants associated with the tenant tag.</span></span>|

## <a name="response"></a><span data-ttu-id="6a6b5-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a6b5-144">Response</span></span>

<span data-ttu-id="6a6b5-145">В случае успешной работы этот метод возвращает код отклика и `200 OK` обновленный [объект tenantTag](../resources/managedtenants-tenanttag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-145">If successful, this method returns a `200 OK` response code and an updated [tenantTag](../resources/managedtenants-tenanttag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a6b5-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="6a6b5-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a6b5-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a6b5-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6a6b5-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a6b5-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tenanttag"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}
Content-Type: application/json
Content-length: 382

{
  "displayName": "Onboarding",
  "description": "Tenants that we are currently onboarding"
}
```
# <a name="c"></a>[<span data-ttu-id="6a6b5-149">C#</span><span class="sxs-lookup"><span data-stu-id="6a6b5-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenanttag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a6b5-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a6b5-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenanttag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a6b5-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a6b5-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenanttag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a6b5-152">Java</span><span class="sxs-lookup"><span data-stu-id="6a6b5-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenanttag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6a6b5-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a6b5-153">Response</span></span>
><span data-ttu-id="6a6b5-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6a6b5-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantTags/$entity",
  "id": "913391c0-5466-42b4-900d-0a7501399cb0",
  "displayName": "Onboarding",
  "description": "Tenants that we are currently onboarding",
  "tenantIds": [
    {
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
    }
  ],
  "isDeleted": null,
  "createdDateTime": "2021-06-16T20:36:31.086644Z",
  "createdByUserId": "9bf6a5ad-aecb-4194-a16b-38e02702a602",
  "lastActionDateTime": "2021-07-11T18:54:44.5262828Z",
  "lastActionByUserId": "cad28f13-0158-43c5-9c59-952f2caa62c0"
}
```
