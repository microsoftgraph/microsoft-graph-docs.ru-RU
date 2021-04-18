---
title: Тип ресурса identityUserFlowAttribute
description: Представляет атрибуты потоков пользователей в клиенте Azure Active Directory и клиенте Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: af3ec2a762fc0252da929d863917ba6cd274ba95
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883115"
---
# <a name="identityuserflowattribute-resource-type"></a><span data-ttu-id="11bd1-103">Тип ресурса identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="11bd1-103">identityUserFlowAttribute resource type</span></span>

<span data-ttu-id="11bd1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11bd1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11bd1-105">Представляет атрибуты потоков пользователей в клиенте Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="11bd1-105">Represents user flow attributes in an Azure Active Directory (Azure AD) tenant.</span></span>

<span data-ttu-id="11bd1-106">Настройка атрибутов потоков пользователей в клиенте Azure AD позволяет вам собирать сведения о пользователе во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="11bd1-106">Configuring user flow attributes in your Azure AD tenant allows you to collect information about a user during sign-up.</span></span> <span data-ttu-id="11bd1-107">Вы можете собирать встроенный набор атрибутов.</span><span class="sxs-lookup"><span data-stu-id="11bd1-107">You can choose to collect a built-in set of attributes.</span></span> <span data-ttu-id="11bd1-108">Например, имя, фамилию, город и почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="11bd1-108">For example, given name, surname, city, and postal code.</span></span> <span data-ttu-id="11bd1-109">Кроме того, вы можете настроить специальные атрибуты потоков пользователей для сбора сведений о пользователе, которые не встроены в каталог.</span><span class="sxs-lookup"><span data-stu-id="11bd1-109">You can also configure custom user flow attributes to collect information from a user that is not built in to the directory.</span></span> <span data-ttu-id="11bd1-110">Настраиваемые атрибуты потоков пользователей — это абстрагирование от [расширений схемы Azure Active Directory](/azure/active-directory/develop/active-directory-schema-extensions).</span><span class="sxs-lookup"><span data-stu-id="11bd1-110">Custom user flow attributes are an abstraction over [Azure Active Directory schema extensions](/azure/active-directory/develop/active-directory-schema-extensions).</span></span>

## <a name="methods"></a><span data-ttu-id="11bd1-111">Методы</span><span class="sxs-lookup"><span data-stu-id="11bd1-111">Methods</span></span>

| <span data-ttu-id="11bd1-112">Метод</span><span class="sxs-lookup"><span data-stu-id="11bd1-112">Method</span></span>       | <span data-ttu-id="11bd1-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="11bd1-113">Return Type</span></span>  |<span data-ttu-id="11bd1-114">Описание</span><span class="sxs-lookup"><span data-stu-id="11bd1-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="11bd1-115">Список</span><span class="sxs-lookup"><span data-stu-id="11bd1-115">List</span></span>](../api/identityuserflowattribute-list.md)|<span data-ttu-id="11bd1-116">identityUserFlowAttributes collection</span><span class="sxs-lookup"><span data-stu-id="11bd1-116">identityUserFlowAttributes collection</span></span>|<span data-ttu-id="11bd1-117">Извлечение всех встроенных и настраиваемых атрибутов потоков пользователей.</span><span class="sxs-lookup"><span data-stu-id="11bd1-117">Retrieve all built-in and custom user flow attributes.</span></span>|
|[<span data-ttu-id="11bd1-118">Создание</span><span class="sxs-lookup"><span data-stu-id="11bd1-118">Create</span></span>](../api/identityuserflowattribute-post.md)|<span data-ttu-id="11bd1-119">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="11bd1-119">identityUserFlowAttribute</span></span>|<span data-ttu-id="11bd1-120">Создание настраиваемого атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="11bd1-120">Create a new custom user flow attribute.</span></span>|
|[<span data-ttu-id="11bd1-121">Получение</span><span class="sxs-lookup"><span data-stu-id="11bd1-121">Get</span></span>](../api/identityuserflowattribute-get.md) |<span data-ttu-id="11bd1-122">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="11bd1-122">identityUserFlowAttribute</span></span>|<span data-ttu-id="11bd1-123">Извлечение свойств атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="11bd1-123">Retrieve properties of a user flow attribute.</span></span>|
|[<span data-ttu-id="11bd1-124">Обновление</span><span class="sxs-lookup"><span data-stu-id="11bd1-124">Update</span></span>](../api/identityuserflowattribute-update.md)|<span data-ttu-id="11bd1-125">Нет</span><span class="sxs-lookup"><span data-stu-id="11bd1-125">None</span></span>|<span data-ttu-id="11bd1-126">Обновление настраиваемого атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="11bd1-126">Update a custom user flow attribute.</span></span>|
|<span data-ttu-id="11bd1-127">[удаление](../api/identityuserflowattribute-delete.md);</span><span class="sxs-lookup"><span data-stu-id="11bd1-127">[Delete](../api/identityuserflowattribute-delete.md)</span></span>|<span data-ttu-id="11bd1-128">Нет</span><span class="sxs-lookup"><span data-stu-id="11bd1-128">None</span></span>|<span data-ttu-id="11bd1-129">Удаление настраиваемого атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="11bd1-129">Delete a custom user flow attribute.</span></span>|

## <a name="properties"></a><span data-ttu-id="11bd1-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="11bd1-130">Properties</span></span>

|<span data-ttu-id="11bd1-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="11bd1-131">Property</span></span>|<span data-ttu-id="11bd1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="11bd1-132">Type</span></span>|<span data-ttu-id="11bd1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="11bd1-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11bd1-134">id</span><span class="sxs-lookup"><span data-stu-id="11bd1-134">id</span></span>|<span data-ttu-id="11bd1-135">String</span><span class="sxs-lookup"><span data-stu-id="11bd1-135">String</span></span>|<span data-ttu-id="11bd1-136">Идентификатор атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="11bd1-136">The identifier of the user flow attribute.</span></span> <span data-ttu-id="11bd1-137">Это автоматически созданный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="11bd1-137">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="11bd1-138">displayName</span><span class="sxs-lookup"><span data-stu-id="11bd1-138">displayName</span></span>|<span data-ttu-id="11bd1-139">String</span><span class="sxs-lookup"><span data-stu-id="11bd1-139">String</span></span>|<span data-ttu-id="11bd1-140">Отображаемое имя атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="11bd1-140">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="11bd1-141">description</span><span class="sxs-lookup"><span data-stu-id="11bd1-141">description</span></span>|<span data-ttu-id="11bd1-142">String</span><span class="sxs-lookup"><span data-stu-id="11bd1-142">String</span></span>|<span data-ttu-id="11bd1-143">Описание атрибута потока пользователей, демонстрируемое пользователю при регистрации.</span><span class="sxs-lookup"><span data-stu-id="11bd1-143">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="11bd1-144">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="11bd1-144">userFlowAttributeType</span></span>|<span data-ttu-id="11bd1-145">identityUserFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="11bd1-145">identityUserFlowAttributeType</span></span>|<span data-ttu-id="11bd1-146">Тип атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="11bd1-146">The type of the user flow attribute.</span></span> <span data-ttu-id="11bd1-147">Это автоматически настроенный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="11bd1-147">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="11bd1-148">В зависимости от типа атрибута значением этого свойства является `builtIn`, `custom` или `required`.</span><span class="sxs-lookup"><span data-stu-id="11bd1-148">Depending on the type of attribute, the values for this property will be `builtIn`, `custom`, or `required`.</span></span>|
|<span data-ttu-id="11bd1-149">dataType</span><span class="sxs-lookup"><span data-stu-id="11bd1-149">dataType</span></span>|<span data-ttu-id="11bd1-150">identityUserFlowAttributeDataType</span><span class="sxs-lookup"><span data-stu-id="11bd1-150">identityUserFlowAttributeDataType</span></span>|<span data-ttu-id="11bd1-151">Тип данных атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="11bd1-151">The data type of the user flow attribute.</span></span> <span data-ttu-id="11bd1-152">Это свойство нельзя изменить после создания атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="11bd1-152">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="11bd1-153">Поддерживаемые значения для **dataType**: `string`, `boolean`, `int64`, `stringCollection`, `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="11bd1-153">The supported values for **dataType** are: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11bd1-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11bd1-154">JSON representation</span></span>

<span data-ttu-id="11bd1-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11bd1-155">The following is a JSON representation of the resource.</span></span>

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
