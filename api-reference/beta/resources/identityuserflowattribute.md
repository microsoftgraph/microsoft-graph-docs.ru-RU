---
title: Тип ресурса identityUserFlowAttribute
description: Представляет атрибуты потоков пользователей в клиенте Azure Active Directory и клиенте Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: ca8930a5cb11edb1cf7345464666478cfc01bcda
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882602"
---
# <a name="identityuserflowattribute-resource-type"></a><span data-ttu-id="0c877-103">Тип ресурса identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="0c877-103">identityUserFlowAttribute resource type</span></span>

<span data-ttu-id="0c877-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c877-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c877-105">Представляет атрибуты потоков пользователей в клиенте Azure Active Directory (Azure AD) и клиенте Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="0c877-105">Represents user flow attributes in an Azure Active Directory (Azure AD) tenant and an Azure AD B2C tenant.</span></span>

<span data-ttu-id="0c877-106">Настройка атрибутов потоков пользователей в клиенте Azure AD или Azure AD B2C позволяет вам собирать сведения о пользователе во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="0c877-106">Configuring user flow attributes in your Azure AD or Azure AD B2C tenant allows you to collect information about a user during sign-up.</span></span> <span data-ttu-id="0c877-107">Вы можете выбрать сбор встроенного набора атрибутов, например имени, фамилии, города и почтового индекса.</span><span class="sxs-lookup"><span data-stu-id="0c877-107">You can choose to collect a built-in set of attribute; for example, Given Name, Surname, City, and Postal Code.</span></span> <span data-ttu-id="0c877-108">Кроме того, вы можете настроить специальные атрибуты потоков пользователей для сбора сведений о пользователе, которые не встроены в каталог.</span><span class="sxs-lookup"><span data-stu-id="0c877-108">You can also configure custom user flow attributes to collect information from a user that is not built in to the directory.</span></span> <span data-ttu-id="0c877-109">Настраиваемые атрибуты потоков пользователей — это абстрагирование от [расширений схемы Azure Active Directory](/azure/active-directory/develop/active-directory-schema-extensions).</span><span class="sxs-lookup"><span data-stu-id="0c877-109">Custom user flow attributes are an abstraction over [Azure Active Directory schema extensions](/azure/active-directory/develop/active-directory-schema-extensions).</span></span>

<span data-ttu-id="0c877-110">[identityBuiltInUserFlowAttributes](../resources/identitybuiltinuserflowattribute.md) и [identityCustomUserFlowAttributes](../resources/identitycustomuserflowattribute.md) наследуются от этого базового типа.</span><span class="sxs-lookup"><span data-stu-id="0c877-110">[identityBuiltInUserFlowAttributes](../resources/identitybuiltinuserflowattribute.md) and [identityCustomUserFlowAttributes](../resources/identitycustomuserflowattribute.md) both inherit from this base type.</span></span>

## <a name="methods"></a><span data-ttu-id="0c877-111">Методы</span><span class="sxs-lookup"><span data-stu-id="0c877-111">Methods</span></span>

| <span data-ttu-id="0c877-112">Метод</span><span class="sxs-lookup"><span data-stu-id="0c877-112">Method</span></span>       | <span data-ttu-id="0c877-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0c877-113">Return Type</span></span>  |<span data-ttu-id="0c877-114">Описание</span><span class="sxs-lookup"><span data-stu-id="0c877-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c877-115">Список</span><span class="sxs-lookup"><span data-stu-id="0c877-115">List</span></span>](../api/identityuserflowattribute-list.md)|<span data-ttu-id="0c877-116">identityUserFlowAttributes collection</span><span class="sxs-lookup"><span data-stu-id="0c877-116">identityUserFlowAttributes collection</span></span>|<span data-ttu-id="0c877-117">Извлечение всех встроенных и настраиваемых атрибутов потоков пользователей.</span><span class="sxs-lookup"><span data-stu-id="0c877-117">Retrieve all built-in and custom user flow attributes.</span></span>|
|[<span data-ttu-id="0c877-118">Создание</span><span class="sxs-lookup"><span data-stu-id="0c877-118">Create</span></span>](../api/identityuserflowattribute-post.md)|<span data-ttu-id="0c877-119">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="0c877-119">identityUserFlowAttribute</span></span>|<span data-ttu-id="0c877-120">Создание настраиваемого атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="0c877-120">Create a new custom user flow attribute.</span></span>|
|[<span data-ttu-id="0c877-121">Получение</span><span class="sxs-lookup"><span data-stu-id="0c877-121">Get</span></span>](../api/identityuserflowattribute-get.md) |<span data-ttu-id="0c877-122">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="0c877-122">identityUserFlowAttribute</span></span>|<span data-ttu-id="0c877-123">Извлечение свойств атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="0c877-123">Retrieve properties of a user flow attribute.</span></span>|
|[<span data-ttu-id="0c877-124">Обновление</span><span class="sxs-lookup"><span data-stu-id="0c877-124">Update</span></span>](../api/identityuserflowattribute-update.md)|<span data-ttu-id="0c877-125">Нет</span><span class="sxs-lookup"><span data-stu-id="0c877-125">None</span></span>|<span data-ttu-id="0c877-126">Обновление настраиваемого атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="0c877-126">Update a custom user flow attribute.</span></span>|
|<span data-ttu-id="0c877-127">[удаление](../api/identityuserflowattribute-delete.md);</span><span class="sxs-lookup"><span data-stu-id="0c877-127">[Delete](../api/identityuserflowattribute-delete.md)</span></span>|<span data-ttu-id="0c877-128">Нет</span><span class="sxs-lookup"><span data-stu-id="0c877-128">None</span></span>|<span data-ttu-id="0c877-129">Удаление настраиваемого атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="0c877-129">Delete a custom user flow attribute.</span></span>|

## <a name="properties"></a><span data-ttu-id="0c877-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c877-130">Properties</span></span>

|<span data-ttu-id="0c877-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c877-131">Property</span></span>|<span data-ttu-id="0c877-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0c877-132">Type</span></span>|<span data-ttu-id="0c877-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0c877-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c877-134">id</span><span class="sxs-lookup"><span data-stu-id="0c877-134">id</span></span>|<span data-ttu-id="0c877-135">String</span><span class="sxs-lookup"><span data-stu-id="0c877-135">String</span></span>|<span data-ttu-id="0c877-136">Идентификатор атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="0c877-136">The identifier of the user flow attribute.</span></span> <span data-ttu-id="0c877-137">Это автоматически созданный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c877-137">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="0c877-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0c877-138">displayName</span></span>|<span data-ttu-id="0c877-139">String</span><span class="sxs-lookup"><span data-stu-id="0c877-139">String</span></span>|<span data-ttu-id="0c877-140">Отображаемое имя атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="0c877-140">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="0c877-141">description</span><span class="sxs-lookup"><span data-stu-id="0c877-141">description</span></span>|<span data-ttu-id="0c877-142">String</span><span class="sxs-lookup"><span data-stu-id="0c877-142">String</span></span>|<span data-ttu-id="0c877-143">Описание атрибута потока пользователей, демонстрируемое пользователю при регистрации.</span><span class="sxs-lookup"><span data-stu-id="0c877-143">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="0c877-144">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="0c877-144">userFlowAttributeType</span></span>|<span data-ttu-id="0c877-145">identityUserFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="0c877-145">identityUserFlowAttributeType</span></span>|<span data-ttu-id="0c877-146">Тип атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="0c877-146">The type of the user flow attribute.</span></span> <span data-ttu-id="0c877-147">Это автоматически настроенный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c877-147">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="0c877-148">В зависимости от типа атрибута значением этого свойства является `builtIn`, `custom` или `required`.</span><span class="sxs-lookup"><span data-stu-id="0c877-148">Depending on the type of attribute, the values for this property will be `builtIn`, `custom`, or `required`.</span></span>|
|<span data-ttu-id="0c877-149">dataType</span><span class="sxs-lookup"><span data-stu-id="0c877-149">dataType</span></span>|<span data-ttu-id="0c877-150">identityUserFlowAttributeDataType</span><span class="sxs-lookup"><span data-stu-id="0c877-150">identityUserFlowAttributeDataType</span></span>|<span data-ttu-id="0c877-151">Тип данных атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="0c877-151">The data type of the user flow attribute.</span></span> <span data-ttu-id="0c877-152">Это свойство нельзя изменить после создания атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="0c877-152">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="0c877-153">Поддерживаемые значения для **dataType**: `string`, `boolean`, `int64`, `stringCollection`, `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="0c877-153">The supported values for **dataType** are: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c877-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c877-154">JSON representation</span></span>

<span data-ttu-id="0c877-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c877-155">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```json
{
    "@odata.type": "#microsoft.graph.identityUserFlowAttribute",
    "id": "String (identifier)",
    "displayName": "String",
    "description": "String",
    "userFlowAttributeType": "String",
    "dataType": "String"
}
```
