---
title: Создание userAttributeAssignments
description: Создание объекта identityUserFlowAttributeAssignment в b2xIdentityUserFlow.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5a330e365cdb5c198136ae52d3edc3ba197b8c47
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689514"
---
# <a name="create-userattributeassignments"></a><span data-ttu-id="a4dc7-103">Создание userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="a4dc7-103">Create userAttributeAssignments</span></span>

<span data-ttu-id="a4dc7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4dc7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4dc7-105">Создание объекта identityUserFlowAttributeAssignment в [b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="a4dc7-105">Create a new identityUserFlowAttributeAssignment object in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a4dc7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4dc7-106">Permissions</span></span>

<span data-ttu-id="a4dc7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4dc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4dc7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4dc7-109">Permission type</span></span>|<span data-ttu-id="a4dc7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4dc7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4dc7-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4dc7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4dc7-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4dc7-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="a4dc7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4dc7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4dc7-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a4dc7-114">Not supported</span></span>|
|<span data-ttu-id="a4dc7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a4dc7-115">Application</span></span>|<span data-ttu-id="a4dc7-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4dc7-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4dc7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4dc7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2xUserFlows/{id}/userAttributeAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a4dc7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4dc7-118">Request headers</span></span>

|<span data-ttu-id="a4dc7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a4dc7-119">Name</span></span>|<span data-ttu-id="a4dc7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a4dc7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a4dc7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4dc7-121">Authorization</span></span>|<span data-ttu-id="a4dc7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4dc7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a4dc7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4dc7-124">Content-Type</span></span>|<span data-ttu-id="a4dc7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4dc7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4dc7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4dc7-127">Request body</span></span>

<span data-ttu-id="a4dc7-128">В теле запроса укажу представление объекта [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="a4dc7-128">In the request body, supply a JSON representation of the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

<span data-ttu-id="a4dc7-129">В следующей таблице показаны свойства, необходимые при создании [объекта identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a4dc7-129">The following table shows the properties that are required when you create the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span></span>

|<span data-ttu-id="a4dc7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4dc7-130">Property</span></span>|<span data-ttu-id="a4dc7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a4dc7-131">Type</span></span>|<span data-ttu-id="a4dc7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a4dc7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4dc7-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a4dc7-133">displayName</span></span>|<span data-ttu-id="a4dc7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a4dc7-134">String</span></span>|<span data-ttu-id="a4dc7-135">Отображаемого имени identityUserFlowAttribute в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="a4dc7-135">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="a4dc7-136">isOptional</span><span class="sxs-lookup"><span data-stu-id="a4dc7-136">isOptional</span></span>|<span data-ttu-id="a4dc7-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4dc7-137">Boolean</span></span>|<span data-ttu-id="a4dc7-138">Определяет, является ли identityUserFlowAttribute необязательным.</span><span class="sxs-lookup"><span data-stu-id="a4dc7-138">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="a4dc7-139">`true` означает, что пользователю не нужно предоставлять значение.</span><span class="sxs-lookup"><span data-stu-id="a4dc7-139">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="a4dc7-140">`false` означает, что пользователь не может завершить регистрацию без предоставления значения.</span><span class="sxs-lookup"><span data-stu-id="a4dc7-140">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="a4dc7-141">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="a4dc7-141">requiresVerification</span></span>|<span data-ttu-id="a4dc7-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4dc7-142">Boolean</span></span>|<span data-ttu-id="a4dc7-143">Определяет, требуется ли проверка identityUserFlowAttribute.</span><span class="sxs-lookup"><span data-stu-id="a4dc7-143">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="a4dc7-144">Он используется только для проверки номера телефона или адреса электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="a4dc7-144">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="a4dc7-145">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="a4dc7-145">userAttributeValues</span></span>|<span data-ttu-id="a4dc7-146">[Коллекция userAttributeValuesItem](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="a4dc7-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="a4dc7-147">Параметры ввода для атрибута пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="a4dc7-147">The input options for the user flow attribute.</span></span> <span data-ttu-id="a4dc7-148">Применимо только в том случае, если userInputType имеет , `radioSingleSelect` `dropdownSingleSelect` или `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="a4dc7-148">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="a4dc7-149">userInputType</span><span class="sxs-lookup"><span data-stu-id="a4dc7-149">userInputType</span></span>|<span data-ttu-id="a4dc7-150">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="a4dc7-150">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="a4dc7-151">Тип ввода атрибута пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="a4dc7-151">The input type of the user flow attribute.</span></span> <span data-ttu-id="a4dc7-152">Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="a4dc7-152">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="a4dc7-153">userAttribute</span><span class="sxs-lookup"><span data-stu-id="a4dc7-153">userAttribute</span></span>|[<span data-ttu-id="a4dc7-154">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="a4dc7-154">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="a4dc7-155">Идентификатор атрибута пользовательского потока, который необходимо включить в назначение пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="a4dc7-155">The identifier for the user flow attribute to include in the user flow assignment.</span></span>

## <a name="response"></a><span data-ttu-id="a4dc7-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4dc7-156">Response</span></span>

<span data-ttu-id="a4dc7-157">В случае успешного выполнения этот метод возвращает код отклика и объект `201 Created` [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a4dc7-157">If successful, this method returns a `201 Created` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4dc7-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="a4dc7-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4dc7-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4dc7-159">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a4dc7-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4dc7-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityuserflowattributeassignment_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments
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
# <a name="c"></a>[<span data-ttu-id="a4dc7-161">C#</span><span class="sxs-lookup"><span data-stu-id="a4dc7-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflowattributeassignment-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4dc7-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4dc7-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflowattributeassignment-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4dc7-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4dc7-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflowattributeassignment-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4dc7-164">Java</span><span class="sxs-lookup"><span data-stu-id="a4dc7-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityuserflowattributeassignment-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a4dc7-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4dc7-165">Response</span></span>

<span data-ttu-id="a4dc7-166">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a4dc7-166">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/extension_guid_shoeSize
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
