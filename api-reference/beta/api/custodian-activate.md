---
title: 'custodian: activate'
description: Повторно активировать хранителя в деле.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 675e62b24b126b2ad37263f3c9a1d57e42bd37e7
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659365"
---
# <a name="custodian-activate"></a><span data-ttu-id="6ec8b-103">custodian: activate</span><span class="sxs-lookup"><span data-stu-id="6ec8b-103">custodian: activate</span></span>

<span data-ttu-id="6ec8b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ec8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ec8b-105">Активируйте хранителя, который был освобожден из дела, чтобы снова сделать его частью дела.</span><span class="sxs-lookup"><span data-stu-id="6ec8b-105">Activate a custodian that has been released from a case to make them part of the case again.</span></span> <span data-ttu-id="6ec8b-106">Дополнительные сведения см. в [деле "Управление хранителями" в деле Advanced eDiscovery.](/microsoft-365/compliance/manage-new-custodians#re-activate-custodian)</span><span class="sxs-lookup"><span data-stu-id="6ec8b-106">For details, see [Manage custodians in an Advanced eDiscovery case](/microsoft-365/compliance/manage-new-custodians#re-activate-custodian).</span></span>

## <a name="permissions"></a><span data-ttu-id="6ec8b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ec8b-107">Permissions</span></span>

<span data-ttu-id="6ec8b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ec8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ec8b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ec8b-110">Permission type</span></span>|<span data-ttu-id="6ec8b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ec8b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ec8b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ec8b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6ec8b-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="6ec8b-113">User.Read</span></span>|
|<span data-ttu-id="6ec8b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ec8b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ec8b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ec8b-115">Not supported.</span></span>|
|<span data-ttu-id="6ec8b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ec8b-116">Application</span></span>|<span data-ttu-id="6ec8b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ec8b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ec8b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ec8b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/activate
```

## <a name="request-headers"></a><span data-ttu-id="6ec8b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ec8b-119">Request headers</span></span>

|<span data-ttu-id="6ec8b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6ec8b-120">Name</span></span>|<span data-ttu-id="6ec8b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6ec8b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6ec8b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ec8b-122">Authorization</span></span>|<span data-ttu-id="6ec8b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ec8b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6ec8b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6ec8b-125">Content-Type</span></span>|<span data-ttu-id="6ec8b-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ec8b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ec8b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ec8b-128">Request body</span></span>

<span data-ttu-id="6ec8b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ec8b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ec8b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ec8b-130">Response</span></span>

<span data-ttu-id="6ec8b-131">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6ec8b-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6ec8b-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="6ec8b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6ec8b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ec8b-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6ec8b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ec8b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "custodian_activate"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/activate
```
# <a name="c"></a>[<span data-ttu-id="6ec8b-135">C#</span><span class="sxs-lookup"><span data-stu-id="6ec8b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/custodian-activate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ec8b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ec8b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/custodian-activate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ec8b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ec8b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/custodian-activate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6ec8b-138">Java</span><span class="sxs-lookup"><span data-stu-id="6ec8b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/custodian-activate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6ec8b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ec8b-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
