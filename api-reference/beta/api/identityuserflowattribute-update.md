---
title: Обновление Идентитюсерфловаттрибуте
description: Обновление свойств объекта Идентитюсерфловаттрибуте.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e62916b373043a2da479d4fa77338362b1621291
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904010"
---
# <a name="update-identityuserflowattribute"></a><span data-ttu-id="d3793-103">Обновление Идентитюсерфловаттрибуте</span><span class="sxs-lookup"><span data-stu-id="d3793-103">Update identityUserFlowAttribute</span></span>

<span data-ttu-id="d3793-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3793-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3793-105">Обновление свойств объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="d3793-105">Update the properties of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span> <span data-ttu-id="d3793-106">Можно обновлять только настраиваемые атрибуты пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="d3793-106">Only custom user flow attributes can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3793-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3793-107">Permissions</span></span>

<span data-ttu-id="d3793-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3793-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3793-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3793-110">Permission type</span></span>      | <span data-ttu-id="d3793-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3793-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3793-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3793-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d3793-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3793-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="d3793-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3793-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d3793-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3793-115">Not supported.</span></span>|
|<span data-ttu-id="d3793-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3793-116">Application</span></span>| <span data-ttu-id="d3793-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3793-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="d3793-118">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="d3793-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d3793-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d3793-119">Global administrator</span></span>
* <span data-ttu-id="d3793-120">Внешний идентификатор пользователя Администратор атрибутов пользовательского процесса</span><span class="sxs-lookup"><span data-stu-id="d3793-120">External Identity User Flow Attributes administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d3793-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3793-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d3793-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3793-122">Request headers</span></span>

|<span data-ttu-id="d3793-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d3793-123">Name</span></span>|<span data-ttu-id="d3793-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d3793-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d3793-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3793-125">Authorization</span></span>|<span data-ttu-id="d3793-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3793-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d3793-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3793-128">Content-Type</span></span>|<span data-ttu-id="d3793-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3793-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3793-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3793-131">Request body</span></span>

<span data-ttu-id="d3793-132">В тексте запроса укажите объект JSON с одним или несколькими свойствами, которые необходимо обновить для объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="d3793-132">In the request body, provide a JSON object with one or more properties that need to be updated for an [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

><span data-ttu-id="d3793-133">**Примечание:** Можно обновить только свойство **Description** .</span><span class="sxs-lookup"><span data-stu-id="d3793-133">**Note:** Only the **description** property can be updated.</span></span>

|<span data-ttu-id="d3793-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3793-134">Property</span></span>|<span data-ttu-id="d3793-135">Тип</span><span class="sxs-lookup"><span data-stu-id="d3793-135">Type</span></span>|<span data-ttu-id="d3793-136">Описание</span><span class="sxs-lookup"><span data-stu-id="d3793-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3793-137">description</span><span class="sxs-lookup"><span data-stu-id="d3793-137">description</span></span>|<span data-ttu-id="d3793-138">String</span><span class="sxs-lookup"><span data-stu-id="d3793-138">String</span></span>|<span data-ttu-id="d3793-139">Описание атрибута Flow User.</span><span class="sxs-lookup"><span data-stu-id="d3793-139">The description of the user flow attribute.</span></span> <span data-ttu-id="d3793-140">Он отображается для пользователя во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="d3793-140">It is shown to the user at the time of sign up.</span></span>|

## <a name="response"></a><span data-ttu-id="d3793-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3793-141">Response</span></span>

<span data-ttu-id="d3793-142">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d3793-142">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="d3793-143">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="d3793-143">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="d3793-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="d3793-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3793-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3793-145">Request</span></span>

<span data-ttu-id="d3793-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3793-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d3793-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3793-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_userFlowAttributes"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby
Content-type: application/json

{
  "description": "Your new hobby"
}
```
# <a name="c"></a>[<span data-ttu-id="d3793-148">C#</span><span class="sxs-lookup"><span data-stu-id="d3793-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3793-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3793-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3793-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3793-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3793-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3793-151">Response</span></span>

<span data-ttu-id="d3793-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d3793-152">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
