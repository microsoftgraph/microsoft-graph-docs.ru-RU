---
title: тип ресурса extensionProperty
description: Представляет расширение каталога
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 93b5c066895bcc3b8adc801bd7f8bf8283cc3535
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961988"
---
# <a name="extensionproperty-resource-type"></a><span data-ttu-id="9a346-103">тип ресурса extensionProperty</span><span class="sxs-lookup"><span data-stu-id="9a346-103">extensionProperty resource type</span></span>

<span data-ttu-id="9a346-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a346-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a346-105">Представляет расширение каталога, которое можно использовать для добавления настраиваемой свойства в объекты каталогов без необходимости хранения внешних данных.</span><span class="sxs-lookup"><span data-stu-id="9a346-105">Represents a directory extension that can be used to add a custom property to directory objects without requiring an external data store.</span></span> <span data-ttu-id="9a346-106">Например, если в организации есть приложение для бизнеса (LOB), для которого для каждого пользователя каталога требуется skype ID, Microsoft Graph можно использовать для регистрации нового свойства skypeId в объекте Пользователя каталога, а затем записываю значение для нового свойства для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9a346-106">For example, if an organization has a line of business (LOB) application that requires a Skype ID for each user in the directory, Microsoft Graph can be used to register a new property named skypeId on the directory’s User object, and then write a value to the new property for a specific user.</span></span>

<span data-ttu-id="9a346-107">Расширения могут быть добавлены к [ресурсам пользователей,](user.md) [групп,](group.md) [организаций,](organization.md) [устройств,](device.md) [приложений.](application.md)</span><span class="sxs-lookup"><span data-stu-id="9a346-107">Extensions can be added to [user](user.md), [group](group.md), [organization](organization.md), [device](device.md), [application](application.md) resources.</span></span> <span data-ttu-id="9a346-108">Только 100 значений  расширения для  всех типов и всех приложений можно написать на любой ресурс Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9a346-108">Only 100 extension values, across *all* types and *all* applications, can be written to any single Azure AD resource.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9a346-109">Описанные здесь расширения схем Azure AD доступны в Microsoft Graph только по причинам обратной совместимости.</span><span class="sxs-lookup"><span data-stu-id="9a346-109">Azure AD schema extensions described here are available in Microsoft Graph for backwards compatibility reasons only.</span></span>
> <span data-ttu-id="9a346-110">Это позволяет использовать Microsoft Graph для управления свойствами расширения, добавленными через Azure AD Graph или [Azure AD Connect.](/azure/active-directory/hybrid/whatis-azure-ad-connect)</span><span class="sxs-lookup"><span data-stu-id="9a346-110">It allows you to use Microsoft Graph to continue to manage extension properties added through Azure AD Graph or [Azure AD Connect](/azure/active-directory/hybrid/whatis-azure-ad-connect).</span></span>
> <span data-ttu-id="9a346-111">Для новых пользовательских расширений рекомендуется использовать расширения схемы Microsoft Graph для [добавления пользовательских данных в ресурсы.](/graph/extensibility-overview)</span><span class="sxs-lookup"><span data-stu-id="9a346-111">For new custom extensions, we recommend that you use Microsoft Graph schema extensions for [adding custom data to resources](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="9a346-112">Методы</span><span class="sxs-lookup"><span data-stu-id="9a346-112">Methods</span></span>

| <span data-ttu-id="9a346-113">Метод</span><span class="sxs-lookup"><span data-stu-id="9a346-113">Method</span></span>       | <span data-ttu-id="9a346-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9a346-114">Return Type</span></span> | <span data-ttu-id="9a346-115">Описание</span><span class="sxs-lookup"><span data-stu-id="9a346-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9a346-116">Создание расширения</span><span class="sxs-lookup"><span data-stu-id="9a346-116">Create extension</span></span>](../api/application-post-extensionproperty.md) | [<span data-ttu-id="9a346-117">extensionProperty</span><span class="sxs-lookup"><span data-stu-id="9a346-117">extensionProperty</span></span>](extensionProperty.md) | <span data-ttu-id="9a346-118">Создание свойства расширения для объекта application.</span><span class="sxs-lookup"><span data-stu-id="9a346-118">Create an extension property on an application object.</span></span> |
| [<span data-ttu-id="9a346-119">Список расширений</span><span class="sxs-lookup"><span data-stu-id="9a346-119">List extensions</span></span>](../api/application-list-extensionproperty.md) | <span data-ttu-id="9a346-120">Коллекция [extensionProperty](extensionProperty.md)</span><span class="sxs-lookup"><span data-stu-id="9a346-120">[extensionProperty](extensionProperty.md) collection</span></span> | <span data-ttu-id="9a346-121">Список свойств расширения для объекта application.</span><span class="sxs-lookup"><span data-stu-id="9a346-121">List extension properties on an application object.</span></span> |
| [<span data-ttu-id="9a346-122">Удаление расширения</span><span class="sxs-lookup"><span data-stu-id="9a346-122">Delete extension</span></span>](../api/application-delete-extensionproperty.md) | <span data-ttu-id="9a346-123">Нет</span><span class="sxs-lookup"><span data-stu-id="9a346-123">None</span></span> | <span data-ttu-id="9a346-124">Удаление свойства расширения объекта application.</span><span class="sxs-lookup"><span data-stu-id="9a346-124">Delete an extension property from an application object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9a346-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a346-125">Properties</span></span>

| <span data-ttu-id="9a346-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a346-126">Property</span></span>     | <span data-ttu-id="9a346-127">Тип</span><span class="sxs-lookup"><span data-stu-id="9a346-127">Type</span></span>        | <span data-ttu-id="9a346-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9a346-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9a346-129">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="9a346-129">appDisplayName</span></span>|<span data-ttu-id="9a346-130">String</span><span class="sxs-lookup"><span data-stu-id="9a346-130">String</span></span>| <span data-ttu-id="9a346-131">Отображение имени объекта приложения, на котором определено это свойство расширения.</span><span class="sxs-lookup"><span data-stu-id="9a346-131">Display name of the application object on which this extension property is defined.</span></span> <span data-ttu-id="9a346-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9a346-132">Read-only.</span></span> |
|<span data-ttu-id="9a346-133">dataType</span><span class="sxs-lookup"><span data-stu-id="9a346-133">dataType</span></span>|<span data-ttu-id="9a346-134">String</span><span class="sxs-lookup"><span data-stu-id="9a346-134">String</span></span>| <span data-ttu-id="9a346-135">Указывает тип данных значения, который может удерживать свойство расширения.</span><span class="sxs-lookup"><span data-stu-id="9a346-135">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="9a346-136">Поддерживаются следующие значения.</span><span class="sxs-lookup"><span data-stu-id="9a346-136">Following values are supported.</span></span> <span data-ttu-id="9a346-137">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="9a346-137">Not nullable.</span></span> <ul><li><span data-ttu-id="9a346-138">`Binary` - максимум 256 bytes</span><span class="sxs-lookup"><span data-stu-id="9a346-138">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="9a346-139">`DateTime` - Должен быть указан в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="9a346-139">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="9a346-140">Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="9a346-140">Will be stored in UTC.</span></span></li><li><span data-ttu-id="9a346-141">`Integer` - 32-битное значение.</span><span class="sxs-lookup"><span data-stu-id="9a346-141">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="9a346-142">`LargeInteger` - 64-битное значение.</span><span class="sxs-lookup"><span data-stu-id="9a346-142">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="9a346-143">`String` - максимум 256 символов</span><span class="sxs-lookup"><span data-stu-id="9a346-143">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="9a346-144">isSyncedFromOnPremises</span><span class="sxs-lookup"><span data-stu-id="9a346-144">isSyncedFromOnPremises</span></span>|<span data-ttu-id="9a346-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a346-145">Boolean</span></span>| <span data-ttu-id="9a346-146">Указывает, было ли это свойство расширения sycned из каталога onpremises с помощью Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9a346-146">Indicates if this extension property was sycned from onpremises directory using Azure AD Connect.</span></span> <span data-ttu-id="9a346-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9a346-147">Read-only.</span></span> |
|<span data-ttu-id="9a346-148">name</span><span class="sxs-lookup"><span data-stu-id="9a346-148">name</span></span>|<span data-ttu-id="9a346-149">String</span><span class="sxs-lookup"><span data-stu-id="9a346-149">String</span></span>| <span data-ttu-id="9a346-150">Имя свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="9a346-150">Name of the extension property.</span></span> <span data-ttu-id="9a346-151">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="9a346-151">Not nullable.</span></span> |
|<span data-ttu-id="9a346-152">targetObjects</span><span class="sxs-lookup"><span data-stu-id="9a346-152">targetObjects</span></span>|<span data-ttu-id="9a346-153">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9a346-153">String collection</span></span>| <span data-ttu-id="9a346-154">Поддерживаются следующие значения.</span><span class="sxs-lookup"><span data-stu-id="9a346-154">Following values are supported.</span></span> <span data-ttu-id="9a346-155">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="9a346-155">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a><span data-ttu-id="9a346-156">Связи</span><span class="sxs-lookup"><span data-stu-id="9a346-156">Relationships</span></span>

<span data-ttu-id="9a346-157">Нет</span><span class="sxs-lookup"><span data-stu-id="9a346-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a346-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a346-158">JSON representation</span></span>

<span data-ttu-id="9a346-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a346-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionProperty",
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
