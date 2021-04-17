---
title: тип ресурса identityUserFlowAttributeAssignment
description: Представляет, как атрибуты собираются в потоке пользователей удостоверений.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0df6309682158e3d4890c6549bc7aeebb710254c
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883110"
---
# <a name="identityuserflowattributeassignment-resource-type"></a><span data-ttu-id="12f14-103">тип ресурса identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="12f14-103">identityUserFlowAttributeAssignment resource type</span></span>

<span data-ttu-id="12f14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12f14-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12f14-105">Представляет, как атрибуты собираются в потоке пользователей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="12f14-105">Represents how attributes are collected in an identity user flow.</span></span> <span data-ttu-id="12f14-106">Это позволяет настраивать параметры для сбора атрибутов в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="12f14-106">This allows customization options for collecting attributes within the user flow.</span></span> <span data-ttu-id="12f14-107">Вы можете иметь несколько удостоверенийUserFlowAttributeAssignments в одном потоке пользователей, что создает возможность предоставления сведений, необходимых пользователю для завершения регистрации.</span><span class="sxs-lookup"><span data-stu-id="12f14-107">You can have multiple identityUserFlowAttributeAssignments within a single user flow that creates the experience for providing the information required by the user to complete sign-up.</span></span>

## <a name="methods"></a><span data-ttu-id="12f14-108">Методы</span><span class="sxs-lookup"><span data-stu-id="12f14-108">Methods</span></span>

|<span data-ttu-id="12f14-109">Метод</span><span class="sxs-lookup"><span data-stu-id="12f14-109">Method</span></span>|<span data-ttu-id="12f14-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="12f14-110">Return type</span></span>|<span data-ttu-id="12f14-111">Описание</span><span class="sxs-lookup"><span data-stu-id="12f14-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="12f14-112">Get identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="12f14-112">Get identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-get.md)|[<span data-ttu-id="12f14-113">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="12f14-113">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="12f14-114">Ознакомьтесь с свойствами и отношениями объекта identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="12f14-114">Read the properties and relationships of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="12f14-115">Обновление identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="12f14-115">Update identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-update.md)|<span data-ttu-id="12f14-116">Нет</span><span class="sxs-lookup"><span data-stu-id="12f14-116">None</span></span>|<span data-ttu-id="12f14-117">Обновление свойств объекта identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="12f14-117">Update the properties of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="12f14-118">Удаление identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="12f14-118">Delete identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-delete.md)|<span data-ttu-id="12f14-119">Нет</span><span class="sxs-lookup"><span data-stu-id="12f14-119">None</span></span>|<span data-ttu-id="12f14-120">Удаление определенного объекта identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="12f14-120">Delete a specific identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="12f14-121">getOrder</span><span class="sxs-lookup"><span data-stu-id="12f14-121">getOrder</span></span>](../api/identityuserflowattributeassignment-getorder.md)|[<span data-ttu-id="12f14-122">assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="12f14-122">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="12f14-123">Получает порядок сбора identityUserFlowAttributes в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="12f14-123">Gets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|
|[<span data-ttu-id="12f14-124">setOrder</span><span class="sxs-lookup"><span data-stu-id="12f14-124">setOrder</span></span>](../api/identityuserflowattributeassignment-setorder.md)|<span data-ttu-id="12f14-125">Нет</span><span class="sxs-lookup"><span data-stu-id="12f14-125">None</span></span>|<span data-ttu-id="12f14-126">Задает порядок сбора identityUserFlowAttributes в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="12f14-126">Sets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="12f14-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="12f14-127">Properties</span></span>

|<span data-ttu-id="12f14-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="12f14-128">Property</span></span>|<span data-ttu-id="12f14-129">Тип</span><span class="sxs-lookup"><span data-stu-id="12f14-129">Type</span></span>|<span data-ttu-id="12f14-130">Описание</span><span class="sxs-lookup"><span data-stu-id="12f14-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12f14-131">id</span><span class="sxs-lookup"><span data-stu-id="12f14-131">id</span></span>|<span data-ttu-id="12f14-132">Строка</span><span class="sxs-lookup"><span data-stu-id="12f14-132">String</span></span>|<span data-ttu-id="12f14-133">Идентификатор identityUserFlowAttributeAssignment.</span><span class="sxs-lookup"><span data-stu-id="12f14-133">The identifier of the identityUserFlowAttributeAssignment.</span></span> <span data-ttu-id="12f14-134">Этот идентификатор неуменяем после создания.</span><span class="sxs-lookup"><span data-stu-id="12f14-134">This identifier is immutable after it is created.</span></span> <span data-ttu-id="12f14-135">Это свойство только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12f14-135">This is a read-only property.</span></span>|
|<span data-ttu-id="12f14-136">displayName</span><span class="sxs-lookup"><span data-stu-id="12f14-136">displayName</span></span>|<span data-ttu-id="12f14-137">Строка</span><span class="sxs-lookup"><span data-stu-id="12f14-137">String</span></span>|<span data-ttu-id="12f14-138">Отображение имени identityUserFlowAttribute в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="12f14-138">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="12f14-139">isOptional</span><span class="sxs-lookup"><span data-stu-id="12f14-139">isOptional</span></span>|<span data-ttu-id="12f14-140">Логическое</span><span class="sxs-lookup"><span data-stu-id="12f14-140">Boolean</span></span>|<span data-ttu-id="12f14-141">Определяет, является ли identityUserFlowAttribute необязательным.</span><span class="sxs-lookup"><span data-stu-id="12f14-141">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="12f14-142">`true` означает, что пользователю не нужно предоставлять значение.</span><span class="sxs-lookup"><span data-stu-id="12f14-142">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="12f14-143">`false` означает, что пользователь не может завершить регистрацию без предоставления значения.</span><span class="sxs-lookup"><span data-stu-id="12f14-143">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="12f14-144">requiresVerification</span><span class="sxs-lookup"><span data-stu-id="12f14-144">requiresVerification</span></span>|<span data-ttu-id="12f14-145">Логическое</span><span class="sxs-lookup"><span data-stu-id="12f14-145">Boolean</span></span>|<span data-ttu-id="12f14-146">Определяет, требуется ли проверка identityUserFlowAttribute.</span><span class="sxs-lookup"><span data-stu-id="12f14-146">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="12f14-147">Это используется только для проверки номера телефона или адреса электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="12f14-147">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="12f14-148">userAttributeValues</span><span class="sxs-lookup"><span data-stu-id="12f14-148">userAttributeValues</span></span>|<span data-ttu-id="12f14-149">[коллекция userAttributeValuesItem](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="12f14-149">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="12f14-150">Параметры ввода атрибута потока пользователя.</span><span class="sxs-lookup"><span data-stu-id="12f14-150">The input options for the user flow attribute.</span></span> <span data-ttu-id="12f14-151">Применимо только в том случае, если userInputType `radioSingleSelect` является `dropdownSingleSelect` , или `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="12f14-151">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="12f14-152">userInputType</span><span class="sxs-lookup"><span data-stu-id="12f14-152">userInputType</span></span>|<span data-ttu-id="12f14-153">identityUserFlowAttributeInputType</span><span class="sxs-lookup"><span data-stu-id="12f14-153">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="12f14-154">Тип ввода атрибута потока пользователя.</span><span class="sxs-lookup"><span data-stu-id="12f14-154">The input type of the user flow attribute.</span></span> <span data-ttu-id="12f14-155">Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="12f14-155">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12f14-156">Связи</span><span class="sxs-lookup"><span data-stu-id="12f14-156">Relationships</span></span>

|<span data-ttu-id="12f14-157">Связь</span><span class="sxs-lookup"><span data-stu-id="12f14-157">Relationship</span></span>|<span data-ttu-id="12f14-158">Тип</span><span class="sxs-lookup"><span data-stu-id="12f14-158">Type</span></span>|<span data-ttu-id="12f14-159">Описание</span><span class="sxs-lookup"><span data-stu-id="12f14-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12f14-160">userAttribute</span><span class="sxs-lookup"><span data-stu-id="12f14-160">userAttribute</span></span>|[<span data-ttu-id="12f14-161">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="12f14-161">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="12f14-162">Атрибут пользователя, который необходимо добавить в поток пользователей.</span><span class="sxs-lookup"><span data-stu-id="12f14-162">The user attribute that you want to add to your user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12f14-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12f14-163">JSON representation</span></span>

<span data-ttu-id="12f14-164">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12f14-164">The following is a JSON representation of the resource.</span></span>
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
