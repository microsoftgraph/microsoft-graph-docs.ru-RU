---
title: Тип ресурса profileCardProperty
description: Используется для назначить новое свойство, которое будет отображаться в общем, пользовательском или пользовательском отображаемом имени или аннотации. Администратор может определить строку отображаемого имени по умолчанию и набор альтернативных переводов для поддерживаемого в организации языка.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 33d2b1111580ba2302848ab1dbce3f773055a0b4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153566"
---
# <a name="profilecardproperty-resource-type"></a><span data-ttu-id="29877-104">Тип ресурса profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="29877-104">profileCardProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29877-105">Представляет атрибут пользователя в карточке профиля Microsoft 365, чтобы организация представляла общий интерфейс пользователей.</span><span class="sxs-lookup"><span data-stu-id="29877-105">Represents an attribute of a user on the Microsoft 365 profile card for an organization to surface in a shared, people experience.</span></span>

<span data-ttu-id="29877-106">Атрибут может быть встроенным атрибутом Azure Active Directory (Azure AD), например или настраиваемый `Alias` `UserPrincipalName` атрибут.</span><span class="sxs-lookup"><span data-stu-id="29877-106">The attribute can be an Azure Active Directory (Azure AD) built-in attribute, such as `Alias` or `UserPrincipalName`, or it can be a custom attribute.</span></span> <span data-ttu-id="29877-107">Для настраиваемого атрибута администратор может определить строку отображаемого имени по умолчанию и набор альтернативных переводов для поддерживаемого в `en-us` организации языка.</span><span class="sxs-lookup"><span data-stu-id="29877-107">For a custom attribute, an administrator can define an `en-us` default display name string and a set of alternative translations for the languages that they support in their organization.</span></span>

<span data-ttu-id="29877-108">Дополнительные сведения о добавлении свойств в карточку профиля для организации см. в [подстройке карточки профиля.](/graph/add-properties-profilecard)</span><span class="sxs-lookup"><span data-stu-id="29877-108">For more information on adding properties to the profile card for an organization, see [customize the profile card](/graph/add-properties-profilecard).</span></span>

## <a name="methods"></a><span data-ttu-id="29877-109">Методы</span><span class="sxs-lookup"><span data-stu-id="29877-109">Methods</span></span>

| <span data-ttu-id="29877-110">Метод</span><span class="sxs-lookup"><span data-stu-id="29877-110">Method</span></span>       | <span data-ttu-id="29877-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="29877-111">Return Type</span></span> | <span data-ttu-id="29877-112">Описание</span><span class="sxs-lookup"><span data-stu-id="29877-112">Description</span></span> |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="29877-113">Список</span><span class="sxs-lookup"><span data-stu-id="29877-113">List</span></span>](../api/organizationsettings-list-profilecardproperties.md) | [<span data-ttu-id="29877-114">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="29877-114">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="29877-115">Получите коллекцию ресурсов **profileCardProperty** организации.</span><span class="sxs-lookup"><span data-stu-id="29877-115">Get a collection of **profileCardProperty** resources of an organization.</span></span> |
| [<span data-ttu-id="29877-116">Создание</span><span class="sxs-lookup"><span data-stu-id="29877-116">Create</span></span>](../api/organizationsettings-post-profilecardproperties.md) | [<span data-ttu-id="29877-117">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="29877-117">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="29877-118">Создайте ресурс **profileCardProperty** для организации.</span><span class="sxs-lookup"><span data-stu-id="29877-118">Create a new **profileCardProperty** resource for an organization.</span></span> |
| [<span data-ttu-id="29877-119">Получение</span><span class="sxs-lookup"><span data-stu-id="29877-119">Get</span></span>](../api/profilecardproperty-get.md) | [<span data-ttu-id="29877-120">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="29877-120">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="29877-121">Прочитайте свойства и связи ресурса **profileCardProperty,** который содержит настройки карточки профиля, которые существуют в организации Microsoft 365 для заданного поля.</span><span class="sxs-lookup"><span data-stu-id="29877-121">Read the properties and relationships of a **profileCardProperty** resource, which contains the profile card customizations that exist in a Microsoft 365 organization for a given field.</span></span> |
| [<span data-ttu-id="29877-122">Обновление</span><span class="sxs-lookup"><span data-stu-id="29877-122">Update</span></span>](../api/profilecardproperty-update.md)               | [<span data-ttu-id="29877-123">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="29877-123">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="29877-124">Обновление объекта **profileCardProperty.**</span><span class="sxs-lookup"><span data-stu-id="29877-124">Update a **profileCardProperty** object.</span></span>                               |
| <span data-ttu-id="29877-125">[удаление](../api/profilecardproperty-delete.md);</span><span class="sxs-lookup"><span data-stu-id="29877-125">[Delete](../api/profilecardproperty-delete.md)</span></span>               | <span data-ttu-id="29877-126">Нет</span><span class="sxs-lookup"><span data-stu-id="29877-126">None</span></span>                                          | <span data-ttu-id="29877-127">Удаление объекта **profileCardProperty.**</span><span class="sxs-lookup"><span data-stu-id="29877-127">Delete a **profileCardProperty** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="29877-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="29877-128">Properties</span></span>

| <span data-ttu-id="29877-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="29877-129">Property</span></span>             | <span data-ttu-id="29877-130">Тип</span><span class="sxs-lookup"><span data-stu-id="29877-130">Type</span></span>                                                        | <span data-ttu-id="29877-131">Описание</span><span class="sxs-lookup"><span data-stu-id="29877-131">Description</span></span> |
|:---------------------|:------------------------------------------------------------|:------------|
|<span data-ttu-id="29877-132">аннотации</span><span class="sxs-lookup"><span data-stu-id="29877-132">annotations</span></span>           |<span data-ttu-id="29877-133">[Коллекция profileCardAnnotation](profilecardannotation.md)</span><span class="sxs-lookup"><span data-stu-id="29877-133">[profileCardAnnotation](profilecardannotation.md) collection</span></span> | <span data-ttu-id="29877-134">Позволяет администратору установить настраиваемую метку отображения для свойства каталога и локализовать ее для пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="29877-134">Allows an administrator to set a custom display label for the directory property and localize it for the users in their tenant.</span></span>|
|<span data-ttu-id="29877-135">directoryPropertyName</span><span class="sxs-lookup"><span data-stu-id="29877-135">directoryPropertyName</span></span> |<span data-ttu-id="29877-136">String</span><span class="sxs-lookup"><span data-stu-id="29877-136">String</span></span>                                                       | <span data-ttu-id="29877-137">Определяет ресурс **profileCardProperty** в операциях [Get,](../api/profilecardproperty-get.md) [Update](../api/profilecardproperty-update.md)и [Delete.](../api/profilecardproperty-delete.md)</span><span class="sxs-lookup"><span data-stu-id="29877-137">Identifies a **profileCardProperty** resource in [Get](../api/profilecardproperty-get.md), [Update](../api/profilecardproperty-update.md), or [Delete](../api/profilecardproperty-delete.md) operations.</span></span> <span data-ttu-id="29877-138">Позволяет администратору использовать скрытые свойства Azure Active Directory (Azure AD) в карточке профиля Microsoft 365 в клиенте.</span><span class="sxs-lookup"><span data-stu-id="29877-138">Allows an administrator to surface hidden Azure Active Directory (Azure AD) properties on the Microsoft 365 profile card within their tenant.</span></span> <span data-ttu-id="29877-139">Если заметен, поле Azure AD, на который ссылается это поле, будет видно всем пользователям в клиенте в области контактов карточки профиля.</span><span class="sxs-lookup"><span data-stu-id="29877-139">When present, the Azure AD field referenced in this field will be visible to all users in your tenant on the contact pane of the profile card.</span></span> <span data-ttu-id="29877-140">Допустимые значения для этого поля: , , , , `UserPrincipalName` , , `Fax` `StreetAddress` `PostalCode` `StateOrProvince` `Alias` `CustomAttribute1` , `CustomAttribute2` `CustomAttribute3` `CustomAttribute4` `CustomAttribute5` `CustomAttribute6` `CustomAttribute7` `CustomAttribute8` `CustomAttribute9` `CustomAttribute10` `CustomAttribute11` `CustomAttribute12` `CustomAttribute13` `CustomAttribute14` . `CustomAttribute15`</span><span class="sxs-lookup"><span data-stu-id="29877-140">Allowed values for this field are: `UserPrincipalName`, `Fax`, `StreetAddress`, `PostalCode`, `StateOrProvince`, `Alias`, `CustomAttribute1`,  `CustomAttribute2`, `CustomAttribute3`, `CustomAttribute4`, `CustomAttribute5`, `CustomAttribute6`, `CustomAttribute7`, `CustomAttribute8`, `CustomAttribute9`, `CustomAttribute10`, `CustomAttribute11`, `CustomAttribute12`, `CustomAttribute13`, `CustomAttribute14`, `CustomAttribute15`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="29877-141">Связи</span><span class="sxs-lookup"><span data-stu-id="29877-141">Relationships</span></span>

<span data-ttu-id="29877-142">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="29877-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="29877-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="29877-143">JSON representation</span></span>

<span data-ttu-id="29877-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29877-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardProperty"
}-->

```json
{
  "annotations": [
    {
      "displayName": "String",
      "localizations": [
        {
          "languageTag": "String",
          "displayName": "String"
        }
      ]
    }
  ],
  "directoryPropertyName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profileCardProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

