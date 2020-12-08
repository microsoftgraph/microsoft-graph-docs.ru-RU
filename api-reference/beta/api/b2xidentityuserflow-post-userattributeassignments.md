---
title: Создание Усераттрибутеассигнментс
description: Создание нового объекта Идентитюсерфловаттрибутеассигнмент в b2xIdentityUserFlow.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fd4f2e7f98359d49239b6a9602f06e1fc51d1749
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581344"
---
# <a name="create-userattributeassignments"></a><span data-ttu-id="a470a-103">Создание Усераттрибутеассигнментс</span><span class="sxs-lookup"><span data-stu-id="a470a-103">Create userAttributeAssignments</span></span>

<span data-ttu-id="a470a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a470a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a470a-105">Создание нового объекта Идентитюсерфловаттрибутеассигнмент в [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="a470a-105">Create a new identityUserFlowAttributeAssignment object in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a470a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a470a-106">Permissions</span></span>

<span data-ttu-id="a470a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a470a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a470a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a470a-109">Permission type</span></span>|<span data-ttu-id="a470a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a470a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a470a-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a470a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a470a-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a470a-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="a470a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a470a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a470a-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a470a-114">Not supported</span></span>|
|<span data-ttu-id="a470a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a470a-115">Application</span></span>|<span data-ttu-id="a470a-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a470a-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a470a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a470a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/b2xUserFlows/{id}/userAttributeAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a470a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a470a-118">Request headers</span></span>

|<span data-ttu-id="a470a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a470a-119">Name</span></span>|<span data-ttu-id="a470a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a470a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a470a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a470a-121">Authorization</span></span>|<span data-ttu-id="a470a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a470a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a470a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a470a-124">Content-Type</span></span>|<span data-ttu-id="a470a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a470a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a470a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a470a-127">Request body</span></span>

<span data-ttu-id="a470a-128">В тексте запроса добавьте представление объекта [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a470a-128">In the request body, supply a JSON representation of the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

<span data-ttu-id="a470a-129">В следующей таблице приведены свойства, необходимые при создании [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a470a-129">The following table shows the properties that are required when you create the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span></span>

|<span data-ttu-id="a470a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a470a-130">Property</span></span>|<span data-ttu-id="a470a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a470a-131">Type</span></span>|<span data-ttu-id="a470a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a470a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a470a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="a470a-133">displayName</span></span>|<span data-ttu-id="a470a-134">String</span><span class="sxs-lookup"><span data-stu-id="a470a-134">String</span></span>|<span data-ttu-id="a470a-135">Отображаемое имя Идентитюсерфловаттрибуте в пользовательском движении.</span><span class="sxs-lookup"><span data-stu-id="a470a-135">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="a470a-136">Переключатель</span><span class="sxs-lookup"><span data-stu-id="a470a-136">isOptional</span></span>|<span data-ttu-id="a470a-137">Логический</span><span class="sxs-lookup"><span data-stu-id="a470a-137">Boolean</span></span>|<span data-ttu-id="a470a-138">Определяет, является ли Идентитюсерфловаттрибуте необязательным.</span><span class="sxs-lookup"><span data-stu-id="a470a-138">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="a470a-139">`true` означает, что пользователю не нужно указывать значение.</span><span class="sxs-lookup"><span data-stu-id="a470a-139">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="a470a-140">`false` означает, что пользователь не может выполнить вход, не указывая значение.</span><span class="sxs-lookup"><span data-stu-id="a470a-140">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="a470a-141">рекуиресверификатион</span><span class="sxs-lookup"><span data-stu-id="a470a-141">requiresVerification</span></span>|<span data-ttu-id="a470a-142">Логический</span><span class="sxs-lookup"><span data-stu-id="a470a-142">Boolean</span></span>|<span data-ttu-id="a470a-143">Определяет, требуется ли для Идентитюсерфловаттрибуте проверка.</span><span class="sxs-lookup"><span data-stu-id="a470a-143">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="a470a-144">Используется только для проверки номера телефона пользователя или адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a470a-144">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="a470a-145">усераттрибутевалуес</span><span class="sxs-lookup"><span data-stu-id="a470a-145">userAttributeValues</span></span>|<span data-ttu-id="a470a-146">Коллекция [усераттрибутевалуеситем](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="a470a-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="a470a-147">Параметры ввода для атрибута Flow User.</span><span class="sxs-lookup"><span data-stu-id="a470a-147">The input options for the user flow attribute.</span></span> <span data-ttu-id="a470a-148">Применяется только в том случае, если для Усеринпуттипе задано значение `radioSingleSelect` , `dropdownSingleSelect` или `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="a470a-148">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="a470a-149">усеринпуттипе</span><span class="sxs-lookup"><span data-stu-id="a470a-149">userInputType</span></span>|<span data-ttu-id="a470a-150">идентитюсерфловаттрибутеинпуттипе</span><span class="sxs-lookup"><span data-stu-id="a470a-150">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="a470a-151">Тип входных данных для атрибута Flow User.</span><span class="sxs-lookup"><span data-stu-id="a470a-151">The input type of the user flow attribute.</span></span> <span data-ttu-id="a470a-152">Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="a470a-152">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="a470a-153">усераттрибуте</span><span class="sxs-lookup"><span data-stu-id="a470a-153">userAttribute</span></span>|[<span data-ttu-id="a470a-154">идентитюсерфловаттрибуте</span><span class="sxs-lookup"><span data-stu-id="a470a-154">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="a470a-155">Идентификатор атрибута пользовательского процесса, включаемый в назначение пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="a470a-155">The identifier for the user flow attribute to include in the user flow assignment.</span></span>

## <a name="response"></a><span data-ttu-id="a470a-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="a470a-156">Response</span></span>

<span data-ttu-id="a470a-157">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a470a-157">If successful, this method returns a `201 Created` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a470a-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="a470a-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a470a-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="a470a-159">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="a470a-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="a470a-160">Response</span></span>

<span data-ttu-id="a470a-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a470a-161">**Note:** The response object shown here might be shortened for readability.</span></span>
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
