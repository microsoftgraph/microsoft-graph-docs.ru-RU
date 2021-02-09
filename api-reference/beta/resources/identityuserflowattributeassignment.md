---
title: Тип ресурса identityUserFlowAttributeAssignment
description: identityUserFlowAttributeAssignments используются для сбора определенных identityUserFlowAttributes в пользовательском потоке.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 65859cb0d235454577e236761064f4597f5c68d8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158788"
---
# <a name="identityuserflowattributeassignment-resource-type"></a><span data-ttu-id="b2733-103">Тип ресурса identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="b2733-103">identityUserFlowAttributeAssignment resource type</span></span>

<span data-ttu-id="b2733-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2733-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2733-105">identityUserFlowAttributeAssignments используются для сбора определенных identityUserFlowAttributes в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="b2733-105">identityUserFlowAttributeAssignments are used to collect specific identityUserFlowAttributes within a user flow.</span></span> <span data-ttu-id="b2733-106">Это позволяет управлять атрибутами, собранными в пользовательском потоке, и предоставляет параметры настройки для сбора атрибута в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="b2733-106">This allows control over the attributes that are collected within a user flow, and provides customization options on how to collect the attribute within the user flow.</span></span> <span data-ttu-id="b2733-107">В одном пользовательском потоке может быть несколько удостоверенийUserFlowAttributeAssignment, что создает интерфейс, который видит конечный пользователь во время регистрации при запросе на предоставление сведений, необходимых пользовательскому потоку для завершения регистрации.</span><span class="sxs-lookup"><span data-stu-id="b2733-107">You can have multiple identityUserFlowAttributeAssignments within a single user flow that creates the experience the end user sees during sign-up when asked to provide the information required by the user flow to complete sign-up.</span></span>

## <a name="methods"></a><span data-ttu-id="b2733-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b2733-108">Methods</span></span>

|<span data-ttu-id="b2733-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b2733-109">Method</span></span>|<span data-ttu-id="b2733-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="b2733-110">Return type</span></span>|<span data-ttu-id="b2733-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b2733-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b2733-112">Get identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="b2733-112">Get identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-get.md)|[<span data-ttu-id="b2733-113">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="b2733-113">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="b2733-114">Чтение свойств и связей объекта identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="b2733-114">Read the properties and relationships of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="b2733-115">Обновление identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="b2733-115">Update identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-update.md)|<span data-ttu-id="b2733-116">Нет</span><span class="sxs-lookup"><span data-stu-id="b2733-116">None</span></span>|<span data-ttu-id="b2733-117">Обновление свойств объекта identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="b2733-117">Update the properties of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="b2733-118">Удаление identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="b2733-118">Delete identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-delete.md)|<span data-ttu-id="b2733-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b2733-119">None</span></span>|<span data-ttu-id="b2733-120">Удаление определенного объекта identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="b2733-120">Delete a specific identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="b2733-121">getOrder</span><span class="sxs-lookup"><span data-stu-id="b2733-121">getOrder</span></span>](../api/identityuserflowattributeassignment-getorder.md)|[<span data-ttu-id="b2733-122">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="b2733-122">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="b2733-123">Получает порядок identityUserFlowAttributes, собираемого в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="b2733-123">Gets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|
|[<span data-ttu-id="b2733-124">setOrder</span><span class="sxs-lookup"><span data-stu-id="b2733-124">setOrder</span></span>](../api/identityuserflowattributeassignment-setorder.md)|<span data-ttu-id="b2733-125">Нет</span><span class="sxs-lookup"><span data-stu-id="b2733-125">None</span></span>|<span data-ttu-id="b2733-126">Задает порядок identityUserFlowAttributes, собираемого в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="b2733-126">Sets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="b2733-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2733-127">Properties</span></span>

|<span data-ttu-id="b2733-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2733-128">Property</span></span>|<span data-ttu-id="b2733-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b2733-129">Type</span></span>|<span data-ttu-id="b2733-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b2733-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2733-131">id</span><span class="sxs-lookup"><span data-stu-id="b2733-131">id</span></span>|<span data-ttu-id="b2733-132">String</span><span class="sxs-lookup"><span data-stu-id="b2733-132">String</span></span>|<span data-ttu-id="b2733-133">Идентификатор identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="b2733-133">The identifier of the identityUserFlowAttributeAssignment.</span></span> <span data-ttu-id="b2733-134">Этот идентификатор не может быть неуявяем после его создания.</span><span class="sxs-lookup"><span data-stu-id="b2733-134">This identifier is immutable after it is created.</span></span> <span data-ttu-id="b2733-135">Это свойство только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2733-135">This is a read-only property.</span></span>|
|<span data-ttu-id="b2733-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b2733-136">displayName</span></span>|<span data-ttu-id="b2733-137">String</span><span class="sxs-lookup"><span data-stu-id="b2733-137">String</span></span>|<span data-ttu-id="b2733-138">Отображаемого имени identityUserFlowAttribute в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="b2733-138">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="b2733-139">isOptional</span><span class="sxs-lookup"><span data-stu-id="b2733-139">isOptional</span></span>|<span data-ttu-id="b2733-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2733-140">Boolean</span></span>|<span data-ttu-id="b2733-141">Определяет, является ли identityUserFlowAttribute необязательным.</span><span class="sxs-lookup"><span data-stu-id="b2733-141">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="b2733-142">`true` означает, что пользователю не нужно предоставлять значение.</span><span class="sxs-lookup"><span data-stu-id="b2733-142">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="b2733-143">`false` означает, что пользователь не может завершить регистрацию без предоставления значения.</span><span class="sxs-lookup"><span data-stu-id="b2733-143">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="b2733-144">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="b2733-144">requiresVerification</span></span>|<span data-ttu-id="b2733-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2733-145">Boolean</span></span>|<span data-ttu-id="b2733-146">Определяет, требуется ли проверка identityUserFlowAttribute.</span><span class="sxs-lookup"><span data-stu-id="b2733-146">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="b2733-147">Он используется только для проверки номера телефона или адреса электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="b2733-147">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="b2733-148">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="b2733-148">userAttributeValues</span></span>|<span data-ttu-id="b2733-149">[Коллекция userAttributeValuesItem](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="b2733-149">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="b2733-150">Параметры ввода для атрибута пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="b2733-150">The input options for the user flow attribute.</span></span> <span data-ttu-id="b2733-151">Применимо только в том случае, если userInputType имеет , `radioSingleSelect` `dropdownSingleSelect` или `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="b2733-151">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="b2733-152">userInputType</span><span class="sxs-lookup"><span data-stu-id="b2733-152">userInputType</span></span>|<span data-ttu-id="b2733-153">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="b2733-153">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="b2733-154">Тип ввода атрибута пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="b2733-154">The input type of the user flow attribute.</span></span> <span data-ttu-id="b2733-155">Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="b2733-155">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2733-156">Связи</span><span class="sxs-lookup"><span data-stu-id="b2733-156">Relationships</span></span>

|<span data-ttu-id="b2733-157">Связь</span><span class="sxs-lookup"><span data-stu-id="b2733-157">Relationship</span></span>|<span data-ttu-id="b2733-158">Тип</span><span class="sxs-lookup"><span data-stu-id="b2733-158">Type</span></span>|<span data-ttu-id="b2733-159">Описание</span><span class="sxs-lookup"><span data-stu-id="b2733-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2733-160">userAttribute</span><span class="sxs-lookup"><span data-stu-id="b2733-160">userAttribute</span></span>|[<span data-ttu-id="b2733-161">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="b2733-161">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="b2733-162">Атрибут пользователя, который вы хотите добавить в пользовательский поток.</span><span class="sxs-lookup"><span data-stu-id="b2733-162">The user attribute that you want to add to your user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2733-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2733-163">JSON representation</span></span>

<span data-ttu-id="b2733-164">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2733-164">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
  "id": "String (identifier)",
  "isOptional": "Boolean",
  "requiresVerification": "Boolean",
  "userInputType": "String",
  "userAttributeValues": [
    {
      "@odata.type": "microsoft.graph.userAttributeValuesItem"
    }
  ],
  "displayName": "String"
}
```
