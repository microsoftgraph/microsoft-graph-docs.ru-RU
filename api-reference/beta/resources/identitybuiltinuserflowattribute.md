---
title: identityBuiltInUserFlowAttribute type
description: Представляет встроенный атрибут потока пользователей в клиентах Azure Active Directory, который можно использовать в потоках пользователей для самостоятельной регистрации.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e3d6c9eef25f428734214854d28a342f9c4f59dd
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882734"
---
# <a name="identitybuiltinuserflowattribute-resource-type"></a><span data-ttu-id="3ba6c-103">identityBuiltInUserFlowAttribute type</span><span class="sxs-lookup"><span data-stu-id="3ba6c-103">identityBuiltInUserFlowAttribute resource type</span></span>

<span data-ttu-id="3ba6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ba6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ba6c-105">Представляет встроенный атрибут потока пользователей в клиентах Azure Active Directory, который можно использовать в потоках пользователей для самостоятельной регистрации.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-105">Represents a built-in user flow attribute in Azure Active Directory tenants that can be used in your self-service sign-up user flows.</span></span> <span data-ttu-id="3ba6c-106">Эти атрибуты не могут быть изменены и являются только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-106">These attributes cannot be modified and are read-only.</span></span>

<span data-ttu-id="3ba6c-107">Наследует [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="3ba6c-107">Inherits from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3ba6c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ba6c-108">Properties</span></span>

|<span data-ttu-id="3ba6c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ba6c-109">Property</span></span>|<span data-ttu-id="3ba6c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3ba6c-110">Type</span></span>|<span data-ttu-id="3ba6c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3ba6c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ba6c-112">id</span><span class="sxs-lookup"><span data-stu-id="3ba6c-112">id</span></span>|<span data-ttu-id="3ba6c-113">String</span><span class="sxs-lookup"><span data-stu-id="3ba6c-113">String</span></span>|<span data-ttu-id="3ba6c-114">Идентификатор атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-114">The identifier of the user flow attribute.</span></span> <span data-ttu-id="3ba6c-115">Это автоматически созданный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-115">This is a read-only attribute that is automatically created.</span></span> <span data-ttu-id="3ba6c-116">Унаследованный от [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="3ba6c-116">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span></span>|
|<span data-ttu-id="3ba6c-117">displayName</span><span class="sxs-lookup"><span data-stu-id="3ba6c-117">displayName</span></span>|<span data-ttu-id="3ba6c-118">String</span><span class="sxs-lookup"><span data-stu-id="3ba6c-118">String</span></span>|<span data-ttu-id="3ba6c-119">Отображаемое имя атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-119">The display name of the user flow attribute.</span></span> <span data-ttu-id="3ba6c-120">Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="3ba6c-120">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="3ba6c-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-121">Read-only.</span></span>|
|<span data-ttu-id="3ba6c-122">description</span><span class="sxs-lookup"><span data-stu-id="3ba6c-122">description</span></span>|<span data-ttu-id="3ba6c-123">String</span><span class="sxs-lookup"><span data-stu-id="3ba6c-123">String</span></span>|<span data-ttu-id="3ba6c-124">Описание атрибута потока пользователей, демонстрируемое пользователю при регистрации.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-124">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span> <span data-ttu-id="3ba6c-125">Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="3ba6c-125">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="3ba6c-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-126">Read-only.</span></span>|
|<span data-ttu-id="3ba6c-127">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="3ba6c-127">userFlowAttributeType</span></span>|<span data-ttu-id="3ba6c-128">identityUserFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="3ba6c-128">identityUserFlowAttributeType</span></span>|<span data-ttu-id="3ba6c-129">Тип атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-129">The type of the user flow attribute.</span></span> <span data-ttu-id="3ba6c-130">Это автоматически настроенный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-130">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="3ba6c-131">Значение для этого свойства будет `builtIn` .</span><span class="sxs-lookup"><span data-stu-id="3ba6c-131">The value for this property will be `builtIn`.</span></span> <span data-ttu-id="3ba6c-132">Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="3ba6c-132">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="3ba6c-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-133">Read-only.</span></span>|
|<span data-ttu-id="3ba6c-134">dataType</span><span class="sxs-lookup"><span data-stu-id="3ba6c-134">dataType</span></span>|<span data-ttu-id="3ba6c-135">identityUserFlowAttributeDataType</span><span class="sxs-lookup"><span data-stu-id="3ba6c-135">identityUserFlowAttributeDataType</span></span>|<span data-ttu-id="3ba6c-136">Тип данных атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-136">The data type of the user flow attribute.</span></span> <span data-ttu-id="3ba6c-137">Это свойство нельзя изменить после создания атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-137">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="3ba6c-138">Поддерживаемые значения для **dataType**: `string`, `boolean`, `int64`, `stringCollection`, `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-138">The supported values for **dataType** are: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span></span> <span data-ttu-id="3ba6c-139">Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="3ba6c-139">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="3ba6c-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ba6c-141">Связи</span><span class="sxs-lookup"><span data-stu-id="3ba6c-141">Relationships</span></span>

<span data-ttu-id="3ba6c-142">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ba6c-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3ba6c-143">JSON representation</span></span>

<span data-ttu-id="3ba6c-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ba6c-144">The following is a JSON representation of the resource.</span></span>
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
