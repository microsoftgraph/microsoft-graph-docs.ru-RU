---
title: Удаление includeGroup
description: Удаление группы из списка групп, включенных в политику управления мобильными устройствами.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5fb051f94ec95d5fea05b19a9273a3ec6cf0d349
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401612"
---
# <a name="delete-includedgroup"></a><span data-ttu-id="6977f-103">Delete includedGroup</span><span class="sxs-lookup"><span data-stu-id="6977f-103">Delete includedGroup</span></span>

<span data-ttu-id="6977f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6977f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6977f-105">Удаление группы из списка групп, включенных в политику управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="6977f-105">Delete a group from the list of groups included in a mobile device management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="6977f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6977f-106">Permissions</span></span>

<span data-ttu-id="6977f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6977f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6977f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6977f-109">Permission type</span></span>|<span data-ttu-id="6977f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6977f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6977f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6977f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6977f-112">Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="6977f-112">Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="6977f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6977f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6977f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6977f-114">Not supported.</span></span>|
|<span data-ttu-id="6977f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6977f-115">Application</span></span> | <span data-ttu-id="6977f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6977f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6977f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6977f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/mobileDeviceManagementPolicies/{id}/includedGroups/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6977f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6977f-118">Request headers</span></span>

|<span data-ttu-id="6977f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6977f-119">Name</span></span>|<span data-ttu-id="6977f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6977f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6977f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6977f-121">Authorization</span></span>|<span data-ttu-id="6977f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6977f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6977f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6977f-124">Request body</span></span>

<span data-ttu-id="6977f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6977f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6977f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="6977f-126">Response</span></span>

<span data-ttu-id="6977f-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6977f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6977f-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="6977f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6977f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6977f-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6977f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6977f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef/$ref
```
# <a name="c"></a>[<span data-ttu-id="6977f-132">C#</span><span class="sxs-lookup"><span data-stu-id="6977f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6977f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6977f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6977f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6977f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6977f-135">Java</span><span class="sxs-lookup"><span data-stu-id="6977f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6977f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6977f-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
