---
title: Удаление mobileDeviceManagementPolicy
description: Удаление политики управления мобильными устройствами.
author: michaelrm97
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4ec86977e3abbb704098936051995e28ebace5c0
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440754"
---
# <a name="delete-mobiledevicemanagementpolicy"></a><span data-ttu-id="f748e-103">Удаление mobileDeviceManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="f748e-103">Delete mobileDeviceManagementPolicy</span></span>

<span data-ttu-id="f748e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f748e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f748e-105">Удаление [объекта mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f748e-105">Delete a [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="f748e-106">Эта операция поддерживается только в том случае, если политика больше не действительна; то есть, если **свойство isValid** является ложным, что указывает на удаление основного объекта службы, связанного с приложением для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f748e-106">This operation is only supported when the policy is no longer valid; that is, when the **isValid** property is false, which indicates that the service principal associated with the application for this policy has been deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="f748e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f748e-107">Permissions</span></span>

<span data-ttu-id="f748e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f748e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f748e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f748e-110">Permission type</span></span>|<span data-ttu-id="f748e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f748e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f748e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f748e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f748e-113">Policy.ReadWrite.MobilityManagement</span><span class="sxs-lookup"><span data-stu-id="f748e-113">Policy.ReadWrite.MobilityManagement</span></span>|
|<span data-ttu-id="f748e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f748e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f748e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f748e-115">Not supported.</span></span>|
|<span data-ttu-id="f748e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f748e-116">Application</span></span> | <span data-ttu-id="f748e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f748e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f748e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f748e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/mobileDeviceManagementPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f748e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f748e-119">Request headers</span></span>

|<span data-ttu-id="f748e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f748e-120">Name</span></span>|<span data-ttu-id="f748e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f748e-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f748e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f748e-122">Authorization</span></span>|<span data-ttu-id="f748e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f748e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f748e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f748e-125">Request body</span></span>

<span data-ttu-id="f748e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f748e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f748e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f748e-127">Response</span></span>

<span data-ttu-id="f748e-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f748e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f748e-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="f748e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f748e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f748e-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f748e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f748e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mobilitymanagementpolicy"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
```
# <a name="c"></a>[<span data-ttu-id="f748e-133">C#</span><span class="sxs-lookup"><span data-stu-id="f748e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mobilitymanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f748e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f748e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mobilitymanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f748e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f748e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mobilitymanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f748e-136">Java</span><span class="sxs-lookup"><span data-stu-id="f748e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-mobilitymanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f748e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f748e-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
