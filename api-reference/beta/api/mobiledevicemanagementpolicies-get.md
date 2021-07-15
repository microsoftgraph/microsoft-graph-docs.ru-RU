---
title: Get mobileDeviceManagementPolicy
description: Ознакомьтесь с свойствами и отношениями объекта политики управления мобильными устройствами.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 31d9c474805b208474f3bcd8328d4cf86914f275
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440292"
---
# <a name="get-mobiledevicemanagementpolicy"></a><span data-ttu-id="c0be4-103">Get mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="c0be4-103">Get mobileDeviceManagementPolicy</span></span>

<span data-ttu-id="c0be4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0be4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0be4-105">Ознакомьтесь с свойствами и отношениями объекта [mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="c0be4-105">Read the properties and relationships of a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0be4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0be4-106">Permissions</span></span>

<span data-ttu-id="c0be4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0be4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0be4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0be4-109">Permission type</span></span>|<span data-ttu-id="c0be4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0be4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0be4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0be4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c0be4-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="c0be4-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="c0be4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0be4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0be4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0be4-114">Not supported.</span></span>|
|<span data-ttu-id="c0be4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0be4-115">Application</span></span> | <span data-ttu-id="c0be4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0be4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0be4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0be4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileDeviceManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c0be4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0be4-118">Request headers</span></span>

|<span data-ttu-id="c0be4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c0be4-119">Name</span></span>|<span data-ttu-id="c0be4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c0be4-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c0be4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0be4-121">Authorization</span></span>|<span data-ttu-id="c0be4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0be4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0be4-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0be4-124">Request body</span></span>

<span data-ttu-id="c0be4-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0be4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0be4-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0be4-126">Response</span></span>

<span data-ttu-id="c0be4-127">В случае успешного выполнения этот метод возвращает код ответа и объект `200 OK` [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c0be4-127">If successful, this method returns a `200 OK` response code and a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0be4-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="c0be4-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c0be4-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0be4-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c0be4-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0be4-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mobilitymanagementpolicy"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
```
# <a name="c"></a>[<span data-ttu-id="c0be4-131">C#</span><span class="sxs-lookup"><span data-stu-id="c0be4-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mobilitymanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0be4-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0be4-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mobilitymanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0be4-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0be4-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mobilitymanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0be4-134">Java</span><span class="sxs-lookup"><span data-stu-id="c0be4-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mobilitymanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0be4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0be4-135">Response</span></span>

><span data-ttu-id="c0be4-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c0be4-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "complianceUrl": "https://portal.mdm.contoso.com/?portalAction=Compliance",
    "description": "Contoso mobilty app is a cloud-based  Endpoint Management solution for managing Windows.",
    "discoveryUrl": "https://enrollment.mdm.contoso.com/enrollmentserver/discovery.svc",
    "displayName": "Contoso mobilty app",
    "termsOfUseUrl": "https://portal.mdm.contoso.com/TermsofUse.aspx",
    "includedGroups": [
      {
        "id": "dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef",
        "displayName": "Test MDM Group"
      }
    ]
  }
}
```
