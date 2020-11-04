---
title: Удаление Идентитюсерфловаттрибуте
description: Удаление Идентитюсерфловаттрибуте.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6912769c140a95054c30c67defc4068a5a8b4e43
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904133"
---
# <a name="delete-identityuserflowattribute"></a><span data-ttu-id="b4cdd-103">Удаление Идентитюсерфловаттрибуте</span><span class="sxs-lookup"><span data-stu-id="b4cdd-103">Delete identityUserFlowAttribute</span></span>

<span data-ttu-id="b4cdd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4cdd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4cdd-105">Удаление [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="b4cdd-105">Delete an [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="b4cdd-106">Удалить можно только настраиваемые атрибуты пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="b4cdd-106">Only custom user flow attributes can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4cdd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4cdd-107">Permissions</span></span>

<span data-ttu-id="b4cdd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4cdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4cdd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4cdd-110">Permission type</span></span>      | <span data-ttu-id="b4cdd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4cdd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4cdd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4cdd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b4cdd-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4cdd-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="b4cdd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4cdd-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b4cdd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4cdd-115">Not supported.</span></span>|
|<span data-ttu-id="b4cdd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4cdd-116">Application</span></span>|<span data-ttu-id="b4cdd-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4cdd-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="b4cdd-118">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="b4cdd-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="b4cdd-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b4cdd-119">Global administrator</span></span>
* <span data-ttu-id="b4cdd-120">Администратор атрибутов пользовательского процесса внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="b4cdd-120">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="b4cdd-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4cdd-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b4cdd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4cdd-122">Request headers</span></span>

|<span data-ttu-id="b4cdd-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b4cdd-123">Name</span></span>|<span data-ttu-id="b4cdd-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b4cdd-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b4cdd-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4cdd-125">Authorization</span></span>|<span data-ttu-id="b4cdd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4cdd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4cdd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4cdd-128">Request body</span></span>

<span data-ttu-id="b4cdd-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4cdd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4cdd-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4cdd-130">Response</span></span>

<span data-ttu-id="b4cdd-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b4cdd-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4cdd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b4cdd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4cdd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4cdd-133">Request</span></span>

<span data-ttu-id="b4cdd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4cdd-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b4cdd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4cdd-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userFlowAttributes"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/userFlowAttributes/{id}
```
# <a name="c"></a>[<span data-ttu-id="b4cdd-136">C#</span><span class="sxs-lookup"><span data-stu-id="b4cdd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4cdd-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4cdd-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4cdd-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4cdd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b4cdd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4cdd-139">Response</span></span>

<span data-ttu-id="b4cdd-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4cdd-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
