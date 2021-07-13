---
title: Список mobileAppManagementPolicies
description: Получите список объектов политики управления мобильными приложениями и их свойств.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3c50e81c1e7d49f55eafa1eb7b0b5ece32e05a68
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401661"
---
# <a name="list-mobileappmanagementpolicies"></a><span data-ttu-id="a0c9a-103">Список mobileAppManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="a0c9a-103">List mobileAppManagementPolicies</span></span>

<span data-ttu-id="a0c9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0c9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0c9a-105">Получите список объектов [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="a0c9a-105">Get a list of the [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0c9a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0c9a-106">Permissions</span></span>

<span data-ttu-id="a0c9a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0c9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0c9a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0c9a-109">Permission type</span></span>|<span data-ttu-id="a0c9a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0c9a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0c9a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0c9a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a0c9a-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="a0c9a-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="a0c9a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0c9a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0c9a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0c9a-114">Not supported.</span></span>|
|<span data-ttu-id="a0c9a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0c9a-115">Application</span></span> | <span data-ttu-id="a0c9a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0c9a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0c9a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0c9a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileAppManagementPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0c9a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a0c9a-118">Optional query parameters</span></span>

<span data-ttu-id="a0c9a-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a0c9a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a0c9a-120">Пример:</span><span class="sxs-lookup"><span data-stu-id="a0c9a-120">For example:</span></span>

- <span data-ttu-id="a0c9a-121">Чтобы выбрать определенные атрибуты добавить `$select=id,displayname` .</span><span class="sxs-lookup"><span data-stu-id="a0c9a-121">To select specific attributes add `$select=id,displayname`.</span></span>
- <span data-ttu-id="a0c9a-122">Чтобы получить включенные группы для каждой политики, добавьте `$expand=includedGroups` .</span><span class="sxs-lookup"><span data-stu-id="a0c9a-122">To retrieve included groups for each policy, add `$expand=includedGroups`.</span></span>
- <span data-ttu-id="a0c9a-123">Чтобы фильтровать на основе атрибута, используйте `$filter=displayName eq 'Microsoft Intune'` .</span><span class="sxs-lookup"><span data-stu-id="a0c9a-123">To filter based on an attribute, use `$filter=displayName eq 'Microsoft Intune'`.</span></span>

<span data-ttu-id="a0c9a-124">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a0c9a-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0c9a-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0c9a-125">Request headers</span></span>

|<span data-ttu-id="a0c9a-126">Имя</span><span class="sxs-lookup"><span data-stu-id="a0c9a-126">Name</span></span>|<span data-ttu-id="a0c9a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a0c9a-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a0c9a-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0c9a-128">Authorization</span></span>|<span data-ttu-id="a0c9a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0c9a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0c9a-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0c9a-131">Request body</span></span>

<span data-ttu-id="a0c9a-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0c9a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0c9a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0c9a-133">Response</span></span>

<span data-ttu-id="a0c9a-134">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a0c9a-134">If successful, this method returns a `200 OK` response code and a collection of [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0c9a-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="a0c9a-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a0c9a-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0c9a-136">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_mobilitymanagementpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies
```

### <a name="response"></a><span data-ttu-id="a0c9a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0c9a-137">Response</span></span>

><span data-ttu-id="a0c9a-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a0c9a-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobilityManagementPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
   {
    "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
    "id": "ab90bacf-55a3-4a3e-839a-aa4b74e4f020",
    "appliesTo": "selected",
    "complianceUrl": "https://portal.manage.contoso.com/?portalAction=Compliance",
    "description": "Contoso mobilty app is a cloud-based  Endpoint Management solution for managing Windows.",
    "discoveryUrl": "https://enrollment.manage.contoso.com/enrollmentserver/discovery.svc",
    "displayName": "Contoso mobilty app",
    "termsOfUseUrl": "https://portal.manage.contoso.com/TermsofUse.aspx",
    "includedGroups": [
      {
        "id": "800c583d-cc3d-4361-8e4a-3fbf668f27f4",
        "displayName": "Test Group"
      }
    ]
  }
  ]
}
```

<!-- uuid: 5c98f801-d1c4-44eb-ac11-f72b6754deda
2020-03-23T22:34:45.203Z -->
<!-- {
  "type": "#page.annotation",
  "description": "List mobileAppManagementPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
