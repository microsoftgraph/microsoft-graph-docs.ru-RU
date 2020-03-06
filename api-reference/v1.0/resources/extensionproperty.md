---
title: Тип ресурса Екстенсионпроперти
description: Представляет расширение каталога
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 065522e6fa13ffb89ac924c2600ede8f6a0e6f8d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531463"
---
# <a name="extensionproperty-resource-type"></a><span data-ttu-id="c53af-103">Тип ресурса Екстенсионпроперти</span><span class="sxs-lookup"><span data-stu-id="c53af-103">extensionProperty resource type</span></span>

<span data-ttu-id="c53af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c53af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c53af-105">Представляет расширение каталога, которое можно использовать для добавления настраиваемого свойства к объектам каталога без использования внешнего хранилища данных.</span><span class="sxs-lookup"><span data-stu-id="c53af-105">Represents a directory extension that can be used to add a custom property to directory objects without requiring an external data store.</span></span> <span data-ttu-id="c53af-106">Например, если в Организации есть бизнес-приложение, для которого требуется идентификатор Skype для каждого пользователя в каталоге, Microsoft Graph можно использовать для регистрации нового свойства с именем Скипеид в объекте пользователя каталога, а затем для записи значения в новое свойство. для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c53af-106">For example, if an organization has a line of business (LOB) application that requires a Skype ID for each user in the directory, Microsoft Graph can be used to register a new property named skypeId on the directory’s User object, and then write a value to the new property for a specific user.</span></span>

<span data-ttu-id="c53af-107">Расширения можно добавлять в ресурсы " [пользователь](user.md)", " [Группа](group.md)", " [Организация](organization.md)", " [устройство](device.md)" и "ресурсы [приложения](application.md) ".</span><span class="sxs-lookup"><span data-stu-id="c53af-107">Extensions can be added to [user](user.md), [group](group.md), [organization](organization.md), [device](device.md), [application](application.md) resources.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c53af-108">Расширения схемы Azure AD, описанные в этой статье, доступны только в целях обеспечения обратной совместимости в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c53af-108">Azure AD schema extensions described here are available in Microsoft Graph for backwards compatibility reasons only.</span></span>
> <span data-ttu-id="c53af-109">Он позволяет использовать Microsoft Graph, чтобы продолжить управление свойствами расширения, добавленными через Azure AD Graph или [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect).</span><span class="sxs-lookup"><span data-stu-id="c53af-109">It allows you to use Microsoft Graph to continue to manage extension properties added through Azure AD Graph or [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect).</span></span>
> <span data-ttu-id="c53af-110">Для новых настраиваемых расширений рекомендуется использовать расширения схемы Microsoft Graph для [добавления пользовательских данных в ресурсы](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="c53af-110">For new custom extensions, we recommend that you use Microsoft Graph schema extensions for [adding custom data to resources](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="c53af-111">Методы</span><span class="sxs-lookup"><span data-stu-id="c53af-111">Methods</span></span>

| <span data-ttu-id="c53af-112">Метод</span><span class="sxs-lookup"><span data-stu-id="c53af-112">Method</span></span>       | <span data-ttu-id="c53af-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c53af-113">Return Type</span></span> | <span data-ttu-id="c53af-114">Описание</span><span class="sxs-lookup"><span data-stu-id="c53af-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c53af-115">Создание расширения</span><span class="sxs-lookup"><span data-stu-id="c53af-115">Create extension</span></span>](../api/application-post-extensionproperty.md) | [<span data-ttu-id="c53af-116">extensionProperty</span><span class="sxs-lookup"><span data-stu-id="c53af-116">extensionProperty</span></span>](extensionProperty.md) | <span data-ttu-id="c53af-117">Создание свойства расширения для объекта application.</span><span class="sxs-lookup"><span data-stu-id="c53af-117">Create an extension property on an application object.</span></span> |
| [<span data-ttu-id="c53af-118">Список расширений</span><span class="sxs-lookup"><span data-stu-id="c53af-118">List extensions</span></span>](../api/application-list-extensionproperty.md) | <span data-ttu-id="c53af-119">Коллекция [extensionProperty](extensionProperty.md)</span><span class="sxs-lookup"><span data-stu-id="c53af-119">[extensionProperty](extensionProperty.md) collection</span></span> | <span data-ttu-id="c53af-120">Список свойств расширения для объекта application.</span><span class="sxs-lookup"><span data-stu-id="c53af-120">List extension properties on an application object.</span></span> |
| [<span data-ttu-id="c53af-121">Удаление расширения</span><span class="sxs-lookup"><span data-stu-id="c53af-121">Delete extension</span></span>](../api/application-delete-extensionproperty.md) | <span data-ttu-id="c53af-122">Нет</span><span class="sxs-lookup"><span data-stu-id="c53af-122">None</span></span> | <span data-ttu-id="c53af-123">Удаление свойства расширения объекта application.</span><span class="sxs-lookup"><span data-stu-id="c53af-123">Delete an extension property from an application object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c53af-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="c53af-124">Properties</span></span>

| <span data-ttu-id="c53af-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="c53af-125">Property</span></span>     | <span data-ttu-id="c53af-126">Тип</span><span class="sxs-lookup"><span data-stu-id="c53af-126">Type</span></span>        | <span data-ttu-id="c53af-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c53af-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c53af-128">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="c53af-128">appDisplayName</span></span>|<span data-ttu-id="c53af-129">String</span><span class="sxs-lookup"><span data-stu-id="c53af-129">String</span></span>| <span data-ttu-id="c53af-130">Отображаемое имя объекта приложения, для которого определено это свойство расширения.</span><span class="sxs-lookup"><span data-stu-id="c53af-130">Display name of the application object on which this extension property is defined.</span></span> <span data-ttu-id="c53af-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c53af-131">Read-only.</span></span> |
|<span data-ttu-id="c53af-132">dataType</span><span class="sxs-lookup"><span data-stu-id="c53af-132">dataType</span></span>|<span data-ttu-id="c53af-133">String</span><span class="sxs-lookup"><span data-stu-id="c53af-133">String</span></span>| <span data-ttu-id="c53af-134">Задает тип данных значения, которое может содержать свойство Extension.</span><span class="sxs-lookup"><span data-stu-id="c53af-134">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="c53af-135">Поддерживаются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="c53af-135">Following values are supported.</span></span> <span data-ttu-id="c53af-136">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c53af-136">Not nullable.</span></span> <ul><li><span data-ttu-id="c53af-137">`Binary`– 256 байт (максимум)</span><span class="sxs-lookup"><span data-stu-id="c53af-137">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="c53af-138">`DateTime`-Должен быть указан в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="c53af-138">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="c53af-139">Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c53af-139">Will be stored in UTC.</span></span></li><li><span data-ttu-id="c53af-140">`Integer`— значение 32 — бит.</span><span class="sxs-lookup"><span data-stu-id="c53af-140">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="c53af-141">`LargeInteger`— значение 64 — бит.</span><span class="sxs-lookup"><span data-stu-id="c53af-141">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="c53af-142">`String`– 256 символов максимум</span><span class="sxs-lookup"><span data-stu-id="c53af-142">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="c53af-143">иссинцедфромонпремисес</span><span class="sxs-lookup"><span data-stu-id="c53af-143">isSyncedFromOnPremises</span></span>|<span data-ttu-id="c53af-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="c53af-144">Boolean</span></span>| <span data-ttu-id="c53af-145">Указывает, было ли это свойство расширения сикнед из локального каталога с помощью Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="c53af-145">Indicates if this extension property was sycned from onpremises directory using Azure AD Connect.</span></span> <span data-ttu-id="c53af-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c53af-146">Read-only.</span></span> |
|<span data-ttu-id="c53af-147">name</span><span class="sxs-lookup"><span data-stu-id="c53af-147">name</span></span>|<span data-ttu-id="c53af-148">Строка</span><span class="sxs-lookup"><span data-stu-id="c53af-148">String</span></span>| <span data-ttu-id="c53af-149">Имя свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="c53af-149">Name of the extension property.</span></span> <span data-ttu-id="c53af-150">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c53af-150">Not nullable.</span></span> |
|<span data-ttu-id="c53af-151">таржетобжектс</span><span class="sxs-lookup"><span data-stu-id="c53af-151">targetObjects</span></span>|<span data-ttu-id="c53af-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c53af-152">String collection</span></span>| <span data-ttu-id="c53af-153">Поддерживаются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="c53af-153">Following values are supported.</span></span> <span data-ttu-id="c53af-154">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c53af-154">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a><span data-ttu-id="c53af-155">Связи</span><span class="sxs-lookup"><span data-stu-id="c53af-155">Relationships</span></span>

<span data-ttu-id="c53af-156">Нет</span><span class="sxs-lookup"><span data-stu-id="c53af-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c53af-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c53af-157">JSON representation</span></span>

<span data-ttu-id="c53af-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c53af-158">The following is a JSON representation of the resource.</span></span>

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
