---
title: Список включенGroups
description: Получите список групп, включенных в политику управления мобильными приложениями.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7f0d48a74ce11a3809a42f9f2c26a8075d33155a
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440984"
---
# <a name="list-includedgroups"></a><span data-ttu-id="b9620-103">Список включенGroups</span><span class="sxs-lookup"><span data-stu-id="b9620-103">List includedGroups</span></span>

<span data-ttu-id="b9620-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9620-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9620-105">Получите список групп, включенных в политику управления мобильными приложениями.</span><span class="sxs-lookup"><span data-stu-id="b9620-105">Get the list of groups that are included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9620-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9620-106">Permissions</span></span>

<span data-ttu-id="b9620-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9620-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9620-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9620-109">Permission type</span></span>|<span data-ttu-id="b9620-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9620-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9620-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9620-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b9620-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="b9620-112">Policy.Read.All, Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="b9620-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9620-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9620-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9620-114">Not supported.</span></span>|
|<span data-ttu-id="b9620-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9620-115">Application</span></span> | <span data-ttu-id="b9620-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9620-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9620-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9620-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /policies/mobileAppManagementPolicies/{id}/includedGroups
```

## <a name="request-headers"></a><span data-ttu-id="b9620-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9620-118">Request headers</span></span>

|<span data-ttu-id="b9620-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b9620-119">Name</span></span>|<span data-ttu-id="b9620-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b9620-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b9620-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9620-121">Authorization</span></span>|<span data-ttu-id="b9620-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9620-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9620-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9620-124">Request body</span></span>

<span data-ttu-id="b9620-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9620-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9620-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9620-126">Response</span></span>

<span data-ttu-id="b9620-127">В случае успешной работы этот метод возвращает код отклика и коллекцию групповых `200 OK` объектов в тексте ответа. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="b9620-127">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9620-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="b9620-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9620-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9620-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b9620-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9620-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->

``` http
GET https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups
```
# <a name="c"></a>[<span data-ttu-id="b9620-131">C#</span><span class="sxs-lookup"><span data-stu-id="b9620-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9620-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9620-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9620-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9620-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9620-134">Java</span><span class="sxs-lookup"><span data-stu-id="b9620-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b9620-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9620-135">Response</span></span>

><span data-ttu-id="b9620-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b9620-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.group)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "800c583d-cc3d-4361-8e4a-3fbf668f27f4",
      "displayName": "Test Group"
    }
  ]
}
```
