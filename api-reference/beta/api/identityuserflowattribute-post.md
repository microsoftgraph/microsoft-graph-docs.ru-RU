---
title: Создание Идентитюсерфловаттрибуте
description: Создание нового объекта Идентитюсерфловаттрибуте.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 816b9e94ca95ec61f7a9628de7ede6617cebb7fd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953144"
---
# <a name="create-identityuserflowattribute"></a><span data-ttu-id="fe87e-103">Создание Идентитюсерфловаттрибуте</span><span class="sxs-lookup"><span data-stu-id="fe87e-103">Create identityUserFlowAttribute</span></span>

<span data-ttu-id="fe87e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe87e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe87e-105">Создание нового объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) .</span><span class="sxs-lookup"><span data-stu-id="fe87e-105">Create a new [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe87e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe87e-106">Permissions</span></span>

<span data-ttu-id="fe87e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe87e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe87e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe87e-109">Permission type</span></span>      | <span data-ttu-id="fe87e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe87e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe87e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe87e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fe87e-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe87e-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="fe87e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe87e-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fe87e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe87e-114">Not supported.</span></span>|
|<span data-ttu-id="fe87e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe87e-115">Application</span></span>|<span data-ttu-id="fe87e-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe87e-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="fe87e-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="fe87e-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="fe87e-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="fe87e-118">Global administrator</span></span>
* <span data-ttu-id="fe87e-119">Администратор атрибутов пользовательского процесса внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="fe87e-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="fe87e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe87e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="fe87e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe87e-121">Request headers</span></span>

|<span data-ttu-id="fe87e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="fe87e-122">Name</span></span>|<span data-ttu-id="fe87e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fe87e-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="fe87e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe87e-124">Authorization</span></span>|<span data-ttu-id="fe87e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe87e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fe87e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe87e-127">Content-Type</span></span>|<span data-ttu-id="fe87e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe87e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe87e-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe87e-130">Request body</span></span>

<span data-ttu-id="fe87e-131">В тексте запроса предоставьте представление объекта [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md)в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe87e-131">In the request body, provide a JSON representation of [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>

|<span data-ttu-id="fe87e-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe87e-132">Property</span></span>|<span data-ttu-id="fe87e-133">Тип</span><span class="sxs-lookup"><span data-stu-id="fe87e-133">Type</span></span>|<span data-ttu-id="fe87e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="fe87e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe87e-135">id</span><span class="sxs-lookup"><span data-stu-id="fe87e-135">id</span></span>|<span data-ttu-id="fe87e-136">String</span><span class="sxs-lookup"><span data-stu-id="fe87e-136">String</span></span>|<span data-ttu-id="fe87e-137">Идентификатор атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="fe87e-137">The identifier of the user flow attribute.</span></span> <span data-ttu-id="fe87e-138">Это автоматически созданный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe87e-138">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="fe87e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="fe87e-139">displayName</span></span>|<span data-ttu-id="fe87e-140">String</span><span class="sxs-lookup"><span data-stu-id="fe87e-140">String</span></span>|<span data-ttu-id="fe87e-141">Отображаемое имя атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="fe87e-141">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="fe87e-142">description</span><span class="sxs-lookup"><span data-stu-id="fe87e-142">description</span></span>|<span data-ttu-id="fe87e-143">String</span><span class="sxs-lookup"><span data-stu-id="fe87e-143">String</span></span>|<span data-ttu-id="fe87e-144">Описание атрибута Flow User.</span><span class="sxs-lookup"><span data-stu-id="fe87e-144">The description of the user flow attribute.</span></span> <span data-ttu-id="fe87e-145">Он отображается для пользователя во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="fe87e-145">It's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="fe87e-146">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="fe87e-146">userFlowAttributeType</span></span>|<span data-ttu-id="fe87e-147">String</span><span class="sxs-lookup"><span data-stu-id="fe87e-147">String</span></span>|<span data-ttu-id="fe87e-148">Тип атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="fe87e-148">The type of the user flow attribute.</span></span> <span data-ttu-id="fe87e-149">Это автоматически настроенный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe87e-149">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="fe87e-150">В зависимости от типа атрибута значением этого свойства является `builtIn` или `custom`.</span><span class="sxs-lookup"><span data-stu-id="fe87e-150">Depending on the type of attribute, the values for this property will be `builtIn` or `custom`.</span></span>|
|<span data-ttu-id="fe87e-151">dataType</span><span class="sxs-lookup"><span data-stu-id="fe87e-151">dataType</span></span>|<span data-ttu-id="fe87e-152">String</span><span class="sxs-lookup"><span data-stu-id="fe87e-152">String</span></span>|<span data-ttu-id="fe87e-153">Тип данных атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="fe87e-153">The data type of the user flow attribute.</span></span> <span data-ttu-id="fe87e-154">Этот параметр нельзя изменить после создания настраиваемого атрибута пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="fe87e-154">This cannot be modified once the custom user flow attribute is created.</span></span> <span data-ttu-id="fe87e-155">Поддерживаемые значения для **dataType** :</span><span class="sxs-lookup"><span data-stu-id="fe87e-155">The supported values for **dataType** are:</span></span><br/><ul><li><span data-ttu-id="fe87e-156">`string` : указывает, что тип данных для Идентитюсерфловаттрибуте является строкой.</span><span class="sxs-lookup"><span data-stu-id="fe87e-156">`string` : denotes that the dataType for the identityUserFlowAttribute is a string.</span></span> </li><li><span data-ttu-id="fe87e-157">`boolean` : указывает, что тип данных для Идентитюсерфловаттрибуте является логическим.</span><span class="sxs-lookup"><span data-stu-id="fe87e-157">`boolean` : denotes that the dataType for the identityUserFlowAttribute is a boolean.</span></span></li><li><span data-ttu-id="fe87e-158">`int64` : указывает, что тип данных для Идентитюсерфловаттрибуте является целым числом.</span><span class="sxs-lookup"><span data-stu-id="fe87e-158">`int64` : denotes that the dataType for the identityUserFlowAttribute is an integer.</span></span></li></ul>|

## <a name="response"></a><span data-ttu-id="fe87e-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe87e-159">Response</span></span>

<span data-ttu-id="fe87e-160">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe87e-160">If successful, this method returns a `201 Created` response code and [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object in the response body.</span></span> <span data-ttu-id="fe87e-161">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="fe87e-161">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="fe87e-162">Примеры</span><span class="sxs-lookup"><span data-stu-id="fe87e-162">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fe87e-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe87e-163">Request</span></span>

<span data-ttu-id="fe87e-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe87e-164">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fe87e-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe87e-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_userFlowAttribute_from_userFlowAttributes"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/userFlowAttributes
Content-type: application/json

{
  "displayName": "Hobby",
  "description": "Your hobby",
  "dataType": "string",
}
```
# <a name="c"></a>[<span data-ttu-id="fe87e-166">C#</span><span class="sxs-lookup"><span data-stu-id="fe87e-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-userflowattribute-from-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe87e-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe87e-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-userflowattribute-from-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe87e-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe87e-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-userflowattribute-from-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe87e-169">Java</span><span class="sxs-lookup"><span data-stu-id="fe87e-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-userflowattribute-from-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fe87e-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe87e-170">Response</span></span>

<span data-ttu-id="fe87e-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fe87e-171">The following is an example of the response.</span></span>

<span data-ttu-id="fe87e-172">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fe87e-172">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/userFlowAttributes/extension_7a95ecd9489b4fb9a45722b913c4703b_Hobby
Content-type: application/json

{
    "id": "extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby",
    "displayName": "Hobby",
    "description": "Your hobby",
    "userFlowAttributeType": "custom",
    "dataType": "string"
}
```
