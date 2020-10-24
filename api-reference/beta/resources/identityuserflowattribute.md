---
title: Тип ресурса identityUserFlowAttribute
description: Представляет атрибуты потоков пользователей в клиенте Azure Active Directory и клиенте Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: f5166cafff64a7050b89bbd7f70cba66f429646d
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742422"
---
# <a name="identityuserflowattribute-resource-type"></a><span data-ttu-id="6d809-103">Тип ресурса identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="6d809-103">identityUserFlowAttribute resource type</span></span>

<span data-ttu-id="6d809-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d809-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d809-105">Представляет атрибуты потоков пользователей в клиенте Azure Active Directory (Azure AD) и клиенте Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="6d809-105">Represents user flow attributes in an Azure Active Directory (Azure AD) tenant and an Azure AD B2C tenant.</span></span>

<span data-ttu-id="6d809-106">Настройка атрибутов потоков пользователей в клиенте Azure AD или Azure AD B2C позволяет вам собирать сведения о пользователе во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="6d809-106">Configuring user flow attributes in your Azure AD or Azure AD B2C tenant allows you to collect information about a user during sign-up.</span></span> <span data-ttu-id="6d809-107">Вы можете выбрать сбор встроенного набора атрибутов, например имени, фамилии, города и почтового индекса.</span><span class="sxs-lookup"><span data-stu-id="6d809-107">You can choose to collect a built-in set of attribute; for example, Given Name, Surname, City, and Postal Code.</span></span> <span data-ttu-id="6d809-108">Кроме того, вы можете настроить специальные атрибуты потоков пользователей для сбора сведений о пользователе, которые не встроены в каталог.</span><span class="sxs-lookup"><span data-stu-id="6d809-108">You can also configure custom user flow attributes to collect information from a user that is not built in to the directory.</span></span> <span data-ttu-id="6d809-109">Настраиваемые атрибуты потоков пользователей — это абстрагирование от [расширений схемы Azure Active Directory](/azure/active-directory/develop/active-directory-schema-extensions).</span><span class="sxs-lookup"><span data-stu-id="6d809-109">Custom user flow attributes are an abstraction over [Azure Active Directory schema extensions](/azure/active-directory/develop/active-directory-schema-extensions).</span></span>

## <a name="methods"></a><span data-ttu-id="6d809-110">Методы</span><span class="sxs-lookup"><span data-stu-id="6d809-110">Methods</span></span>

| <span data-ttu-id="6d809-111">Метод</span><span class="sxs-lookup"><span data-stu-id="6d809-111">Method</span></span>       | <span data-ttu-id="6d809-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6d809-112">Return Type</span></span>  |<span data-ttu-id="6d809-113">Описание</span><span class="sxs-lookup"><span data-stu-id="6d809-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6d809-114">Список</span><span class="sxs-lookup"><span data-stu-id="6d809-114">List</span></span>](../api/identityuserflowattribute-list.md)|<span data-ttu-id="6d809-115">identityUserFlowAttributes collection</span><span class="sxs-lookup"><span data-stu-id="6d809-115">identityUserFlowAttributes collection</span></span>|<span data-ttu-id="6d809-116">Извлечение всех встроенных и настраиваемых атрибутов потоков пользователей.</span><span class="sxs-lookup"><span data-stu-id="6d809-116">Retrieve all built-in and custom user flow attributes.</span></span>|
|[<span data-ttu-id="6d809-117">Создание</span><span class="sxs-lookup"><span data-stu-id="6d809-117">Create</span></span>](../api/identityuserflowattribute-post.md)|<span data-ttu-id="6d809-118">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="6d809-118">identityUserFlowAttribute</span></span>|<span data-ttu-id="6d809-119">Создание настраиваемого атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="6d809-119">Create a new custom user flow attribute.</span></span>|
|[<span data-ttu-id="6d809-120">Получение</span><span class="sxs-lookup"><span data-stu-id="6d809-120">Get</span></span>](../api/identityuserflowattribute-get.md) |<span data-ttu-id="6d809-121">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="6d809-121">identityUserFlowAttribute</span></span>|<span data-ttu-id="6d809-122">Извлечение свойств атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="6d809-122">Retrieve properties of a user flow attribute.</span></span>|
|[<span data-ttu-id="6d809-123">Обновление</span><span class="sxs-lookup"><span data-stu-id="6d809-123">Update</span></span>](../api/identityuserflowattribute-update.md)|<span data-ttu-id="6d809-124">Нет</span><span class="sxs-lookup"><span data-stu-id="6d809-124">None</span></span>|<span data-ttu-id="6d809-125">Обновление настраиваемого атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="6d809-125">Update a custom user flow attribute.</span></span>|
|<span data-ttu-id="6d809-126">[удаление](../api/identityuserflowattribute-delete.md);</span><span class="sxs-lookup"><span data-stu-id="6d809-126">[Delete](../api/identityuserflowattribute-delete.md)</span></span>|<span data-ttu-id="6d809-127">Нет</span><span class="sxs-lookup"><span data-stu-id="6d809-127">None</span></span>|<span data-ttu-id="6d809-128">Удаление настраиваемого атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="6d809-128">Delete a custom user flow attribute.</span></span>|

## <a name="properties"></a><span data-ttu-id="6d809-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d809-129">Properties</span></span>

|<span data-ttu-id="6d809-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d809-130">Property</span></span>|<span data-ttu-id="6d809-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6d809-131">Type</span></span>|<span data-ttu-id="6d809-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6d809-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d809-133">id</span><span class="sxs-lookup"><span data-stu-id="6d809-133">id</span></span>|<span data-ttu-id="6d809-134">String</span><span class="sxs-lookup"><span data-stu-id="6d809-134">String</span></span>|<span data-ttu-id="6d809-135">Идентификатор атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="6d809-135">The identifier of the user flow attribute.</span></span> <span data-ttu-id="6d809-136">Это автоматически созданный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6d809-136">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="6d809-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6d809-137">displayName</span></span>|<span data-ttu-id="6d809-138">String</span><span class="sxs-lookup"><span data-stu-id="6d809-138">String</span></span>|<span data-ttu-id="6d809-139">Отображаемое имя атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="6d809-139">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="6d809-140">description</span><span class="sxs-lookup"><span data-stu-id="6d809-140">description</span></span>|<span data-ttu-id="6d809-141">String</span><span class="sxs-lookup"><span data-stu-id="6d809-141">String</span></span>|<span data-ttu-id="6d809-142">Описание атрибута потока пользователей, демонстрируемое пользователю при регистрации.</span><span class="sxs-lookup"><span data-stu-id="6d809-142">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="6d809-143">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="6d809-143">userFlowAttributeType</span></span>|<span data-ttu-id="6d809-144">String</span><span class="sxs-lookup"><span data-stu-id="6d809-144">String</span></span>|<span data-ttu-id="6d809-145">Тип атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="6d809-145">The type of the user flow attribute.</span></span> <span data-ttu-id="6d809-146">Это автоматически настроенный атрибут только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6d809-146">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="6d809-147">В зависимости от типа атрибута значением этого свойства является `builtIn` или `custom`.</span><span class="sxs-lookup"><span data-stu-id="6d809-147">Depending on the type of attribute, the values for this property will be `builtIn` or `custom`.</span></span>|
|<span data-ttu-id="6d809-148">dataType</span><span class="sxs-lookup"><span data-stu-id="6d809-148">dataType</span></span>|<span data-ttu-id="6d809-149">String</span><span class="sxs-lookup"><span data-stu-id="6d809-149">String</span></span>|<span data-ttu-id="6d809-150">Тип данных атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="6d809-150">The data type of the user flow attribute.</span></span> <span data-ttu-id="6d809-151">Это свойство нельзя изменить после создания атрибута потока пользователей.</span><span class="sxs-lookup"><span data-stu-id="6d809-151">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="6d809-152">Поддерживаемые значения для **dataType**:</span><span class="sxs-lookup"><span data-stu-id="6d809-152">The supported values for **dataType** are:</span></span><br/><ul><li><span data-ttu-id="6d809-153">`string` — указывает, что dataType для identityUserFlowAttribute является строкой.</span><span class="sxs-lookup"><span data-stu-id="6d809-153">`string` - denotes that the dataType for the identityUserFlowAttribute is a string.</span></span> </li><li><span data-ttu-id="6d809-154">`boolean` — указывает, что dataType для identityUserFlowAttribute является логическим значением.</span><span class="sxs-lookup"><span data-stu-id="6d809-154">`boolean` - denotes that the dataType for the identityUserFlowAttribute is a Boolean.</span></span></li><li><span data-ttu-id="6d809-155">`int64` — указывает, что dataType для identityUserFlowAttribute является целым числом.</span><span class="sxs-lookup"><span data-stu-id="6d809-155">`int64` - denotes that the dataType for the identityUserFlowAttribute is an integer.</span></span></li></ul>|

## <a name="json-representation"></a><span data-ttu-id="6d809-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d809-156">JSON representation</span></span>

<span data-ttu-id="6d809-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d809-157">The following is a JSON representation of the resource.</span></span>

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
