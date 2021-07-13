---
title: Создание tenantTag
description: Создание нового объекта tenantTag.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 9de058914e2262debcbe87d449b5ffc7fc15db7b
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403056"
---
# <a name="create-tenanttag"></a><span data-ttu-id="8aea7-103">Создание tenantTag</span><span class="sxs-lookup"><span data-stu-id="8aea7-103">Create tenantTag</span></span>
<span data-ttu-id="8aea7-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="8aea7-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aea7-105">Создание нового [объекта tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="8aea7-105">Create a new [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8aea7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8aea7-106">Permissions</span></span>
<span data-ttu-id="8aea7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8aea7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8aea7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8aea7-109">Permission type</span></span>|<span data-ttu-id="8aea7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8aea7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8aea7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8aea7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8aea7-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="8aea7-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="8aea7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8aea7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8aea7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8aea7-114">Not supported.</span></span>|
|<span data-ttu-id="8aea7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8aea7-115">Application</span></span>|<span data-ttu-id="8aea7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8aea7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8aea7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8aea7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantTags
```

## <a name="request-headers"></a><span data-ttu-id="8aea7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8aea7-118">Request headers</span></span>
|<span data-ttu-id="8aea7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8aea7-119">Name</span></span>|<span data-ttu-id="8aea7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8aea7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8aea7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8aea7-121">Authorization</span></span>|<span data-ttu-id="8aea7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8aea7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8aea7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8aea7-124">Content-Type</span></span>|<span data-ttu-id="8aea7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8aea7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8aea7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8aea7-127">Request body</span></span>
<span data-ttu-id="8aea7-128">В теле запроса поставляем представление JSON объекта [tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="8aea7-128">In the request body, supply a JSON representation of the [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

<span data-ttu-id="8aea7-129">В следующей таблице показаны свойства, необходимые при создании [tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="8aea7-129">The following table shows the properties that are required when you create the [tenantTag](../resources/managedtenants-tenanttag.md).</span></span>

|<span data-ttu-id="8aea7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8aea7-130">Property</span></span>|<span data-ttu-id="8aea7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8aea7-131">Type</span></span>|<span data-ttu-id="8aea7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8aea7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8aea7-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8aea7-133">displayName</span></span>|<span data-ttu-id="8aea7-134">String</span><span class="sxs-lookup"><span data-stu-id="8aea7-134">String</span></span>|<span data-ttu-id="8aea7-135">Имя отображения тега клиента.</span><span class="sxs-lookup"><span data-stu-id="8aea7-135">The display name for the tenant tag.</span></span>|
|<span data-ttu-id="8aea7-136">description</span><span class="sxs-lookup"><span data-stu-id="8aea7-136">description</span></span>|<span data-ttu-id="8aea7-137">String</span><span class="sxs-lookup"><span data-stu-id="8aea7-137">String</span></span>|<span data-ttu-id="8aea7-138">Описание тега клиента.</span><span class="sxs-lookup"><span data-stu-id="8aea7-138">The description for the tenant tag.</span></span>|

## <a name="response"></a><span data-ttu-id="8aea7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="8aea7-139">Response</span></span>

<span data-ttu-id="8aea7-140">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект tenantTag](../resources/managedtenants-tenanttag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8aea7-140">If successful, this method returns a `201 Created` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8aea7-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="8aea7-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8aea7-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="8aea7-142">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="8aea7-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8aea7-143">Response</span></span>
><span data-ttu-id="8aea7-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8aea7-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
