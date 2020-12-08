---
title: Обновление Идентитюсерфловаттрибутеассигнмент
description: Обновление свойств объекта Усераттрибутеассигнментс.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2b9b5e39cd8d7462b678608ae74727eacdf101cb
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581423"
---
# <a name="update-identityuserflowattributeassignment"></a><span data-ttu-id="73cf7-103">Обновление Идентитюсерфловаттрибутеассигнмент</span><span class="sxs-lookup"><span data-stu-id="73cf7-103">Update identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="73cf7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73cf7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73cf7-105">Обновление свойств объекта Идентитюсерфловаттрибутеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="73cf7-105">Update the properties of a identityUserFlowAttributeAssignment object.</span></span>

## <a name="permissions"></a><span data-ttu-id="73cf7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73cf7-106">Permissions</span></span>

<span data-ttu-id="73cf7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73cf7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73cf7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73cf7-109">Permission type</span></span>|<span data-ttu-id="73cf7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73cf7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73cf7-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73cf7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="73cf7-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="73cf7-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="73cf7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73cf7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73cf7-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="73cf7-114">Not supported</span></span>|
|<span data-ttu-id="73cf7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="73cf7-115">Application</span></span>|<span data-ttu-id="73cf7-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="73cf7-116">IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73cf7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73cf7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
PATCH /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="73cf7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73cf7-118">Request headers</span></span>

|<span data-ttu-id="73cf7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="73cf7-119">Name</span></span>|<span data-ttu-id="73cf7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="73cf7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="73cf7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73cf7-121">Authorization</span></span>|<span data-ttu-id="73cf7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73cf7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="73cf7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73cf7-124">Content-Type</span></span>|<span data-ttu-id="73cf7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73cf7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73cf7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73cf7-127">Request body</span></span>

<span data-ttu-id="73cf7-128">В тексте запроса добавьте представление объекта [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73cf7-128">In the request body, supply a JSON representation of the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

<span data-ttu-id="73cf7-129">В следующей таблице приведены свойства, доступные для обновления в [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md).</span><span class="sxs-lookup"><span data-stu-id="73cf7-129">The following table shows the properties that are available to update in the [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md).</span></span>

|<span data-ttu-id="73cf7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="73cf7-130">Property</span></span>|<span data-ttu-id="73cf7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="73cf7-131">Type</span></span>|<span data-ttu-id="73cf7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="73cf7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73cf7-133">displayName</span><span class="sxs-lookup"><span data-stu-id="73cf7-133">displayName</span></span>|<span data-ttu-id="73cf7-134">String</span><span class="sxs-lookup"><span data-stu-id="73cf7-134">String</span></span>|<span data-ttu-id="73cf7-135">Отображаемое имя Идентитюсерфловаттрибуте в пользовательском движении.</span><span class="sxs-lookup"><span data-stu-id="73cf7-135">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="73cf7-136">Переключатель</span><span class="sxs-lookup"><span data-stu-id="73cf7-136">isOptional</span></span>|<span data-ttu-id="73cf7-137">Логический</span><span class="sxs-lookup"><span data-stu-id="73cf7-137">Boolean</span></span>|<span data-ttu-id="73cf7-138">Определяет, является ли Идентитюсерфловаттрибуте необязательным.</span><span class="sxs-lookup"><span data-stu-id="73cf7-138">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="73cf7-139">`true` означает, что пользователю не нужно указывать значение.</span><span class="sxs-lookup"><span data-stu-id="73cf7-139">`true` means the user does not have to provide a value.</span></span> <span data-ttu-id="73cf7-140">`false` Указывает, что пользователь не может выполнить вход, не предоставляя значение.</span><span class="sxs-lookup"><span data-stu-id="73cf7-140">`false` means the user cannot complete sign up without providing a value.</span></span>|
|<span data-ttu-id="73cf7-141">рекуиресверификатион</span><span class="sxs-lookup"><span data-stu-id="73cf7-141">requiresVerification</span></span>|<span data-ttu-id="73cf7-142">Логический</span><span class="sxs-lookup"><span data-stu-id="73cf7-142">Boolean</span></span>|<span data-ttu-id="73cf7-143">Определяет, требуется ли для Идентитюсерфловаттрибуте проверка.</span><span class="sxs-lookup"><span data-stu-id="73cf7-143">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="73cf7-144">Используется только для проверки номера телефона пользователя или адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="73cf7-144">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="73cf7-145">усераттрибутевалуес</span><span class="sxs-lookup"><span data-stu-id="73cf7-145">userAttributeValues</span></span>|<span data-ttu-id="73cf7-146">Коллекция [усераттрибутевалуеситем](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="73cf7-146">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="73cf7-147">Параметры ввода для атрибута Flow User.</span><span class="sxs-lookup"><span data-stu-id="73cf7-147">The input options for the user flow attribute.</span></span> <span data-ttu-id="73cf7-148">Применяется только в том случае, если для Усеринпуттипе задано значение `radioSingleSelect` , `dropdownSingleSelect` или `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="73cf7-148">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="73cf7-149">усеринпуттипе</span><span class="sxs-lookup"><span data-stu-id="73cf7-149">userInputType</span></span>|<span data-ttu-id="73cf7-150">идентитюсерфловаттрибутеинпуттипе</span><span class="sxs-lookup"><span data-stu-id="73cf7-150">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="73cf7-151">Тип входных данных для атрибута Flow User.</span><span class="sxs-lookup"><span data-stu-id="73cf7-151">The input type of the user flow attribute.</span></span> <span data-ttu-id="73cf7-152">Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="73cf7-152">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="response"></a><span data-ttu-id="73cf7-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="73cf7-153">Response</span></span>

<span data-ttu-id="73cf7-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73cf7-154">If successful, this method returns a `200 OK` response code and an updated [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73cf7-155">Примеры</span><span class="sxs-lookup"><span data-stu-id="73cf7-155">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73cf7-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="73cf7-156">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="73cf7-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="73cf7-157">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
