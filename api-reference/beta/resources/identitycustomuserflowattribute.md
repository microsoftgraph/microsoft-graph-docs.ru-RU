---
title: тип ресурса identityCustomUserFlowAttribute
description: Представляет настраиваемый атрибут потока пользователей в клиентах Azure Active Directory, который можно использовать в потоках пользователей самообслуживки.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3a07ea64be3cf5a215c43271982b7fdfce3f6662
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882731"
---
# <a name="identitycustomuserflowattribute-resource-type"></a><span data-ttu-id="fa7cf-103">тип ресурса identityCustomUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="fa7cf-103">identityCustomUserFlowAttribute resource type</span></span>

<span data-ttu-id="fa7cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa7cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa7cf-105">Представляет настраиваемый атрибут потока пользователей в клиентах Azure Active Directory, который можно использовать в потоках пользователей самообслуживки.</span><span class="sxs-lookup"><span data-stu-id="fa7cf-105">Represents a custom user flow attribute in Azure Active Directory tenants that can be used in your self-service sign-up user flows.</span></span> <span data-ttu-id="fa7cf-106">Эти атрибуты не могут быть изменены и являются только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa7cf-106">These attributes cannot be modified and are read-only.</span></span>

<span data-ttu-id="fa7cf-107">Наследует [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="fa7cf-107">Inherits from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fa7cf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa7cf-108">Properties</span></span>

|<span data-ttu-id="fa7cf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa7cf-109">Property</span></span>|<span data-ttu-id="fa7cf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fa7cf-110">Type</span></span>|<span data-ttu-id="fa7cf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fa7cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa7cf-112">id</span><span class="sxs-lookup"><span data-stu-id="fa7cf-112">id</span></span>|<span data-ttu-id="fa7cf-113">String</span><span class="sxs-lookup"><span data-stu-id="fa7cf-113">String</span></span>|<span data-ttu-id="fa7cf-114">Идентификатор атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="fa7cf-114">The identifier of the user flow attribute.</span></span> <span data-ttu-id="fa7cf-115">Это автоматически созданный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa7cf-115">This is a read-only attribute that is automatically created.</span></span> <span data-ttu-id="fa7cf-116">Унаследованный от [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="fa7cf-116">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span></span>|
|<span data-ttu-id="fa7cf-117">displayName</span><span class="sxs-lookup"><span data-stu-id="fa7cf-117">displayName</span></span>|<span data-ttu-id="fa7cf-118">String</span><span class="sxs-lookup"><span data-stu-id="fa7cf-118">String</span></span>|<span data-ttu-id="fa7cf-119">Отображаемое имя атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="fa7cf-119">The display name of the user flow attribute.</span></span> <span data-ttu-id="fa7cf-120">Унаследованный от [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="fa7cf-120">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span></span>|
|<span data-ttu-id="fa7cf-121">description</span><span class="sxs-lookup"><span data-stu-id="fa7cf-121">description</span></span>|<span data-ttu-id="fa7cf-122">String</span><span class="sxs-lookup"><span data-stu-id="fa7cf-122">String</span></span>|<span data-ttu-id="fa7cf-123">Описание атрибута потока пользователей, демонстрируемое пользователю при регистрации.</span><span class="sxs-lookup"><span data-stu-id="fa7cf-123">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span> <span data-ttu-id="fa7cf-124">Унаследованный от [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="fa7cf-124">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span></span>|
|<span data-ttu-id="fa7cf-125">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="fa7cf-125">userFlowAttributeType</span></span>|<span data-ttu-id="fa7cf-126">identityUserFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="fa7cf-126">identityUserFlowAttributeType</span></span>|<span data-ttu-id="fa7cf-127">Тип атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="fa7cf-127">The type of the user flow attribute.</span></span> <span data-ttu-id="fa7cf-128">Это автоматически настроенный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa7cf-128">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="fa7cf-129">Значение для этого свойства будет `custom` .</span><span class="sxs-lookup"><span data-stu-id="fa7cf-129">The value for this property will be `custom`.</span></span> <span data-ttu-id="fa7cf-130">Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="fa7cf-130">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>|
|<span data-ttu-id="fa7cf-131">dataType</span><span class="sxs-lookup"><span data-stu-id="fa7cf-131">dataType</span></span>|<span data-ttu-id="fa7cf-132">identityUserFlowAttributeDataType</span><span class="sxs-lookup"><span data-stu-id="fa7cf-132">identityUserFlowAttributeDataType</span></span>|<span data-ttu-id="fa7cf-133">Тип данных атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="fa7cf-133">The data type of the user flow attribute.</span></span> <span data-ttu-id="fa7cf-134">Это свойство нельзя изменить после создания атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="fa7cf-134">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="fa7cf-135">Поддерживаемые значения для **dataType**: `string`, `boolean`, `int64`, `stringCollection`, `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="fa7cf-135">The supported values for **dataType** are: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span></span> <span data-ttu-id="fa7cf-136">Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span><span class="sxs-lookup"><span data-stu-id="fa7cf-136">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa7cf-137">Связи</span><span class="sxs-lookup"><span data-stu-id="fa7cf-137">Relationships</span></span>

<span data-ttu-id="fa7cf-138">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fa7cf-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa7cf-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fa7cf-139">JSON representation</span></span>

<span data-ttu-id="fa7cf-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa7cf-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityCustomUserFlowAttribute",
  "baseType": "microsoft.graph.identityUserFlowAttribute",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityCustomUserFlowAttribute",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "userFlowAttributeType": "String",
  "dataType": "String"
}
```
