---
title: Создание userAttributeAssignments
description: Создайте новый объект identityUserFlowAttributeAssignment.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 52e459d65820ca1225e5aefe2eafff0f5a044ecc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944693"
---
# <a name="create-userattributeassignments"></a><span data-ttu-id="9f25c-103">Создание userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="9f25c-103">Create userAttributeAssignments</span></span>

<span data-ttu-id="9f25c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f25c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f25c-105">Создайте новый объект identityUserFlowAttributeAssignment в [b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="9f25c-105">Create a new identityUserFlowAttributeAssignment object in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9f25c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f25c-106">Permissions</span></span>

<span data-ttu-id="9f25c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f25c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f25c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f25c-109">Permission type</span></span>|<span data-ttu-id="9f25c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f25c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f25c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f25c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f25c-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f25c-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="9f25c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f25c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f25c-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9f25c-114">Not supported</span></span>|
|<span data-ttu-id="9f25c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9f25c-115">Application</span></span>|<span data-ttu-id="9f25c-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f25c-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f25c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f25c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2cUserFlows/{id}/userAttributeAssignments
```

## <a name="request-headers"></a><span data-ttu-id="9f25c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f25c-118">Request headers</span></span>

|<span data-ttu-id="9f25c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9f25c-119">Name</span></span>|<span data-ttu-id="9f25c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9f25c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9f25c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f25c-121">Authorization</span></span>|<span data-ttu-id="9f25c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f25c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9f25c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9f25c-124">Content-Type</span></span>|<span data-ttu-id="9f25c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f25c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f25c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f25c-127">Request body</span></span>

<span data-ttu-id="9f25c-128">В теле запроса подарят представление JSON объекта [identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9f25c-128">In the request body, supply a JSON representation of the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

<span data-ttu-id="9f25c-129">В следующей таблице показаны свойства, необходимые при создании [identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9f25c-129">The following table shows the properties that are required when you create the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span></span>

|<span data-ttu-id="9f25c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f25c-130">Property</span></span>|<span data-ttu-id="9f25c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9f25c-131">Type</span></span>|<span data-ttu-id="9f25c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9f25c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f25c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9f25c-133">displayName</span></span>|<span data-ttu-id="9f25c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9f25c-134">String</span></span>|<span data-ttu-id="9f25c-135">Отображение имени identityUserFlowAttribute в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="9f25c-135">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="9f25c-136">isOptional</span><span class="sxs-lookup"><span data-stu-id="9f25c-136">isOptional</span></span>|<span data-ttu-id="9f25c-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f25c-137">Boolean</span></span>|<span data-ttu-id="9f25c-138">Определяет, является ли identityUserFlowAttribute необязательным.</span><span class="sxs-lookup"><span data-stu-id="9f25c-138">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="9f25c-139">`true` означает, что пользователю не нужно предоставлять значение.</span><span class="sxs-lookup"><span data-stu-id="9f25c-139">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="9f25c-140">`false` означает, что пользователь не может завершить регистрацию без предоставления значения.</span><span class="sxs-lookup"><span data-stu-id="9f25c-140">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="9f25c-141">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="9f25c-141">requiresVerification</span></span>|<span data-ttu-id="9f25c-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f25c-142">Boolean</span></span>|<span data-ttu-id="9f25c-143">Определяет, требуется ли проверка identityUserFlowAttribute.</span><span class="sxs-lookup"><span data-stu-id="9f25c-143">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="9f25c-144">Это используется только для проверки номера телефона или адреса электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f25c-144">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="9f25c-145">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="9f25c-145">userAttributeValues</span></span>|<span data-ttu-id="9f25c-146">[коллекция userAttributeValuesItem](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="9f25c-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="9f25c-147">Параметры ввода атрибута потока пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f25c-147">The input options for the user flow attribute.</span></span> <span data-ttu-id="9f25c-148">Применимо только в том случае, если userInputType `radioSingleSelect` является `dropdownSingleSelect` , или `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="9f25c-148">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="9f25c-149">userInputType</span><span class="sxs-lookup"><span data-stu-id="9f25c-149">userInputType</span></span>|<span data-ttu-id="9f25c-150">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="9f25c-150">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="9f25c-151">Тип ввода атрибута потока пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f25c-151">The input type of the user flow attribute.</span></span> <span data-ttu-id="9f25c-152">Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="9f25c-152">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="9f25c-153">userAttribute</span><span class="sxs-lookup"><span data-stu-id="9f25c-153">userAttribute</span></span>|[<span data-ttu-id="9f25c-154">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="9f25c-154">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="9f25c-155">Идентификатор атрибута потока пользователей, который должен включаться в назначение потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="9f25c-155">The identifier for the user flow attribute to include in the user flow assignment.</span></span>

## <a name="response"></a><span data-ttu-id="9f25c-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f25c-156">Response</span></span>

<span data-ttu-id="9f25c-157">В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9f25c-157">If successful, this method returns a `201 Created` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f25c-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="9f25c-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9f25c-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f25c-159">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9f25c-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f25c-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityuserflowattributeassignment_from__1"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Consumer/userAttributeAssignments
Content-Type: application/json

{
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "Shoe size",
    "userAttributeValues": [],
    "userAttribute": {
        "id": "extension_guid_shoeSize"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="9f25c-161">C#</span><span class="sxs-lookup"><span data-stu-id="9f25c-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflowattributeassignment-from--1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f25c-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f25c-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflowattributeassignment-from--1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f25c-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f25c-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflowattributeassignment-from--1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f25c-164">Java</span><span class="sxs-lookup"><span data-stu-id="9f25c-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityuserflowattributeassignment-from--1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9f25c-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f25c-165">Response</span></span>

<span data-ttu-id="9f25c-166">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9f25c-166">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2C_1_Consumer/userAttributeAssignments/extension_guid_shoeSize
Content-Type: application/json

{
    "id": "extension_guid_shoeSize",
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "Shoe size",
    "userAttributeValues": []
}
```
