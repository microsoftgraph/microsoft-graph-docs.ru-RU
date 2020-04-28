---
title: Тип ресурса Екстенсионпроперти
description: Представляет расширение каталога
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3d6f6e89ca6e54e1c74e43c6201766aa199f454d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43423799"
---
# <a name="extensionproperty-resource-type"></a><span data-ttu-id="5fcb7-103">Тип ресурса Екстенсионпроперти</span><span class="sxs-lookup"><span data-stu-id="5fcb7-103">extensionProperty resource type</span></span>

<span data-ttu-id="5fcb7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fcb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fcb7-105">Представляет расширение каталога, которое можно использовать для добавления настраиваемого свойства к объектам каталога без использования внешнего хранилища данных.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-105">Represents a directory extension that can be used to add a custom property to directory objects without requiring an external data store.</span></span> <span data-ttu-id="5fcb7-106">Например, если в Организации есть бизнес-приложение, для которого требуется идентификатор Skype для каждого пользователя в каталоге, Microsoft Graph можно использовать для регистрации нового свойства с именем Скипеид в объекте пользователя каталога, а затем для записи значения в новое свойство для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-106">For example, if an organization has a line of business (LOB) application that requires a Skype ID for each user in the directory, Microsoft Graph can be used to register a new property named skypeId on the directory’s User object, and then write a value to the new property for a specific user.</span></span>

<span data-ttu-id="5fcb7-107">Расширения можно добавлять в ресурсы " [пользователь](user.md)", " [Группа](group.md)", " [Организация](organization.md)", " [устройство](device.md)" и "ресурсы [приложения](application.md) ".</span><span class="sxs-lookup"><span data-stu-id="5fcb7-107">Extensions can be added to [user](user.md), [group](group.md), [organization](organization.md), [device](device.md), [application](application.md) resources.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5fcb7-108">Расширения схемы Azure AD, описанные в этой статье, доступны только в целях обеспечения обратной совместимости в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-108">Azure AD schema extensions described here are available in Microsoft Graph for backwards compatibility reasons only.</span></span>
> <span data-ttu-id="5fcb7-109">Он позволяет использовать Microsoft Graph, чтобы продолжить управление свойствами расширения, добавленными через Azure AD Graph или [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect).</span><span class="sxs-lookup"><span data-stu-id="5fcb7-109">It allows you to use Microsoft Graph to continue to manage extension properties added through Azure AD Graph or [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect).</span></span>
> <span data-ttu-id="5fcb7-110">Для новых настраиваемых расширений рекомендуется использовать расширения схемы Microsoft Graph для [добавления пользовательских данных в ресурсы](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="5fcb7-110">For new custom extensions, we recommend that you use Microsoft Graph schema extensions for [adding custom data to resources](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="5fcb7-111">Методы</span><span class="sxs-lookup"><span data-stu-id="5fcb7-111">Methods</span></span>

| <span data-ttu-id="5fcb7-112">Метод</span><span class="sxs-lookup"><span data-stu-id="5fcb7-112">Method</span></span>       | <span data-ttu-id="5fcb7-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5fcb7-113">Return Type</span></span> | <span data-ttu-id="5fcb7-114">Описание</span><span class="sxs-lookup"><span data-stu-id="5fcb7-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5fcb7-115">Список расширений</span><span class="sxs-lookup"><span data-stu-id="5fcb7-115">List extensions</span></span>](../api/application-list-extensionproperty.md) | <span data-ttu-id="5fcb7-116">Коллекция [extensionProperty](extensionProperty.md)</span><span class="sxs-lookup"><span data-stu-id="5fcb7-116">[extensionProperty](extensionProperty.md) collection</span></span> | <span data-ttu-id="5fcb7-117">Список свойств расширения для объекта application.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-117">List extension properties on an application object.</span></span> |
| [<span data-ttu-id="5fcb7-118">Создание расширения</span><span class="sxs-lookup"><span data-stu-id="5fcb7-118">Create extension</span></span>](../api/application-post-extensionproperty.md) | [<span data-ttu-id="5fcb7-119">extensionProperty</span><span class="sxs-lookup"><span data-stu-id="5fcb7-119">extensionProperty</span></span>](extensionProperty.md) | <span data-ttu-id="5fcb7-120">Создание свойства расширения для объекта application.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-120">Create an extension property on an application object.</span></span> |
| [<span data-ttu-id="5fcb7-121">Удаление расширения</span><span class="sxs-lookup"><span data-stu-id="5fcb7-121">Delete extension</span></span>](../api/application-delete-extensionproperty.md) | <span data-ttu-id="5fcb7-122">Нет</span><span class="sxs-lookup"><span data-stu-id="5fcb7-122">None</span></span> | <span data-ttu-id="5fcb7-123">Удаление свойства расширения объекта application.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-123">Delete an extension property from an application object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5fcb7-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="5fcb7-124">Properties</span></span>

| <span data-ttu-id="5fcb7-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fcb7-125">Property</span></span>     | <span data-ttu-id="5fcb7-126">Тип</span><span class="sxs-lookup"><span data-stu-id="5fcb7-126">Type</span></span>        | <span data-ttu-id="5fcb7-127">Описание</span><span class="sxs-lookup"><span data-stu-id="5fcb7-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5fcb7-128">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="5fcb7-128">appDisplayName</span></span>|<span data-ttu-id="5fcb7-129">String</span><span class="sxs-lookup"><span data-stu-id="5fcb7-129">String</span></span>| <span data-ttu-id="5fcb7-130">Отображаемое имя объекта приложения, для которого определено это свойство расширения.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-130">Display name of the application object on which this extension property is defined.</span></span> <span data-ttu-id="5fcb7-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-131">Read-only.</span></span> |
|<span data-ttu-id="5fcb7-132">dataType</span><span class="sxs-lookup"><span data-stu-id="5fcb7-132">dataType</span></span>|<span data-ttu-id="5fcb7-133">String</span><span class="sxs-lookup"><span data-stu-id="5fcb7-133">String</span></span>| <span data-ttu-id="5fcb7-134">Задает тип данных значения, которое может содержать свойство Extension.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-134">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="5fcb7-135">Поддерживаются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="5fcb7-135">Following values are supported.</span></span> <span data-ttu-id="5fcb7-136">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-136">Not nullable.</span></span> <ul><li><span data-ttu-id="5fcb7-137">`Binary`– 256 байт (максимум)</span><span class="sxs-lookup"><span data-stu-id="5fcb7-137">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="5fcb7-138">`DateTime`-Должен быть указан в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-138">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="5fcb7-139">Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-139">Will be stored in UTC.</span></span></li><li><span data-ttu-id="5fcb7-140">`Integer`— значение 32 — бит.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-140">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="5fcb7-141">`LargeInteger`— значение 64 — бит.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-141">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="5fcb7-142">`String`– 256 символов максимум</span><span class="sxs-lookup"><span data-stu-id="5fcb7-142">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="5fcb7-143">иссинцедфромонпремисес</span><span class="sxs-lookup"><span data-stu-id="5fcb7-143">isSyncedFromOnPremises</span></span>|<span data-ttu-id="5fcb7-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="5fcb7-144">Boolean</span></span>| <span data-ttu-id="5fcb7-145">Указывает, было ли это свойство расширения сикнед из локального каталога с помощью Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-145">Indicates if this extension property was sycned from onpremises directory using Azure AD Connect.</span></span> <span data-ttu-id="5fcb7-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-146">Read-only.</span></span> |
|<span data-ttu-id="5fcb7-147">name</span><span class="sxs-lookup"><span data-stu-id="5fcb7-147">name</span></span>|<span data-ttu-id="5fcb7-148">Строка</span><span class="sxs-lookup"><span data-stu-id="5fcb7-148">String</span></span>| <span data-ttu-id="5fcb7-149">Имя свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-149">Name of the extension property.</span></span> <span data-ttu-id="5fcb7-150">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-150">Not nullable.</span></span> |
|<span data-ttu-id="5fcb7-151">таржетобжектс</span><span class="sxs-lookup"><span data-stu-id="5fcb7-151">targetObjects</span></span>|<span data-ttu-id="5fcb7-152">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="5fcb7-152">String collection</span></span>| <span data-ttu-id="5fcb7-153">Поддерживаются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="5fcb7-153">Following values are supported.</span></span> <span data-ttu-id="5fcb7-154">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-154">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a><span data-ttu-id="5fcb7-155">Связи</span><span class="sxs-lookup"><span data-stu-id="5fcb7-155">Relationships</span></span>

<span data-ttu-id="5fcb7-156">Нет</span><span class="sxs-lookup"><span data-stu-id="5fcb7-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5fcb7-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5fcb7-157">JSON representation</span></span>

<span data-ttu-id="5fcb7-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fcb7-158">The following is a JSON representation of the resource.</span></span>

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
