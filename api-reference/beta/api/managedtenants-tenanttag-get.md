---
title: Get tenantTag
description: Ознакомьтесь с свойствами и отношениями объекта tenantTag.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 5094df9488292e521cbddfedd380a0846385f147
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403120"
---
# <a name="get-tenanttag"></a><span data-ttu-id="3b1d9-103">Get tenantTag</span><span class="sxs-lookup"><span data-stu-id="3b1d9-103">Get tenantTag</span></span>
<span data-ttu-id="3b1d9-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="3b1d9-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b1d9-105">Ознакомьтесь с свойствами и отношениями объекта [tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="3b1d9-105">Read the properties and relationships of a [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b1d9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b1d9-106">Permissions</span></span>
<span data-ttu-id="3b1d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b1d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b1d9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b1d9-109">Permission type</span></span>|<span data-ttu-id="3b1d9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b1d9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b1d9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b1d9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3b1d9-112">ManagedTenants.Read.All, ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="3b1d9-112">ManagedTenants.Read.All, ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="3b1d9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b1d9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b1d9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b1d9-114">Not supported.</span></span>|
|<span data-ttu-id="3b1d9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b1d9-115">Application</span></span>|<span data-ttu-id="3b1d9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b1d9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b1d9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b1d9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b1d9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3b1d9-118">Optional query parameters</span></span>
<span data-ttu-id="3b1d9-119">Этот метод поддерживает [параметры запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$count` , , , , , и `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="3b1d9-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b1d9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b1d9-120">Request headers</span></span>
|<span data-ttu-id="3b1d9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3b1d9-121">Name</span></span>|<span data-ttu-id="3b1d9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3b1d9-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3b1d9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b1d9-123">Authorization</span></span>|<span data-ttu-id="3b1d9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b1d9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b1d9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b1d9-126">Request body</span></span>
<span data-ttu-id="3b1d9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3b1d9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b1d9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b1d9-128">Response</span></span>

<span data-ttu-id="3b1d9-129">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект tenantTag](../resources/managedtenants-tenanttag.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3b1d9-129">If successful, this method returns a `200 OK` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3b1d9-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="3b1d9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3b1d9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b1d9-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tenanttag"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```


### <a name="response"></a><span data-ttu-id="3b1d9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b1d9-132">Response</span></span>
><span data-ttu-id="3b1d9-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3b1d9-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/tenantTags/$entity",
    "id": "913391c0-5466-42b4-900d-0a7501399cb0",
    "displayName": "Onboarding",
    "description": "Tenants that we are currently onboarding",
    "tenantIds": [
        "38227791-a88b-4fcc-81c5-58cf77668320",
        "34298981-4fc8-4974-9486-c8909ed1521b",
        "4d262a25-c70a-430b-9e8e-46c31dec116b"
    ],
    "isDeleted": null,
    "createdDateTime": "2021-06-16T20:36:31.086644Z",
    "createdByUserId": "9bf6a5ad-aecb-4194-a16b-38e02702a602",
    "lastActionDateTime": "2021-06-28T20:46:09.0071888Z",
    "lastActionByUserId": "08ea0285-30cb-46cc-abc8-3d8422e21ecb",
    "tenants": [
        {
            "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
        },
        {
            "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b"
        },
        {
            "tenantId": "4d262a25-c70a-430b-9e8e-46c31dec116b"
        }
    ]
}
```
