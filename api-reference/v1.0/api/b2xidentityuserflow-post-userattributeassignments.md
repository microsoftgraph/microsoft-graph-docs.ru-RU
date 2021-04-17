---
title: Создание userAttributeAssignments
description: Создайте новый объект identityUserFlowAttributeAssignment в b2xIdentityUserFlow.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8daa8a13baa6e08ebfdc666d2f783fbacb82645a
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883122"
---
# <a name="create-userattributeassignments"></a><span data-ttu-id="9feaa-103">Создание userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="9feaa-103">Create userAttributeAssignments</span></span>

<span data-ttu-id="9feaa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9feaa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9feaa-105">Создайте новый объект identityUserFlowAttributeAssignment в [b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="9feaa-105">Create a new identityUserFlowAttributeAssignment object in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9feaa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9feaa-106">Permissions</span></span>

<span data-ttu-id="9feaa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9feaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9feaa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9feaa-109">Permission type</span></span>|<span data-ttu-id="9feaa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9feaa-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9feaa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9feaa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9feaa-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9feaa-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="9feaa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9feaa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9feaa-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9feaa-114">Not supported</span></span>|
|<span data-ttu-id="9feaa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9feaa-115">Application</span></span>|<span data-ttu-id="9feaa-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9feaa-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9feaa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9feaa-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2xUserFlows/{id}/userAttributeAssignments
```

## <a name="request-headers"></a><span data-ttu-id="9feaa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9feaa-118">Request headers</span></span>

|<span data-ttu-id="9feaa-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9feaa-119">Name</span></span>|<span data-ttu-id="9feaa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9feaa-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9feaa-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9feaa-121">Authorization</span></span>|<span data-ttu-id="9feaa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9feaa-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9feaa-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9feaa-124">Content-Type</span></span>|<span data-ttu-id="9feaa-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9feaa-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9feaa-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9feaa-127">Request body</span></span>

<span data-ttu-id="9feaa-128">В теле запроса подарят представление JSON объекта [identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9feaa-128">In the request body, supply a JSON representation of the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

<span data-ttu-id="9feaa-129">В следующей таблице показаны свойства, необходимые при создании [identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9feaa-129">The following table shows the properties that are required when you create the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span></span>

|<span data-ttu-id="9feaa-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9feaa-130">Property</span></span>|<span data-ttu-id="9feaa-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9feaa-131">Type</span></span>|<span data-ttu-id="9feaa-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9feaa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9feaa-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9feaa-133">displayName</span></span>|<span data-ttu-id="9feaa-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9feaa-134">String</span></span>|<span data-ttu-id="9feaa-135">Отображение имени identityUserFlowAttribute в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="9feaa-135">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="9feaa-136">isOptional</span><span class="sxs-lookup"><span data-stu-id="9feaa-136">isOptional</span></span>|<span data-ttu-id="9feaa-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="9feaa-137">Boolean</span></span>|<span data-ttu-id="9feaa-138">Определяет, является ли identityUserFlowAttribute необязательным.</span><span class="sxs-lookup"><span data-stu-id="9feaa-138">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="9feaa-139">`true` означает, что пользователю не нужно предоставлять значение.</span><span class="sxs-lookup"><span data-stu-id="9feaa-139">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="9feaa-140">`false` означает, что пользователь не может завершить регистрацию без предоставления значения.</span><span class="sxs-lookup"><span data-stu-id="9feaa-140">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="9feaa-141">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="9feaa-141">requiresVerification</span></span>|<span data-ttu-id="9feaa-142">Логическое</span><span class="sxs-lookup"><span data-stu-id="9feaa-142">Boolean</span></span>|<span data-ttu-id="9feaa-143">Определяет, требуется ли проверка identityUserFlowAttribute.</span><span class="sxs-lookup"><span data-stu-id="9feaa-143">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="9feaa-144">Это используется только для проверки номера телефона или адреса электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="9feaa-144">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="9feaa-145">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="9feaa-145">userAttributeValues</span></span>|<span data-ttu-id="9feaa-146">[коллекция userAttributeValuesItem](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="9feaa-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="9feaa-147">Параметры ввода атрибута потока пользователя.</span><span class="sxs-lookup"><span data-stu-id="9feaa-147">The input options for the user flow attribute.</span></span> <span data-ttu-id="9feaa-148">Применимо только в том случае, если userInputType `radioSingleSelect` является `dropdownSingleSelect` , или `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="9feaa-148">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="9feaa-149">userInputType</span><span class="sxs-lookup"><span data-stu-id="9feaa-149">userInputType</span></span>|<span data-ttu-id="9feaa-150">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="9feaa-150">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="9feaa-151">Тип ввода атрибута потока пользователя.</span><span class="sxs-lookup"><span data-stu-id="9feaa-151">The input type of the user flow attribute.</span></span> <span data-ttu-id="9feaa-152">Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="9feaa-152">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="9feaa-153">userAttribute</span><span class="sxs-lookup"><span data-stu-id="9feaa-153">userAttribute</span></span>|[<span data-ttu-id="9feaa-154">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="9feaa-154">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="9feaa-155">Идентификатор атрибута потока пользователей, который должен включаться в назначение потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="9feaa-155">The identifier for the user flow attribute to include in the user flow assignment.</span></span>

## <a name="response"></a><span data-ttu-id="9feaa-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="9feaa-156">Response</span></span>

<span data-ttu-id="9feaa-157">В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9feaa-157">If successful, this method returns a `201 Created` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9feaa-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="9feaa-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9feaa-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="9feaa-159">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityuserflowattributeassignment_from__2"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments
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

### <a name="response"></a><span data-ttu-id="9feaa-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="9feaa-160">Response</span></span>

<span data-ttu-id="9feaa-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9feaa-161">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/extension_guid_shoeSize
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
