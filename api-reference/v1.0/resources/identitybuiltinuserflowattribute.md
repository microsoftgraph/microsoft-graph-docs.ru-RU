---
title: identityBuiltInUserFlowAttribute type
description: Представляет встроенный атрибут потока пользователей в клиентах Azure Active Directory, который можно использовать в потоке пользователей для самостоятельной регистрации.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c549be6035b26d6e2d7faedafb6848240a9303dc
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883346"
---
# <a name="identitybuiltinuserflowattribute-resource-type"></a><span data-ttu-id="4c93f-103">identityBuiltInUserFlowAttribute type</span><span class="sxs-lookup"><span data-stu-id="4c93f-103">identityBuiltInUserFlowAttribute resource type</span></span>

<span data-ttu-id="4c93f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c93f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c93f-105">Представляет встроенный атрибут потока пользователей в клиентах Azure Active Directory, который можно использовать в потоке пользователей для самостоятельной регистрации.</span><span class="sxs-lookup"><span data-stu-id="4c93f-105">Represents a built-in user flow attribute in Azure Active Directory tenants that can be used in a self-service sign-up user flow.</span></span> <span data-ttu-id="4c93f-106">Эти атрибуты не могут быть изменены и являются только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c93f-106">These attributes cannot be modified and are read-only.</span></span>

<span data-ttu-id="4c93f-107">Наследует [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="4c93f-107">Inherits from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4c93f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c93f-108">Properties</span></span>

|<span data-ttu-id="4c93f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c93f-109">Property</span></span>|<span data-ttu-id="4c93f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4c93f-110">Type</span></span>|<span data-ttu-id="4c93f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4c93f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c93f-112">id</span><span class="sxs-lookup"><span data-stu-id="4c93f-112">id</span></span>|<span data-ttu-id="4c93f-113">String</span><span class="sxs-lookup"><span data-stu-id="4c93f-113">String</span></span>|<span data-ttu-id="4c93f-114">Идентификатор атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="4c93f-114">The identifier of the user flow attribute.</span></span> <span data-ttu-id="4c93f-115">Это автоматически созданный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c93f-115">This is a read-only attribute that is automatically created.</span></span> <span data-ttu-id="4c93f-116">Унаследованный от [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="4c93f-116">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span></span>|
|<span data-ttu-id="4c93f-117">displayName</span><span class="sxs-lookup"><span data-stu-id="4c93f-117">displayName</span></span>|<span data-ttu-id="4c93f-118">String</span><span class="sxs-lookup"><span data-stu-id="4c93f-118">String</span></span>|<span data-ttu-id="4c93f-119">Отображаемое имя атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="4c93f-119">The display name of the user flow attribute.</span></span> <span data-ttu-id="4c93f-120">Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="4c93f-120">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="4c93f-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c93f-121">Read-only.</span></span>|
|<span data-ttu-id="4c93f-122">description</span><span class="sxs-lookup"><span data-stu-id="4c93f-122">description</span></span>|<span data-ttu-id="4c93f-123">String</span><span class="sxs-lookup"><span data-stu-id="4c93f-123">String</span></span>|<span data-ttu-id="4c93f-124">Описание атрибута потока пользователей, демонстрируемое пользователю при регистрации.</span><span class="sxs-lookup"><span data-stu-id="4c93f-124">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span> <span data-ttu-id="4c93f-125">Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="4c93f-125">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="4c93f-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c93f-126">Read-only.</span></span>|
|<span data-ttu-id="4c93f-127">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="4c93f-127">userFlowAttributeType</span></span>|<span data-ttu-id="4c93f-128">identityUserFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="4c93f-128">identityUserFlowAttributeType</span></span>|<span data-ttu-id="4c93f-129">Тип атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="4c93f-129">The type of the user flow attribute.</span></span> <span data-ttu-id="4c93f-130">Это автоматически настроенный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c93f-130">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="4c93f-131">Значение для этого свойства будет `builtIn` .</span><span class="sxs-lookup"><span data-stu-id="4c93f-131">The value for this property will be `builtIn`.</span></span> <span data-ttu-id="4c93f-132">Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="4c93f-132">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="4c93f-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c93f-133">Read-only.</span></span>|
|<span data-ttu-id="4c93f-134">dataType</span><span class="sxs-lookup"><span data-stu-id="4c93f-134">dataType</span></span>|<span data-ttu-id="4c93f-135">identityUserFlowAttributeDataType</span><span class="sxs-lookup"><span data-stu-id="4c93f-135">identityUserFlowAttributeDataType</span></span>|<span data-ttu-id="4c93f-136">Тип данных атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="4c93f-136">The data type of the user flow attribute.</span></span> <span data-ttu-id="4c93f-137">Это свойство нельзя изменить после создания атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="4c93f-137">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="4c93f-138">Поддерживаемые значения для **dataType**: `string`, `boolean`, `int64`, `stringCollection`, `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="4c93f-138">The supported values for **dataType** are: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span></span> <span data-ttu-id="4c93f-139">Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="4c93f-139">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="4c93f-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4c93f-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c93f-141">Связи</span><span class="sxs-lookup"><span data-stu-id="4c93f-141">Relationships</span></span>

<span data-ttu-id="4c93f-142">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4c93f-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c93f-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4c93f-143">JSON representation</span></span>

<span data-ttu-id="4c93f-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c93f-144">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityBuiltInUserFlowAttribute",
  "baseType": "microsoft.graph.identityUserFlowAttribute",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityBuiltInUserFlowAttribute",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "userFlowAttributeType": "String",
  "dataType": "String"
}
```
