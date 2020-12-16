---
title: Обновление identityUserFlowAttributeAssignment
description: Обновление свойств объекта userAttributeAssignments.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2d179602f93ad3e9e44b527364e8cfb1f212c36b
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689236"
---
# <a name="update-identityuserflowattributeassignment"></a><span data-ttu-id="59cf9-103">Обновление identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="59cf9-103">Update identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="59cf9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59cf9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="59cf9-105">Обновление свойств объекта identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="59cf9-105">Update the properties of a identityUserFlowAttributeAssignment object.</span></span>

## <a name="permissions"></a><span data-ttu-id="59cf9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59cf9-106">Permissions</span></span>

<span data-ttu-id="59cf9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59cf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59cf9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59cf9-109">Permission type</span></span>|<span data-ttu-id="59cf9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59cf9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59cf9-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59cf9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="59cf9-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59cf9-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="59cf9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59cf9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59cf9-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="59cf9-114">Not supported</span></span>|
|<span data-ttu-id="59cf9-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="59cf9-115">Application</span></span>|<span data-ttu-id="59cf9-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59cf9-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59cf9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59cf9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
PATCH /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="59cf9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59cf9-118">Request headers</span></span>

|<span data-ttu-id="59cf9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="59cf9-119">Name</span></span>|<span data-ttu-id="59cf9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="59cf9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="59cf9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59cf9-121">Authorization</span></span>|<span data-ttu-id="59cf9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59cf9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="59cf9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="59cf9-124">Content-Type</span></span>|<span data-ttu-id="59cf9-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59cf9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59cf9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59cf9-127">Request body</span></span>

<span data-ttu-id="59cf9-128">В теле запроса укажу представление объекта [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="59cf9-128">In the request body, supply a JSON representation of the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

<span data-ttu-id="59cf9-129">В следующей таблице показаны свойства, доступные для обновления в [identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="59cf9-129">The following table shows the properties that are available to update in the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span></span>

|<span data-ttu-id="59cf9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="59cf9-130">Property</span></span>|<span data-ttu-id="59cf9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="59cf9-131">Type</span></span>|<span data-ttu-id="59cf9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="59cf9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59cf9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="59cf9-133">displayName</span></span>|<span data-ttu-id="59cf9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="59cf9-134">String</span></span>|<span data-ttu-id="59cf9-135">Отображаемого имени identityUserFlowAttribute в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="59cf9-135">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="59cf9-136">isOptional</span><span class="sxs-lookup"><span data-stu-id="59cf9-136">isOptional</span></span>|<span data-ttu-id="59cf9-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="59cf9-137">Boolean</span></span>|<span data-ttu-id="59cf9-138">Определяет, является ли identityUserFlowAttribute необязательным.</span><span class="sxs-lookup"><span data-stu-id="59cf9-138">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="59cf9-139">`true` означает, что пользователю не нужно предоставлять значение.</span><span class="sxs-lookup"><span data-stu-id="59cf9-139">`true` means the user does not have to provide a value.</span></span> <span data-ttu-id="59cf9-140">`false` означает, что пользователь не может зарегистрироваться без предоставления значения.</span><span class="sxs-lookup"><span data-stu-id="59cf9-140">`false` means the user cannot complete sign up without providing a value.</span></span>|
|<span data-ttu-id="59cf9-141">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="59cf9-141">requiresVerification</span></span>|<span data-ttu-id="59cf9-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="59cf9-142">Boolean</span></span>|<span data-ttu-id="59cf9-143">Определяет, требуется ли проверка identityUserFlowAttribute.</span><span class="sxs-lookup"><span data-stu-id="59cf9-143">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="59cf9-144">Он используется только для проверки номера телефона или адреса электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="59cf9-144">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="59cf9-145">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="59cf9-145">userAttributeValues</span></span>|<span data-ttu-id="59cf9-146">[Коллекция userAttributeValuesItem](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="59cf9-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="59cf9-147">Параметры ввода для атрибута пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="59cf9-147">The input options for the user flow attribute.</span></span> <span data-ttu-id="59cf9-148">Применимо только в том случае, если userInputType имеет , `radioSingleSelect` `dropdownSingleSelect` или `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="59cf9-148">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="59cf9-149">userInputType</span><span class="sxs-lookup"><span data-stu-id="59cf9-149">userInputType</span></span>|<span data-ttu-id="59cf9-150">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="59cf9-150">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="59cf9-151">Тип ввода атрибута пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="59cf9-151">The input type of the user flow attribute.</span></span> <span data-ttu-id="59cf9-152">Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="59cf9-152">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="response"></a><span data-ttu-id="59cf9-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="59cf9-153">Response</span></span>

<span data-ttu-id="59cf9-154">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="59cf9-154">If successful, this method returns a `200 OK` response code and an updated [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="59cf9-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="59cf9-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="59cf9-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="59cf9-156">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="59cf9-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="59cf9-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_userattributeassignments"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/{id}
Content-Type: application/json

{
  "userInputType": "textBox"
}
```
# <a name="c"></a>[<span data-ttu-id="59cf9-158">C#</span><span class="sxs-lookup"><span data-stu-id="59cf9-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-userattributeassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59cf9-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59cf9-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-userattributeassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59cf9-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59cf9-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-userattributeassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59cf9-161">Java</span><span class="sxs-lookup"><span data-stu-id="59cf9-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-userattributeassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="59cf9-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="59cf9-162">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
