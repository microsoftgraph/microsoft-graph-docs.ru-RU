---
title: Тип ресурса Профилекардпроперти
description: Используется для обозначения нового свойства для общего доступа, для людей или для пользователя, к которому будет применено пользовательское отображаемое имя или Аннотация. Администратор может определить строку отображаемого имени по умолчанию и набор альтернативных переводов для языков, которые они поддерживают в Организации.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 036b9c84bda2a30e00206194768c621f127a4d75
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183675"
---
# <a name="profilecardproperty-resource-type"></a><span data-ttu-id="34a65-104">Тип ресурса Профилекардпроперти</span><span class="sxs-lookup"><span data-stu-id="34a65-104">profileCardProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34a65-105">Представляет атрибут пользователя в карточке профиля Microsoft 365, который Организация будет использовать совместно с другими пользователями.</span><span class="sxs-lookup"><span data-stu-id="34a65-105">Represents an attribute of a user on the Microsoft 365 profile card for an organization to surface in a shared, people experience.</span></span>

<span data-ttu-id="34a65-106">Атрибут может быть встроенным атрибутом Azure Active Directory (Azure AD), таким как `Alias` OR `UserPrincipalName` , или может быть настраиваемым атрибутом.</span><span class="sxs-lookup"><span data-stu-id="34a65-106">The attribute can be an Azure Active Directory (Azure AD) built-in attribute, such as `Alias` or `UserPrincipalName`, or it can be a custom attribute.</span></span> <span data-ttu-id="34a65-107">Для настраиваемого атрибута администратор может определить `en-us` строку отображаемого имени по умолчанию и набор альтернативных переводов для языков, поддерживаемых в Организации.</span><span class="sxs-lookup"><span data-stu-id="34a65-107">For a custom attribute, an administrator can define an `en-us` default display name string and a set of alternative translations for the languages that they support in their organization.</span></span>

<span data-ttu-id="34a65-108">Дополнительные сведения о добавлении свойств в карточку профиля для организации можно узнать в статье [Настройка карточки профиля](/graph/add-properties-profilecard).</span><span class="sxs-lookup"><span data-stu-id="34a65-108">For more information on adding properties to the profile card for an organization, see [customize the profile card](/graph/add-properties-profilecard).</span></span>

## <a name="methods"></a><span data-ttu-id="34a65-109">Методы</span><span class="sxs-lookup"><span data-stu-id="34a65-109">Methods</span></span>

| <span data-ttu-id="34a65-110">Метод</span><span class="sxs-lookup"><span data-stu-id="34a65-110">Method</span></span>       | <span data-ttu-id="34a65-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="34a65-111">Return Type</span></span> | <span data-ttu-id="34a65-112">Описание</span><span class="sxs-lookup"><span data-stu-id="34a65-112">Description</span></span> |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="34a65-113">Список</span><span class="sxs-lookup"><span data-stu-id="34a65-113">List</span></span>](../api/organizationsettings-list-profilecardproperties.md) | [<span data-ttu-id="34a65-114">профилекардпроперти</span><span class="sxs-lookup"><span data-stu-id="34a65-114">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="34a65-115">Получение коллекции ресурсов **профилекардпроперти** Организации.</span><span class="sxs-lookup"><span data-stu-id="34a65-115">Get a collection of **profileCardProperty** resources of an organization.</span></span> |
| <span data-ttu-id="34a65-116">[создание](../api/organizationsettings-post-profilecardproperties.md);</span><span class="sxs-lookup"><span data-stu-id="34a65-116">[Create](../api/organizationsettings-post-profilecardproperties.md)</span></span> | [<span data-ttu-id="34a65-117">профилекардпроперти</span><span class="sxs-lookup"><span data-stu-id="34a65-117">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="34a65-118">Создайте новый ресурс **профилекардпроперти** для Организации.</span><span class="sxs-lookup"><span data-stu-id="34a65-118">Create a new **profileCardProperty** resource for an organization.</span></span> |
| <span data-ttu-id="34a65-119">[получение](../api/profilecardproperty-get.md);</span><span class="sxs-lookup"><span data-stu-id="34a65-119">[Get](../api/profilecardproperty-get.md)</span></span> | [<span data-ttu-id="34a65-120">профилекардпроперти</span><span class="sxs-lookup"><span data-stu-id="34a65-120">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="34a65-121">Прочитайте свойства и связи ресурса **профилекардпроперти** , в котором содержатся настройки карты профилей, существующие в организации Microsoft 365 для данного поля.</span><span class="sxs-lookup"><span data-stu-id="34a65-121">Read the properties and relationships of a **profileCardProperty** resource, which contains the profile card customizations that exist in a Microsoft 365 organization for a given field.</span></span> |
| <span data-ttu-id="34a65-122">[обновление](../api/profilecardproperty-update.md).</span><span class="sxs-lookup"><span data-stu-id="34a65-122">[Update](../api/profilecardproperty-update.md)</span></span>               | [<span data-ttu-id="34a65-123">профилекардпроперти</span><span class="sxs-lookup"><span data-stu-id="34a65-123">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="34a65-124">Обновление объекта **профилекардпроперти** .</span><span class="sxs-lookup"><span data-stu-id="34a65-124">Update a **profileCardProperty** object.</span></span>                               |
| <span data-ttu-id="34a65-125">[удаление](../api/profilecardproperty-delete.md);</span><span class="sxs-lookup"><span data-stu-id="34a65-125">[Delete](../api/profilecardproperty-delete.md)</span></span>               | <span data-ttu-id="34a65-126">Нет</span><span class="sxs-lookup"><span data-stu-id="34a65-126">None</span></span>                                          | <span data-ttu-id="34a65-127">Удаление объекта **профилекардпроперти** .</span><span class="sxs-lookup"><span data-stu-id="34a65-127">Delete a **profileCardProperty** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="34a65-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="34a65-128">Properties</span></span>

| <span data-ttu-id="34a65-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="34a65-129">Property</span></span>             | <span data-ttu-id="34a65-130">Тип</span><span class="sxs-lookup"><span data-stu-id="34a65-130">Type</span></span>                                                        | <span data-ttu-id="34a65-131">Описание</span><span class="sxs-lookup"><span data-stu-id="34a65-131">Description</span></span> |
|:---------------------|:------------------------------------------------------------|:------------|
|<span data-ttu-id="34a65-132">Комментарии</span><span class="sxs-lookup"><span data-stu-id="34a65-132">annotations</span></span>           |<span data-ttu-id="34a65-133">Коллекция [профилекарданнотатион](profilecardannotation.md)</span><span class="sxs-lookup"><span data-stu-id="34a65-133">[profileCardAnnotation](profilecardannotation.md) collection</span></span> | <span data-ttu-id="34a65-134">Позволяет администратору задать настраиваемую метку отображения для свойства каталога и локализовать ее для пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="34a65-134">Allows an administrator to set a custom display label for the directory property and localize it for the users in their tenant.</span></span>|
|<span data-ttu-id="34a65-135">директорипропертинаме</span><span class="sxs-lookup"><span data-stu-id="34a65-135">directoryPropertyName</span></span> |<span data-ttu-id="34a65-136">String</span><span class="sxs-lookup"><span data-stu-id="34a65-136">String</span></span>                                                       | <span data-ttu-id="34a65-137">Определяет ресурс **профилекардпроперти** в операциях [Get](../api/profilecardproperty-get.md), [Update](../api/profilecardproperty-update.md)или [Delete](../api/profilecardproperty-delete.md) .</span><span class="sxs-lookup"><span data-stu-id="34a65-137">Identifies a **profileCardProperty** resource in [Get](../api/profilecardproperty-get.md), [Update](../api/profilecardproperty-update.md), or [Delete](../api/profilecardproperty-delete.md) operations.</span></span> <span data-ttu-id="34a65-138">Позволяет администратору показывать скрытые свойства Azure Active Directory (Azure AD) на карте профиля Microsoft 365 в своем клиенте.</span><span class="sxs-lookup"><span data-stu-id="34a65-138">Allows an administrator to surface hidden Azure Active Directory (Azure AD) properties on the Microsoft 365 profile card within their tenant.</span></span> <span data-ttu-id="34a65-139">Если этот параметр указан, поле Azure AD, указанное в этом поле, будет отображаться для всех пользователей в клиенте в области контактов карточки профиля.</span><span class="sxs-lookup"><span data-stu-id="34a65-139">When present, the Azure AD field referenced in this field will be visible to all users in your tenant on the contact pane of the profile card.</span></span> <span data-ttu-id="34a65-140">Допустимые значения для этого поля:,,,,,,,,,,,,,,,, `UserPrincipalName` `Fax` `StreetAddress` ,, `PostalCode` `StateOrProvince` `Alias` `CustomAttribute1` `CustomAttribute2` `CustomAttribute3` `CustomAttribute4` `CustomAttribute5` `CustomAttribute6` `CustomAttribute7` , `CustomAttribute8` , `CustomAttribute9` `CustomAttribute10` `CustomAttribute11` `CustomAttribute12` `CustomAttribute13` `CustomAttribute14` `CustomAttribute15` ,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="34a65-140">Allowed values for this field are: `UserPrincipalName`, `Fax`, `StreetAddress`, `PostalCode`, `StateOrProvince`, `Alias`, `CustomAttribute1`,  `CustomAttribute2`, `CustomAttribute3`, `CustomAttribute4`, `CustomAttribute5`, `CustomAttribute6`, `CustomAttribute7`, `CustomAttribute8`, `CustomAttribute9`, `CustomAttribute10`, `CustomAttribute11`, `CustomAttribute12`, `CustomAttribute13`, `CustomAttribute14`, `CustomAttribute15`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="34a65-141">Связи</span><span class="sxs-lookup"><span data-stu-id="34a65-141">Relationships</span></span>

<span data-ttu-id="34a65-142">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="34a65-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="34a65-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="34a65-143">JSON representation</span></span>

<span data-ttu-id="34a65-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34a65-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardProperty",
  "baseType": ""
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