---
title: Get mobileAppManagementPolicy
description: Ознакомьтесь с свойствами и отношениями политики управления мобильными приложениями.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 66e20ff34af0cca293cc320b7b6f20852853b39c
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401675"
---
# <a name="get-mobileappmanagementpolicy"></a><span data-ttu-id="70920-103">Get mobileAppManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="70920-103">Get mobileAppManagementPolicy</span></span>

<span data-ttu-id="70920-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70920-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70920-105">Ознакомьтесь с свойствами и отношениями объекта [mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="70920-105">Read the properties and relationships of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="70920-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70920-106">Permissions</span></span>

<span data-ttu-id="70920-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70920-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70920-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70920-109">Permission type</span></span>|<span data-ttu-id="70920-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70920-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70920-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70920-111">Delegated (work or school account)</span></span>|<span data-ttu-id="70920-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="70920-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="70920-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70920-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70920-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70920-114">Not supported.</span></span>|
|<span data-ttu-id="70920-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="70920-115">Application</span></span> | <span data-ttu-id="70920-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70920-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70920-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70920-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileAppManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="70920-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70920-118">Request headers</span></span>

|<span data-ttu-id="70920-119">Имя</span><span class="sxs-lookup"><span data-stu-id="70920-119">Name</span></span>|<span data-ttu-id="70920-120">Описание</span><span class="sxs-lookup"><span data-stu-id="70920-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="70920-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70920-121">Authorization</span></span>|<span data-ttu-id="70920-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70920-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70920-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70920-124">Request body</span></span>

<span data-ttu-id="70920-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70920-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70920-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="70920-126">Response</span></span>

<span data-ttu-id="70920-127">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="70920-127">If successful, this method returns a `200 OK` response code and a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="70920-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="70920-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="70920-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="70920-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mobilitymanagementpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
```

### <a name="response"></a><span data-ttu-id="70920-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="70920-130">Response</span></span>

><span data-ttu-id="70920-131">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="70920-131">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "value": {
    "id": "ab90bacf-55a3-4a3e-839a-aa4b74e4f020",
    "appliesTo": "selected",
    "complianceUrl": "https://portal.mam.contoso.com/?portalAction=Compliance",
    "description": "Contoso mobilty app is a cloud-based  Endpoint Management solution for managing Windows.",
    "discoveryUrl": "https://enrollment.mam.contoso.com/enrollmentserver/discovery.svc",
    "displayName": "Contoso mobilty app",
    "termsOfUseUrl": "https://portal.mam.contoso.com/TermsofUse.aspx",
    "includedGroups": [
      {
        "id": "800c583d-cc3d-4361-8e4a-3fbf668f27f4",
        "displayName": "Test Group"
      }
    ]
  }
}
```
