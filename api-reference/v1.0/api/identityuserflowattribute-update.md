---
title: Обновление identityUserFlowAttribute
description: Обновление свойств identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: d998a5501443c026d685ac8eaec7910312d35967
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883334"
---
# <a name="update-identityuserflowattribute"></a><span data-ttu-id="0536e-103">Обновление identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="0536e-103">Update identityUserFlowAttribute</span></span>

<span data-ttu-id="0536e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0536e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0536e-105">Обновление свойств объекта [identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="0536e-105">Update the properties of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span> <span data-ttu-id="0536e-106">Можно обновить только настраиваемые атрибуты потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="0536e-106">Only custom user flow attributes can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="0536e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0536e-107">Permissions</span></span>

<span data-ttu-id="0536e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0536e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0536e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0536e-110">Permission type</span></span>      | <span data-ttu-id="0536e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0536e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0536e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0536e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0536e-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0536e-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="0536e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0536e-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0536e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0536e-115">Not supported.</span></span>|
|<span data-ttu-id="0536e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0536e-116">Application</span></span>| <span data-ttu-id="0536e-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0536e-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="0536e-118">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="0536e-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0536e-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="0536e-119">Global administrator</span></span>
* <span data-ttu-id="0536e-120">Администратор атрибутов потока внешних удостоверений пользователей</span><span class="sxs-lookup"><span data-stu-id="0536e-120">External Identity User Flow Attributes administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0536e-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0536e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0536e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0536e-122">Request headers</span></span>

|<span data-ttu-id="0536e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="0536e-123">Name</span></span>|<span data-ttu-id="0536e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0536e-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="0536e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0536e-125">Authorization</span></span>|<span data-ttu-id="0536e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0536e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0536e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0536e-128">Content-Type</span></span>|<span data-ttu-id="0536e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0536e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0536e-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0536e-131">Request body</span></span>

<span data-ttu-id="0536e-132">В теле запроса предопределять объект JSON одним или более свойствами, которые необходимо обновить для [объекта identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="0536e-132">In the request body, provide a JSON object with one or more properties that need to be updated for an [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

><span data-ttu-id="0536e-133">**Примечание:** Только свойство **описания** может быть обновлено.</span><span class="sxs-lookup"><span data-stu-id="0536e-133">**Note:** Only the **description** property can be updated.</span></span>

|<span data-ttu-id="0536e-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="0536e-134">Property</span></span>|<span data-ttu-id="0536e-135">Тип</span><span class="sxs-lookup"><span data-stu-id="0536e-135">Type</span></span>|<span data-ttu-id="0536e-136">Описание</span><span class="sxs-lookup"><span data-stu-id="0536e-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0536e-137">description</span><span class="sxs-lookup"><span data-stu-id="0536e-137">description</span></span>|<span data-ttu-id="0536e-138">Строка</span><span class="sxs-lookup"><span data-stu-id="0536e-138">String</span></span>|<span data-ttu-id="0536e-139">Описание атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="0536e-139">The description of the user flow attribute.</span></span> <span data-ttu-id="0536e-140">Он отображается пользователю во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="0536e-140">It is shown to the user at the time of sign up.</span></span>|

## <a name="response"></a><span data-ttu-id="0536e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0536e-141">Response</span></span>

<span data-ttu-id="0536e-142">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0536e-142">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="0536e-143">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="0536e-143">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="0536e-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="0536e-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0536e-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="0536e-145">Request</span></span>

<span data-ttu-id="0536e-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0536e-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_userFlowAttributes"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby
Content-type: application/json

{
  "description": "Your new hobby"
}
```

### <a name="response"></a><span data-ttu-id="0536e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0536e-147">Response</span></span>

<span data-ttu-id="0536e-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0536e-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
