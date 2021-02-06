---
title: Тип ресурса extensionProperty
description: Представляет расширение каталога
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f71ec6da3013b6d0bda0edec8d6a47b30de84546
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129480"
---
# <a name="extensionproperty-resource-type"></a><span data-ttu-id="879f6-103">Тип ресурса extensionProperty</span><span class="sxs-lookup"><span data-stu-id="879f6-103">extensionProperty resource type</span></span>

<span data-ttu-id="879f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="879f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="879f6-105">Представляет расширение каталога, которое можно использовать для добавления настраиваемой свойства в объекты каталогов без необходимости хранения внешних данных.</span><span class="sxs-lookup"><span data-stu-id="879f6-105">Represents a directory extension that can be used to add a custom property to directory objects without requiring an external data store.</span></span> <span data-ttu-id="879f6-106">Например, если в организации есть бизнес-приложение, для которого требуется ИД Skype для каждого пользователя в каталоге, Microsoft Graph можно использовать для регистрации нового свойства skypeId в объекте User каталога, а затем записи значения в новое свойство для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="879f6-106">For example, if an organization has a line of business (LOB) application that requires a Skype ID for each user in the directory, Microsoft Graph can be used to register a new property named skypeId on the directory’s User object, and then write a value to the new property for a specific user.</span></span>

<span data-ttu-id="879f6-107">Расширения можно добавлять в ресурсы [пользователей,](user.md) [групп,](group.md) [организаций,](organization.md) [устройств,](device.md) [приложений.](application.md)</span><span class="sxs-lookup"><span data-stu-id="879f6-107">Extensions can be added to [user](user.md), [group](group.md), [organization](organization.md), [device](device.md), [application](application.md) resources.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="879f6-108">Описанные здесь расширения схемы Azure AD доступны в Microsoft Graph только из соображений обратной совместимости.</span><span class="sxs-lookup"><span data-stu-id="879f6-108">Azure AD schema extensions described here are available in Microsoft Graph for backwards compatibility reasons only.</span></span>
> <span data-ttu-id="879f6-109">Это позволяет использовать Microsoft Graph для управления свойствами расширений, добавленными через Azure AD Graph или [Azure AD Connect.](/azure/active-directory/hybrid/whatis-azure-ad-connect)</span><span class="sxs-lookup"><span data-stu-id="879f6-109">It allows you to use Microsoft Graph to continue to manage extension properties added through Azure AD Graph or [Azure AD Connect](/azure/active-directory/hybrid/whatis-azure-ad-connect).</span></span>
> <span data-ttu-id="879f6-110">Для новых пользовательских расширений рекомендуется использовать расширения схемы Microsoft Graph для добавления пользовательских [данных в ресурсы.](/graph/extensibility-overview)</span><span class="sxs-lookup"><span data-stu-id="879f6-110">For new custom extensions, we recommend that you use Microsoft Graph schema extensions for [adding custom data to resources](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="879f6-111">Методы</span><span class="sxs-lookup"><span data-stu-id="879f6-111">Methods</span></span>

| <span data-ttu-id="879f6-112">Метод</span><span class="sxs-lookup"><span data-stu-id="879f6-112">Method</span></span>       | <span data-ttu-id="879f6-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="879f6-113">Return Type</span></span> | <span data-ttu-id="879f6-114">Описание</span><span class="sxs-lookup"><span data-stu-id="879f6-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="879f6-115">Список расширений</span><span class="sxs-lookup"><span data-stu-id="879f6-115">List extensions</span></span>](../api/application-list-extensionproperty.md) | <span data-ttu-id="879f6-116">Коллекция [extensionProperty](extensionProperty.md)</span><span class="sxs-lookup"><span data-stu-id="879f6-116">[extensionProperty](extensionProperty.md) collection</span></span> | <span data-ttu-id="879f6-117">Список свойств расширения для объекта application.</span><span class="sxs-lookup"><span data-stu-id="879f6-117">List extension properties on an application object.</span></span> |
| [<span data-ttu-id="879f6-118">Создание расширения</span><span class="sxs-lookup"><span data-stu-id="879f6-118">Create extension</span></span>](../api/application-post-extensionproperty.md) | [<span data-ttu-id="879f6-119">extensionProperty</span><span class="sxs-lookup"><span data-stu-id="879f6-119">extensionProperty</span></span>](extensionProperty.md) | <span data-ttu-id="879f6-120">Создание свойства расширения для объекта application.</span><span class="sxs-lookup"><span data-stu-id="879f6-120">Create an extension property on an application object.</span></span> |
| [<span data-ttu-id="879f6-121">Удаление расширения</span><span class="sxs-lookup"><span data-stu-id="879f6-121">Delete extension</span></span>](../api/application-delete-extensionproperty.md) | <span data-ttu-id="879f6-122">Нет</span><span class="sxs-lookup"><span data-stu-id="879f6-122">None</span></span> | <span data-ttu-id="879f6-123">Удаление свойства расширения объекта application.</span><span class="sxs-lookup"><span data-stu-id="879f6-123">Delete an extension property from an application object.</span></span> |

## <a name="properties"></a><span data-ttu-id="879f6-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="879f6-124">Properties</span></span>

| <span data-ttu-id="879f6-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="879f6-125">Property</span></span>     | <span data-ttu-id="879f6-126">Тип</span><span class="sxs-lookup"><span data-stu-id="879f6-126">Type</span></span>        | <span data-ttu-id="879f6-127">Описание</span><span class="sxs-lookup"><span data-stu-id="879f6-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="879f6-128">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="879f6-128">appDisplayName</span></span>|<span data-ttu-id="879f6-129">String</span><span class="sxs-lookup"><span data-stu-id="879f6-129">String</span></span>| <span data-ttu-id="879f6-130">Отображает имя объекта приложения, в котором определено это свойство расширения.</span><span class="sxs-lookup"><span data-stu-id="879f6-130">Display name of the application object on which this extension property is defined.</span></span> <span data-ttu-id="879f6-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="879f6-131">Read-only.</span></span> |
|<span data-ttu-id="879f6-132">dataType</span><span class="sxs-lookup"><span data-stu-id="879f6-132">dataType</span></span>|<span data-ttu-id="879f6-133">String</span><span class="sxs-lookup"><span data-stu-id="879f6-133">String</span></span>| <span data-ttu-id="879f6-134">Указывает тип данных значения, который может быть в свойстве расширения.</span><span class="sxs-lookup"><span data-stu-id="879f6-134">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="879f6-135">Поддерживаются следующие значения.</span><span class="sxs-lookup"><span data-stu-id="879f6-135">Following values are supported.</span></span> <span data-ttu-id="879f6-136">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="879f6-136">Not nullable.</span></span> <ul><li><span data-ttu-id="879f6-137">`Binary` - Не более 256байт</span><span class="sxs-lookup"><span data-stu-id="879f6-137">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="879f6-138">`DateTime` - Должен быть указан в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="879f6-138">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="879f6-139">Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="879f6-139">Will be stored in UTC.</span></span></li><li><span data-ttu-id="879f6-140">`Integer` - 32-битное значение.</span><span class="sxs-lookup"><span data-stu-id="879f6-140">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="879f6-141">`LargeInteger` - 64-битное значение.</span><span class="sxs-lookup"><span data-stu-id="879f6-141">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="879f6-142">`String` — не более 256 символов</span><span class="sxs-lookup"><span data-stu-id="879f6-142">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="879f6-143">isSyncedFromOnPremises</span><span class="sxs-lookup"><span data-stu-id="879f6-143">isSyncedFromOnPremises</span></span>|<span data-ttu-id="879f6-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="879f6-144">Boolean</span></span>| <span data-ttu-id="879f6-145">Указывает, было ли это свойство расширения sycned из каталога onpremises с помощью Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="879f6-145">Indicates if this extension property was sycned from onpremises directory using Azure AD Connect.</span></span> <span data-ttu-id="879f6-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="879f6-146">Read-only.</span></span> |
|<span data-ttu-id="879f6-147">name</span><span class="sxs-lookup"><span data-stu-id="879f6-147">name</span></span>|<span data-ttu-id="879f6-148">String</span><span class="sxs-lookup"><span data-stu-id="879f6-148">String</span></span>| <span data-ttu-id="879f6-149">Имя свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="879f6-149">Name of the extension property.</span></span> <span data-ttu-id="879f6-150">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="879f6-150">Not nullable.</span></span> |
|<span data-ttu-id="879f6-151">targetObjects</span><span class="sxs-lookup"><span data-stu-id="879f6-151">targetObjects</span></span>|<span data-ttu-id="879f6-152">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="879f6-152">String collection</span></span>| <span data-ttu-id="879f6-153">Поддерживаются следующие значения.</span><span class="sxs-lookup"><span data-stu-id="879f6-153">Following values are supported.</span></span> <span data-ttu-id="879f6-154">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="879f6-154">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a><span data-ttu-id="879f6-155">Связи</span><span class="sxs-lookup"><span data-stu-id="879f6-155">Relationships</span></span>

<span data-ttu-id="879f6-156">Нет</span><span class="sxs-lookup"><span data-stu-id="879f6-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="879f6-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="879f6-157">JSON representation</span></span>

<span data-ttu-id="879f6-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="879f6-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionProperty",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "appDisplayName": "String",
  "dataType": "String",
  "isSyncedFromOnPremises": true,
  "name": "String",
  "targetObjects": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
