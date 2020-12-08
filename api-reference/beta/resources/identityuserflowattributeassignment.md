---
title: Тип ресурса Идентитюсерфловаттрибутеассигнмент
description: Идентитюсерфловаттрибутеассигнментс используются для сбора определенных Идентитюсерфловаттрибутес в рамках пользовательского процесса.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 80bc6547307914e0d206ea9b5c79073f96fce19c
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581345"
---
# <a name="identityuserflowattributeassignment-resource-type"></a><span data-ttu-id="17158-103">Тип ресурса Идентитюсерфловаттрибутеассигнмент</span><span class="sxs-lookup"><span data-stu-id="17158-103">identityUserFlowAttributeAssignment resource type</span></span>

<span data-ttu-id="17158-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17158-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="17158-105">Идентитюсерфловаттрибутеассигнментс используются для сбора определенных Идентитюсерфловаттрибутес в рамках пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="17158-105">identityUserFlowAttributeAssignments are used to collect specific identityUserFlowAttributes within a user flow.</span></span> <span data-ttu-id="17158-106">Это позволяет управлять атрибутами, собранными в пользовательском цикле, и предоставляет варианты настройки для сбора атрибута в пределах пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="17158-106">This allows control over the attributes that are collected within a user flow, and provides customization options on how to collect the attribute within the user flow.</span></span> <span data-ttu-id="17158-107">Вы можете использовать несколько Идентитюсерфловаттрибутеассигнментс в одном потоке пользователей, который создает интерфейс, который видит конечный пользователь во время регистрации, когда вам будет предложено предоставить сведения, необходимые для входа пользователя в систему.</span><span class="sxs-lookup"><span data-stu-id="17158-107">You can have multiple identityUserFlowAttributeAssignments within a single user flow that creates the experience the end user sees during sign-up when asked to provide the information required by the user flow to complete sign-up.</span></span>

## <a name="methods"></a><span data-ttu-id="17158-108">Методы</span><span class="sxs-lookup"><span data-stu-id="17158-108">Methods</span></span>

|<span data-ttu-id="17158-109">Метод</span><span class="sxs-lookup"><span data-stu-id="17158-109">Method</span></span>|<span data-ttu-id="17158-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="17158-110">Return type</span></span>|<span data-ttu-id="17158-111">Описание</span><span class="sxs-lookup"><span data-stu-id="17158-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="17158-112">Получение Идентитюсерфловаттрибутеассигнмент</span><span class="sxs-lookup"><span data-stu-id="17158-112">Get identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-get.md)|[<span data-ttu-id="17158-113">идентитюсерфловаттрибутеассигнмент</span><span class="sxs-lookup"><span data-stu-id="17158-113">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="17158-114">Чтение свойств и связей объекта Идентитюсерфловаттрибутеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="17158-114">Read the properties and relationships of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="17158-115">Обновление Идентитюсерфловаттрибутеассигнмент</span><span class="sxs-lookup"><span data-stu-id="17158-115">Update identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-update.md)|<span data-ttu-id="17158-116">Нет</span><span class="sxs-lookup"><span data-stu-id="17158-116">None</span></span>|<span data-ttu-id="17158-117">Обновление свойств объекта Идентитюсерфловаттрибутеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="17158-117">Update the properties of an identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="17158-118">Удаление Идентитюсерфловаттрибутеассигнмент</span><span class="sxs-lookup"><span data-stu-id="17158-118">Delete identityUserFlowAttributeAssignment</span></span>](../api/identityuserflowattributeassignment-delete.md)|<span data-ttu-id="17158-119">Нет</span><span class="sxs-lookup"><span data-stu-id="17158-119">None</span></span>|<span data-ttu-id="17158-120">Удаление определенного объекта Идентитюсерфловаттрибутеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="17158-120">Delete a specific identityUserFlowAttributeAssignment object.</span></span>|
|[<span data-ttu-id="17158-121">по убыванию</span><span class="sxs-lookup"><span data-stu-id="17158-121">getOrder</span></span>](../api/identityuserflowattributeassignment-getorder.md)|[<span data-ttu-id="17158-122">ассигнментордер</span><span class="sxs-lookup"><span data-stu-id="17158-122">assignmentOrder</span></span>](../resources/assignmentorder.md)|<span data-ttu-id="17158-123">Получает порядок Идентитюсерфловаттрибутес, собранных в пользовательском движении.</span><span class="sxs-lookup"><span data-stu-id="17158-123">Gets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|
|[<span data-ttu-id="17158-124">сетордер</span><span class="sxs-lookup"><span data-stu-id="17158-124">setOrder</span></span>](../api/identityuserflowattributeassignment-setorder.md)|<span data-ttu-id="17158-125">Нет</span><span class="sxs-lookup"><span data-stu-id="17158-125">None</span></span>|<span data-ttu-id="17158-126">Задает порядок Идентитюсерфловаттрибутес, собранных в пользовательском движении.</span><span class="sxs-lookup"><span data-stu-id="17158-126">Sets the order of the identityUserFlowAttributes being collected within a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="17158-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="17158-127">Properties</span></span>

|<span data-ttu-id="17158-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="17158-128">Property</span></span>|<span data-ttu-id="17158-129">Тип</span><span class="sxs-lookup"><span data-stu-id="17158-129">Type</span></span>|<span data-ttu-id="17158-130">Описание</span><span class="sxs-lookup"><span data-stu-id="17158-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17158-131">id</span><span class="sxs-lookup"><span data-stu-id="17158-131">id</span></span>|<span data-ttu-id="17158-132">String</span><span class="sxs-lookup"><span data-stu-id="17158-132">String</span></span>|<span data-ttu-id="17158-133">Идентификатор Идентитюсерфловаттрибутеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="17158-133">The identifier of the identityUserFlowAttributeAssignment.</span></span> <span data-ttu-id="17158-134">Этот идентификатор становится неизменяемым после его создания.</span><span class="sxs-lookup"><span data-stu-id="17158-134">This identifier is immutable after it is created.</span></span> <span data-ttu-id="17158-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17158-135">This is a read-only property.</span></span>|
|<span data-ttu-id="17158-136">displayName</span><span class="sxs-lookup"><span data-stu-id="17158-136">displayName</span></span>|<span data-ttu-id="17158-137">String</span><span class="sxs-lookup"><span data-stu-id="17158-137">String</span></span>|<span data-ttu-id="17158-138">Отображаемое имя Идентитюсерфловаттрибуте в пользовательском движении.</span><span class="sxs-lookup"><span data-stu-id="17158-138">The display name of the identityUserFlowAttribute within a user flow.</span></span>|
|<span data-ttu-id="17158-139">Переключатель</span><span class="sxs-lookup"><span data-stu-id="17158-139">isOptional</span></span>|<span data-ttu-id="17158-140">Логический</span><span class="sxs-lookup"><span data-stu-id="17158-140">Boolean</span></span>|<span data-ttu-id="17158-141">Определяет, является ли Идентитюсерфловаттрибуте необязательным.</span><span class="sxs-lookup"><span data-stu-id="17158-141">Determines whether the identityUserFlowAttribute is optional.</span></span> <span data-ttu-id="17158-142">`true` означает, что пользователю не нужно указывать значение.</span><span class="sxs-lookup"><span data-stu-id="17158-142">`true` means the user doesn't have to provide a value.</span></span> <span data-ttu-id="17158-143">`false` означает, что пользователь не может выполнить вход, не указывая значение.</span><span class="sxs-lookup"><span data-stu-id="17158-143">`false` means the user cannot complete sign-up without providing a value.</span></span>|
|<span data-ttu-id="17158-144">рекуиресверификатион</span><span class="sxs-lookup"><span data-stu-id="17158-144">requiresVerification</span></span>|<span data-ttu-id="17158-145">Логический</span><span class="sxs-lookup"><span data-stu-id="17158-145">Boolean</span></span>|<span data-ttu-id="17158-146">Определяет, требуется ли для Идентитюсерфловаттрибуте проверка.</span><span class="sxs-lookup"><span data-stu-id="17158-146">Determines whether the identityUserFlowAttribute requires verification.</span></span> <span data-ttu-id="17158-147">Используется только для проверки номера телефона пользователя или адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="17158-147">This is only used for verifying the user's phone number or email address.</span></span>|
|<span data-ttu-id="17158-148">усераттрибутевалуес</span><span class="sxs-lookup"><span data-stu-id="17158-148">userAttributeValues</span></span>|<span data-ttu-id="17158-149">Коллекция [усераттрибутевалуеситем](../resources/userattributevaluesitem.md)</span><span class="sxs-lookup"><span data-stu-id="17158-149">[userAttributeValuesItem](../resources/userattributevaluesitem.md) collection</span></span>|<span data-ttu-id="17158-150">Параметры ввода для атрибута Flow User.</span><span class="sxs-lookup"><span data-stu-id="17158-150">The input options for the user flow attribute.</span></span> <span data-ttu-id="17158-151">Применяется только в том случае, если для Усеринпуттипе задано значение `radioSingleSelect` , `dropdownSingleSelect` или `checkboxMultiSelect` .</span><span class="sxs-lookup"><span data-stu-id="17158-151">Only applicable when the userInputType is `radioSingleSelect`, `dropdownSingleSelect`, or `checkboxMultiSelect`.</span></span>|
|<span data-ttu-id="17158-152">усеринпуттипе</span><span class="sxs-lookup"><span data-stu-id="17158-152">userInputType</span></span>|<span data-ttu-id="17158-153">идентитюсерфловаттрибутеинпуттипе</span><span class="sxs-lookup"><span data-stu-id="17158-153">identityUserFlowAttributeInputType</span></span>|<span data-ttu-id="17158-154">Тип входных данных для атрибута Flow User.</span><span class="sxs-lookup"><span data-stu-id="17158-154">The input type of the user flow attribute.</span></span> <span data-ttu-id="17158-155">Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span><span class="sxs-lookup"><span data-stu-id="17158-155">Possible values are: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17158-156">Связи</span><span class="sxs-lookup"><span data-stu-id="17158-156">Relationships</span></span>

|<span data-ttu-id="17158-157">Связь</span><span class="sxs-lookup"><span data-stu-id="17158-157">Relationship</span></span>|<span data-ttu-id="17158-158">Тип</span><span class="sxs-lookup"><span data-stu-id="17158-158">Type</span></span>|<span data-ttu-id="17158-159">Описание</span><span class="sxs-lookup"><span data-stu-id="17158-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17158-160">усераттрибуте</span><span class="sxs-lookup"><span data-stu-id="17158-160">userAttribute</span></span>|[<span data-ttu-id="17158-161">идентитюсерфловаттрибуте</span><span class="sxs-lookup"><span data-stu-id="17158-161">identityUserFlowAttribute</span></span>](../resources/identityuserflowattribute.md)|<span data-ttu-id="17158-162">Атрибут пользователя, который требуется добавить в пользовательский блок.</span><span class="sxs-lookup"><span data-stu-id="17158-162">The user attribute that you want to add to your user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17158-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17158-163">JSON representation</span></span>

<span data-ttu-id="17158-164">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17158-164">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment",
  "baseType": "",
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
