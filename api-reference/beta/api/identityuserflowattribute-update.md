---
title: Обновление identityUserFlowAttribute
description: Обновление свойств identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 7f9f5589069e6b96115f73edb653d7262efe445a
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625823"
---
# <a name="update-identityuserflowattribute"></a><span data-ttu-id="d7e2e-103">Обновление identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="d7e2e-103">Update identityUserFlowAttribute</span></span>

<span data-ttu-id="d7e2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7e2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7e2e-105">Обновление свойств объекта [identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="d7e2e-105">Update the properties of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span> <span data-ttu-id="d7e2e-106">Можно обновить только настраиваемые атрибуты потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="d7e2e-106">Only custom user flow attributes can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7e2e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7e2e-107">Permissions</span></span>

<span data-ttu-id="d7e2e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7e2e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7e2e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7e2e-110">Permission type</span></span>      | <span data-ttu-id="d7e2e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7e2e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7e2e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7e2e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7e2e-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7e2e-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="d7e2e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7e2e-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d7e2e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7e2e-115">Not supported.</span></span>|
|<span data-ttu-id="d7e2e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d7e2e-116">Application</span></span>| <span data-ttu-id="d7e2e-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7e2e-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="d7e2e-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="d7e2e-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d7e2e-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d7e2e-119">Global administrator</span></span>
* <span data-ttu-id="d7e2e-120">Администратор атрибутов потока внешних удостоверений пользователей</span><span class="sxs-lookup"><span data-stu-id="d7e2e-120">External Identity User Flow Attributes administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d7e2e-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7e2e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d7e2e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7e2e-122">Request headers</span></span>

|<span data-ttu-id="d7e2e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d7e2e-123">Name</span></span>|<span data-ttu-id="d7e2e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d7e2e-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d7e2e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7e2e-125">Authorization</span></span>|<span data-ttu-id="d7e2e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7e2e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d7e2e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d7e2e-128">Content-Type</span></span>|<span data-ttu-id="d7e2e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7e2e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7e2e-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7e2e-131">Request body</span></span>

<span data-ttu-id="d7e2e-132">В теле запроса предопределять объект JSON одним или более свойствами, которые необходимо обновить для [объекта identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="d7e2e-132">In the request body, provide a JSON object with one or more properties that need to be updated for an [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

><span data-ttu-id="d7e2e-133">**Примечание:** Только свойство **описания** может быть обновлено.</span><span class="sxs-lookup"><span data-stu-id="d7e2e-133">**Note:** Only the **description** property can be updated.</span></span>

|<span data-ttu-id="d7e2e-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7e2e-134">Property</span></span>|<span data-ttu-id="d7e2e-135">Тип</span><span class="sxs-lookup"><span data-stu-id="d7e2e-135">Type</span></span>|<span data-ttu-id="d7e2e-136">Описание</span><span class="sxs-lookup"><span data-stu-id="d7e2e-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7e2e-137">description</span><span class="sxs-lookup"><span data-stu-id="d7e2e-137">description</span></span>|<span data-ttu-id="d7e2e-138">String</span><span class="sxs-lookup"><span data-stu-id="d7e2e-138">String</span></span>|<span data-ttu-id="d7e2e-139">Описание атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="d7e2e-139">The description of the user flow attribute.</span></span> <span data-ttu-id="d7e2e-140">Он отображается пользователю во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="d7e2e-140">It is shown to the user at the time of sign up.</span></span>|

## <a name="response"></a><span data-ttu-id="d7e2e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7e2e-141">Response</span></span>

<span data-ttu-id="d7e2e-142">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d7e2e-142">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="d7e2e-143">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="d7e2e-143">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="d7e2e-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="d7e2e-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d7e2e-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7e2e-145">Request</span></span>

<span data-ttu-id="d7e2e-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7e2e-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d7e2e-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7e2e-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d7e2e-148">C#</span><span class="sxs-lookup"><span data-stu-id="d7e2e-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7e2e-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7e2e-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7e2e-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7e2e-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7e2e-151">Java</span><span class="sxs-lookup"><span data-stu-id="d7e2e-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d7e2e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7e2e-152">Response</span></span>

<span data-ttu-id="d7e2e-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d7e2e-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
