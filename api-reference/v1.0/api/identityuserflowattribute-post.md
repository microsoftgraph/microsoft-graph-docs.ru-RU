---
title: Создание identityUserFlowAttribute
description: Создание нового объекта identityUserFlowAttribute.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 3b5298d433e9ee79ff141f73b1081c7a72374feb
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883008"
---
# <a name="create-identityuserflowattribute"></a><span data-ttu-id="284bb-103">Создание identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="284bb-103">Create identityUserFlowAttribute</span></span>

<span data-ttu-id="284bb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="284bb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="284bb-105">Создание нового [объекта identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="284bb-105">Create a new [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="284bb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="284bb-106">Permissions</span></span>

<span data-ttu-id="284bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="284bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="284bb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="284bb-109">Permission type</span></span>      | <span data-ttu-id="284bb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="284bb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="284bb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="284bb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="284bb-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="284bb-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="284bb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="284bb-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="284bb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="284bb-114">Not supported.</span></span>|
|<span data-ttu-id="284bb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="284bb-115">Application</span></span>|<span data-ttu-id="284bb-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="284bb-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="284bb-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="284bb-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="284bb-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="284bb-118">Global administrator</span></span>
* <span data-ttu-id="284bb-119">Администратор атрибута потока внешних удостоверений</span><span class="sxs-lookup"><span data-stu-id="284bb-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="284bb-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="284bb-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="284bb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="284bb-121">Request headers</span></span>

|<span data-ttu-id="284bb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="284bb-122">Name</span></span>|<span data-ttu-id="284bb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="284bb-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="284bb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="284bb-124">Authorization</span></span>|<span data-ttu-id="284bb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="284bb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="284bb-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="284bb-127">Content-Type</span></span>|<span data-ttu-id="284bb-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="284bb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="284bb-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="284bb-130">Request body</span></span>

<span data-ttu-id="284bb-131">В теле запроса предопределять представление JSON [identityUserFlowAttribute.](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="284bb-131">In the request body, provide a JSON representation of [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>

|<span data-ttu-id="284bb-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="284bb-132">Property</span></span>|<span data-ttu-id="284bb-133">Тип</span><span class="sxs-lookup"><span data-stu-id="284bb-133">Type</span></span>|<span data-ttu-id="284bb-134">Описание</span><span class="sxs-lookup"><span data-stu-id="284bb-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="284bb-135">id</span><span class="sxs-lookup"><span data-stu-id="284bb-135">id</span></span>|<span data-ttu-id="284bb-136">String</span><span class="sxs-lookup"><span data-stu-id="284bb-136">String</span></span>|<span data-ttu-id="284bb-137">Идентификатор атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="284bb-137">The identifier of the user flow attribute.</span></span> <span data-ttu-id="284bb-138">Это автоматически созданный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="284bb-138">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="284bb-139">displayName</span><span class="sxs-lookup"><span data-stu-id="284bb-139">displayName</span></span>|<span data-ttu-id="284bb-140">String</span><span class="sxs-lookup"><span data-stu-id="284bb-140">String</span></span>|<span data-ttu-id="284bb-141">Отображаемое имя атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="284bb-141">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="284bb-142">description</span><span class="sxs-lookup"><span data-stu-id="284bb-142">description</span></span>|<span data-ttu-id="284bb-143">Строка</span><span class="sxs-lookup"><span data-stu-id="284bb-143">String</span></span>|<span data-ttu-id="284bb-144">Описание атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="284bb-144">The description of the user flow attribute.</span></span> <span data-ttu-id="284bb-145">Он отображается пользователю во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="284bb-145">It's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="284bb-146">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="284bb-146">userFlowAttributeType</span></span>|<span data-ttu-id="284bb-147">String</span><span class="sxs-lookup"><span data-stu-id="284bb-147">String</span></span>|<span data-ttu-id="284bb-148">Тип атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="284bb-148">The type of the user flow attribute.</span></span> <span data-ttu-id="284bb-149">Это автоматически настроенный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="284bb-149">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="284bb-150">В зависимости от типа атрибута значением этого свойства является `builtIn` или `custom`.</span><span class="sxs-lookup"><span data-stu-id="284bb-150">Depending on the type of attribute, the values for this property will be `builtIn` or `custom`.</span></span>|
|<span data-ttu-id="284bb-151">dataType</span><span class="sxs-lookup"><span data-stu-id="284bb-151">dataType</span></span>|<span data-ttu-id="284bb-152">String</span><span class="sxs-lookup"><span data-stu-id="284bb-152">String</span></span>|<span data-ttu-id="284bb-153">Тип данных атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="284bb-153">The data type of the user flow attribute.</span></span> <span data-ttu-id="284bb-154">Это невозможно изменить после создания настраиваемой атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="284bb-154">This cannot be modified once the custom user flow attribute is created.</span></span> <span data-ttu-id="284bb-155">Поддерживаемые значения для **dataType**:</span><span class="sxs-lookup"><span data-stu-id="284bb-155">The supported values for **dataType** are:</span></span><br/><ul><li>`string` </li><li>`boolean`</li><li>`int64`</li></ul>|

## <a name="response"></a><span data-ttu-id="284bb-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="284bb-156">Response</span></span>

<span data-ttu-id="284bb-157">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект identityUserFlowAttribute](../resources/identityuserflowattribute.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="284bb-157">If successful, this method returns a `201 Created` response code and [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object in the response body.</span></span> <span data-ttu-id="284bb-158">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="284bb-158">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="284bb-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="284bb-159">Examples</span></span>

### <a name="request"></a><span data-ttu-id="284bb-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="284bb-160">Request</span></span>

<span data-ttu-id="284bb-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="284bb-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_userFlowAttribute_from_userFlowAttributes"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/userFlowAttributes
Content-type: application/json

{
  "displayName": "Hobby",
  "description": "Your hobby",
  "dataType": "string",
}
```

### <a name="response"></a><span data-ttu-id="284bb-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="284bb-162">Response</span></span>

<span data-ttu-id="284bb-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="284bb-163">The following is an example of the response.</span></span>

<span data-ttu-id="284bb-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="284bb-164">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/identity/userFlowAttributes/extension_7a95ecd9489b4fb9a45722b913c4703b_Hobby
Content-type: application/json

{
    "id": "extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby",
    "displayName": "Hobby",
    "description": "Your hobby",
    "userFlowAttributeType": "custom",
    "dataType": "string"
}
```
