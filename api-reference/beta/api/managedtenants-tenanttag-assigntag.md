---
title: 'tenantTag: assignTag'
description: Назначьте тег клиента указанным управляемым арендаторам.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 8f9d641cb0d3129802431948601d656f9036e2ef
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403097"
---
# <a name="tenanttag-assigntag"></a><span data-ttu-id="60e3f-103">tenantTag: assignTag</span><span class="sxs-lookup"><span data-stu-id="60e3f-103">tenantTag: assignTag</span></span>
<span data-ttu-id="60e3f-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="60e3f-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60e3f-105">Назначьте тег клиента указанным управляемым арендаторам.</span><span class="sxs-lookup"><span data-stu-id="60e3f-105">Assign the tenant tag to the specified managed tenants.</span></span>

## <a name="permissions"></a><span data-ttu-id="60e3f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60e3f-106">Permissions</span></span>
<span data-ttu-id="60e3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60e3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60e3f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60e3f-109">Permission type</span></span>|<span data-ttu-id="60e3f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60e3f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60e3f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60e3f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="60e3f-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="60e3f-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="60e3f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60e3f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60e3f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60e3f-114">Not supported.</span></span>|
|<span data-ttu-id="60e3f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60e3f-115">Application</span></span>|<span data-ttu-id="60e3f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60e3f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60e3f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60e3f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantTags/{tenantTagId}/assignTag
```

## <a name="request-headers"></a><span data-ttu-id="60e3f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60e3f-118">Request headers</span></span>
|<span data-ttu-id="60e3f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="60e3f-119">Name</span></span>|<span data-ttu-id="60e3f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="60e3f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="60e3f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60e3f-121">Authorization</span></span>|<span data-ttu-id="60e3f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60e3f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="60e3f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="60e3f-124">Content-Type</span></span>|<span data-ttu-id="60e3f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60e3f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60e3f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60e3f-127">Request body</span></span>
<span data-ttu-id="60e3f-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60e3f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="60e3f-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="60e3f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="60e3f-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="60e3f-130">Parameter</span></span>|<span data-ttu-id="60e3f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="60e3f-131">Type</span></span>|<span data-ttu-id="60e3f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="60e3f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60e3f-133">tenantIds</span><span class="sxs-lookup"><span data-stu-id="60e3f-133">tenantIds</span></span>|<span data-ttu-id="60e3f-134">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="60e3f-134">String collection</span></span>|<span data-ttu-id="60e3f-135">Коллекция идентификаторов Azure Active Directory, на которые должен быть назначен тег клиента.</span><span class="sxs-lookup"><span data-stu-id="60e3f-135">The collection of Azure Active Directory tenant identifiers where the tenant tag should be assigned.</span></span>|

## <a name="response"></a><span data-ttu-id="60e3f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="60e3f-136">Response</span></span>

<span data-ttu-id="60e3f-137">В случае успеха это действие возвращает код отклика и `200 OK` [tenantTag](../resources/managedtenants-tenanttag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="60e3f-137">If successful, this action returns a `200 OK` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60e3f-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="60e3f-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60e3f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="60e3f-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "tenanttag_assigntag"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}/assignTag
Content-Type: application/json
Content-length: 41

{
  "tenantIds": [
    "String"
  ]
}
```

### <a name="response"></a><span data-ttu-id="60e3f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="60e3f-140">Response</span></span>
><span data-ttu-id="60e3f-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="60e3f-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "displayName": "Support",
  "description": "Tenants that have purchased support",
  "tenants": [
    {
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b"
    }
  ],
  "isDeleted": null,
  "createdDateTime": "2021-06-26T13:51:23.3927236Z",
  "createdByUserId": "65ca7649-4ccb-4823-9c39-42bd75191bf8",
  "lastActionDateTime": "2021-07-11T19:55:19.7230386Z",
  "lastActionByUserId": "50bf7bd8-1b3a-4d1d-94c5-86d27e68857f"
}
```
