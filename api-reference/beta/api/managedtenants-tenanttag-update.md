---
title: Обновление tenantTag
description: Обновление свойств объекта tenantTag.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e5e947437a8b91edd88c5ea81e9c1f8575aadf5d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402586"
---
# <a name="update-tenanttag"></a><span data-ttu-id="97a25-103">Обновление tenantTag</span><span class="sxs-lookup"><span data-stu-id="97a25-103">Update tenantTag</span></span>
<span data-ttu-id="97a25-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="97a25-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97a25-105">Обновление свойств объекта [tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="97a25-105">Update the properties of a [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="97a25-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97a25-106">Permissions</span></span>
<span data-ttu-id="97a25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97a25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97a25-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97a25-109">Permission type</span></span>|<span data-ttu-id="97a25-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97a25-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97a25-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97a25-111">Delegated (work or school account)</span></span>|<span data-ttu-id="97a25-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="97a25-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="97a25-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97a25-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97a25-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97a25-114">Not supported.</span></span>|
|<span data-ttu-id="97a25-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97a25-115">Application</span></span>|<span data-ttu-id="97a25-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97a25-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97a25-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97a25-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```

## <a name="request-headers"></a><span data-ttu-id="97a25-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97a25-118">Request headers</span></span>
|<span data-ttu-id="97a25-119">Имя</span><span class="sxs-lookup"><span data-stu-id="97a25-119">Name</span></span>|<span data-ttu-id="97a25-120">Описание</span><span class="sxs-lookup"><span data-stu-id="97a25-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="97a25-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97a25-121">Authorization</span></span>|<span data-ttu-id="97a25-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97a25-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="97a25-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97a25-124">Content-Type</span></span>|<span data-ttu-id="97a25-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97a25-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97a25-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97a25-127">Request body</span></span>
<span data-ttu-id="97a25-128">В теле запроса укажи значения для соответствующих [полей tenantTag,](../resources/managedtenants-tenanttag.md) которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="97a25-128">In the request body, supply the values for relevant [tenantTag](../resources/managedtenants-tenanttag.md) fields that should be updated.</span></span> <span data-ttu-id="97a25-129">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="97a25-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="97a25-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="97a25-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="97a25-131">Следующие свойства можно обновить:</span><span class="sxs-lookup"><span data-stu-id="97a25-131">Following properties can be updated:</span></span>

| <span data-ttu-id="97a25-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="97a25-132">Property</span></span>     | <span data-ttu-id="97a25-133">Тип</span><span class="sxs-lookup"><span data-stu-id="97a25-133">Type</span></span>        | <span data-ttu-id="97a25-134">Описание</span><span class="sxs-lookup"><span data-stu-id="97a25-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="97a25-135">displayName</span><span class="sxs-lookup"><span data-stu-id="97a25-135">displayName</span></span>|<span data-ttu-id="97a25-136">String</span><span class="sxs-lookup"><span data-stu-id="97a25-136">String</span></span>|<span data-ttu-id="97a25-137">Имя отображения тега клиента.</span><span class="sxs-lookup"><span data-stu-id="97a25-137">The display name for the tenant tag.</span></span>|
|<span data-ttu-id="97a25-138">description</span><span class="sxs-lookup"><span data-stu-id="97a25-138">description</span></span>|<span data-ttu-id="97a25-139">String</span><span class="sxs-lookup"><span data-stu-id="97a25-139">String</span></span>|<span data-ttu-id="97a25-140">Описание тега клиента.</span><span class="sxs-lookup"><span data-stu-id="97a25-140">The description for the tenant tag.</span></span>|
|<span data-ttu-id="97a25-141">клиенты</span><span class="sxs-lookup"><span data-stu-id="97a25-141">tenants</span></span>|<span data-ttu-id="97a25-142">[коллекция microsoft.graph.managedTenants.tenantInfo](../resources/managedtenants-tenantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="97a25-142">[microsoft.graph.managedTenants.tenantInfo](../resources/managedtenants-tenantinfo.md) collection</span></span>|<span data-ttu-id="97a25-143">Коллекция управляемых клиентов, связанных с тегом клиента.</span><span class="sxs-lookup"><span data-stu-id="97a25-143">The collection of managed tenants associated with the tenant tag.</span></span>|

## <a name="response"></a><span data-ttu-id="97a25-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="97a25-144">Response</span></span>

<span data-ttu-id="97a25-145">В случае успешной работы этот метод возвращает код отклика и `200 OK` обновленный [объект tenantTag](../resources/managedtenants-tenanttag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="97a25-145">If successful, this method returns a `200 OK` response code and an updated [tenantTag](../resources/managedtenants-tenanttag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="97a25-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="97a25-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="97a25-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="97a25-147">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="97a25-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="97a25-148">Response</span></span>
><span data-ttu-id="97a25-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="97a25-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
