---
title: Обновление Идентитюсерфловаттрибуте
description: Обновление свойств объекта Идентитюсерфловаттрибуте.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c3bce3e4af9ddef293ae172193b868c4b5e59cf8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953130"
---
# <a name="update-identityuserflowattribute"></a><span data-ttu-id="40b5a-103">Обновление Идентитюсерфловаттрибуте</span><span class="sxs-lookup"><span data-stu-id="40b5a-103">Update identityUserFlowAttribute</span></span>

<span data-ttu-id="40b5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40b5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40b5a-105">Обновление свойств объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="40b5a-105">Update the properties of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span> <span data-ttu-id="40b5a-106">Можно обновлять только настраиваемые атрибуты пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="40b5a-106">Only custom user flow attributes can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="40b5a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40b5a-107">Permissions</span></span>

<span data-ttu-id="40b5a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40b5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40b5a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40b5a-110">Permission type</span></span>      | <span data-ttu-id="40b5a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40b5a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40b5a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40b5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40b5a-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40b5a-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="40b5a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40b5a-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="40b5a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40b5a-115">Not supported.</span></span>|
|<span data-ttu-id="40b5a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40b5a-116">Application</span></span>| <span data-ttu-id="40b5a-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40b5a-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="40b5a-118">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="40b5a-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="40b5a-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="40b5a-119">Global administrator</span></span>
* <span data-ttu-id="40b5a-120">Внешний идентификатор пользователя Администратор атрибутов пользовательского процесса</span><span class="sxs-lookup"><span data-stu-id="40b5a-120">External Identity User Flow Attributes administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="40b5a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40b5a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="40b5a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40b5a-122">Request headers</span></span>

|<span data-ttu-id="40b5a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="40b5a-123">Name</span></span>|<span data-ttu-id="40b5a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="40b5a-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="40b5a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40b5a-125">Authorization</span></span>|<span data-ttu-id="40b5a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40b5a-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="40b5a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="40b5a-128">Content-Type</span></span>|<span data-ttu-id="40b5a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40b5a-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40b5a-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40b5a-131">Request body</span></span>

<span data-ttu-id="40b5a-132">В тексте запроса укажите объект JSON с одним или несколькими свойствами, которые необходимо обновить для объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="40b5a-132">In the request body, provide a JSON object with one or more properties that need to be updated for an [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

><span data-ttu-id="40b5a-133">**Примечание:** Можно обновить только свойство **Description** .</span><span class="sxs-lookup"><span data-stu-id="40b5a-133">**Note:** Only the **description** property can be updated.</span></span>

|<span data-ttu-id="40b5a-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="40b5a-134">Property</span></span>|<span data-ttu-id="40b5a-135">Тип</span><span class="sxs-lookup"><span data-stu-id="40b5a-135">Type</span></span>|<span data-ttu-id="40b5a-136">Описание</span><span class="sxs-lookup"><span data-stu-id="40b5a-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40b5a-137">description</span><span class="sxs-lookup"><span data-stu-id="40b5a-137">description</span></span>|<span data-ttu-id="40b5a-138">String</span><span class="sxs-lookup"><span data-stu-id="40b5a-138">String</span></span>|<span data-ttu-id="40b5a-139">Описание атрибута Flow User.</span><span class="sxs-lookup"><span data-stu-id="40b5a-139">The description of the user flow attribute.</span></span> <span data-ttu-id="40b5a-140">Он отображается для пользователя во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="40b5a-140">It is shown to the user at the time of sign up.</span></span>|

## <a name="response"></a><span data-ttu-id="40b5a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="40b5a-141">Response</span></span>

<span data-ttu-id="40b5a-142">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="40b5a-142">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="40b5a-143">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="40b5a-143">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="40b5a-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="40b5a-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40b5a-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="40b5a-145">Request</span></span>

<span data-ttu-id="40b5a-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40b5a-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="40b5a-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="40b5a-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="40b5a-148">C#</span><span class="sxs-lookup"><span data-stu-id="40b5a-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40b5a-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40b5a-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40b5a-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40b5a-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40b5a-151">Java</span><span class="sxs-lookup"><span data-stu-id="40b5a-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="40b5a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="40b5a-152">Response</span></span>

<span data-ttu-id="40b5a-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="40b5a-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
