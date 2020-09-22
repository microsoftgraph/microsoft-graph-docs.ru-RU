---
title: Тип ресурса Екстенсионпроперти
description: Представляет расширение каталога
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e49d72a5231980fef906d70e92623a70bb308e8a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026943"
---
# <a name="extensionproperty-resource-type"></a><span data-ttu-id="bf4ae-103">Тип ресурса Екстенсионпроперти</span><span class="sxs-lookup"><span data-stu-id="bf4ae-103">extensionProperty resource type</span></span>

<span data-ttu-id="bf4ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf4ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf4ae-105">Представляет расширение каталога, которое можно использовать для добавления настраиваемого свойства к объектам каталога без использования внешнего хранилища данных.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-105">Represents a directory extension that can be used to add a custom property to directory objects without requiring an external data store.</span></span> <span data-ttu-id="bf4ae-106">Например, если в Организации есть бизнес-приложение, для которого требуется идентификатор Skype для каждого пользователя в каталоге, Microsoft Graph можно использовать для регистрации нового свойства с именем Скипеид в объекте пользователя каталога, а затем для записи значения в новое свойство для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-106">For example, if an organization has a line of business (LOB) application that requires a Skype ID for each user in the directory, Microsoft Graph can be used to register a new property named skypeId on the directory’s User object, and then write a value to the new property for a specific user.</span></span>

<span data-ttu-id="bf4ae-107">Расширения можно добавлять в ресурсы " [пользователь](user.md)", " [Группа](group.md)", " [Организация](organization.md)", " [устройство](device.md)" и "ресурсы [приложения](application.md) ".</span><span class="sxs-lookup"><span data-stu-id="bf4ae-107">Extensions can be added to [user](user.md), [group](group.md), [organization](organization.md), [device](device.md), [application](application.md) resources.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="bf4ae-108">Расширения схемы Azure AD, описанные в этой статье, доступны только в целях обеспечения обратной совместимости в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-108">Azure AD schema extensions described here are available in Microsoft Graph for backwards compatibility reasons only.</span></span>
> <span data-ttu-id="bf4ae-109">Он позволяет использовать Microsoft Graph, чтобы продолжить управление свойствами расширения, добавленными через Azure AD Graph или [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect).</span><span class="sxs-lookup"><span data-stu-id="bf4ae-109">It allows you to use Microsoft Graph to continue to manage extension properties added through Azure AD Graph or [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect).</span></span>
> <span data-ttu-id="bf4ae-110">Для новых настраиваемых расширений рекомендуется использовать расширения схемы Microsoft Graph для [добавления пользовательских данных в ресурсы](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="bf4ae-110">For new custom extensions, we recommend that you use Microsoft Graph schema extensions for [adding custom data to resources](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="bf4ae-111">Методы</span><span class="sxs-lookup"><span data-stu-id="bf4ae-111">Methods</span></span>

| <span data-ttu-id="bf4ae-112">Метод</span><span class="sxs-lookup"><span data-stu-id="bf4ae-112">Method</span></span>       | <span data-ttu-id="bf4ae-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bf4ae-113">Return Type</span></span> | <span data-ttu-id="bf4ae-114">Описание</span><span class="sxs-lookup"><span data-stu-id="bf4ae-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bf4ae-115">Список расширений</span><span class="sxs-lookup"><span data-stu-id="bf4ae-115">List extensions</span></span>](../api/application-list-extensionproperty.md) | <span data-ttu-id="bf4ae-116">Коллекция [extensionProperty](extensionProperty.md)</span><span class="sxs-lookup"><span data-stu-id="bf4ae-116">[extensionProperty](extensionProperty.md) collection</span></span> | <span data-ttu-id="bf4ae-117">Список свойств расширения для объекта application.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-117">List extension properties on an application object.</span></span> |
| [<span data-ttu-id="bf4ae-118">Создание расширения</span><span class="sxs-lookup"><span data-stu-id="bf4ae-118">Create extension</span></span>](../api/application-post-extensionproperty.md) | [<span data-ttu-id="bf4ae-119">extensionProperty</span><span class="sxs-lookup"><span data-stu-id="bf4ae-119">extensionProperty</span></span>](extensionProperty.md) | <span data-ttu-id="bf4ae-120">Создание свойства расширения для объекта application.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-120">Create an extension property on an application object.</span></span> |
| [<span data-ttu-id="bf4ae-121">Удаление расширения</span><span class="sxs-lookup"><span data-stu-id="bf4ae-121">Delete extension</span></span>](../api/application-delete-extensionproperty.md) | <span data-ttu-id="bf4ae-122">Нет</span><span class="sxs-lookup"><span data-stu-id="bf4ae-122">None</span></span> | <span data-ttu-id="bf4ae-123">Удаление свойства расширения объекта application.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-123">Delete an extension property from an application object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bf4ae-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf4ae-124">Properties</span></span>

| <span data-ttu-id="bf4ae-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf4ae-125">Property</span></span>     | <span data-ttu-id="bf4ae-126">Тип</span><span class="sxs-lookup"><span data-stu-id="bf4ae-126">Type</span></span>        | <span data-ttu-id="bf4ae-127">Описание</span><span class="sxs-lookup"><span data-stu-id="bf4ae-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bf4ae-128">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="bf4ae-128">appDisplayName</span></span>|<span data-ttu-id="bf4ae-129">String</span><span class="sxs-lookup"><span data-stu-id="bf4ae-129">String</span></span>| <span data-ttu-id="bf4ae-130">Отображаемое имя объекта приложения, для которого определено это свойство расширения.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-130">Display name of the application object on which this extension property is defined.</span></span> <span data-ttu-id="bf4ae-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-131">Read-only.</span></span> |
|<span data-ttu-id="bf4ae-132">dataType</span><span class="sxs-lookup"><span data-stu-id="bf4ae-132">dataType</span></span>|<span data-ttu-id="bf4ae-133">String</span><span class="sxs-lookup"><span data-stu-id="bf4ae-133">String</span></span>| <span data-ttu-id="bf4ae-134">Задает тип данных значения, которое может содержать свойство Extension.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-134">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="bf4ae-135">Поддерживаются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="bf4ae-135">Following values are supported.</span></span> <span data-ttu-id="bf4ae-136">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-136">Not nullable.</span></span> <ul><li><span data-ttu-id="bf4ae-137">`Binary` – 256 байт (максимум)</span><span class="sxs-lookup"><span data-stu-id="bf4ae-137">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="bf4ae-138">`DateTime` -Должен быть указан в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-138">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="bf4ae-139">Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-139">Will be stored in UTC.</span></span></li><li><span data-ttu-id="bf4ae-140">`Integer` — значение 32 — бит.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-140">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="bf4ae-141">`LargeInteger` — значение 64 — бит.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-141">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="bf4ae-142">`String` – 256 символов максимум</span><span class="sxs-lookup"><span data-stu-id="bf4ae-142">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="bf4ae-143">иссинцедфромонпремисес</span><span class="sxs-lookup"><span data-stu-id="bf4ae-143">isSyncedFromOnPremises</span></span>|<span data-ttu-id="bf4ae-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf4ae-144">Boolean</span></span>| <span data-ttu-id="bf4ae-145">Указывает, было ли это свойство расширения сикнед из локального каталога с помощью Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-145">Indicates if this extension property was sycned from onpremises directory using Azure AD Connect.</span></span> <span data-ttu-id="bf4ae-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-146">Read-only.</span></span> |
|<span data-ttu-id="bf4ae-147">name</span><span class="sxs-lookup"><span data-stu-id="bf4ae-147">name</span></span>|<span data-ttu-id="bf4ae-148">String</span><span class="sxs-lookup"><span data-stu-id="bf4ae-148">String</span></span>| <span data-ttu-id="bf4ae-149">Имя свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-149">Name of the extension property.</span></span> <span data-ttu-id="bf4ae-150">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-150">Not nullable.</span></span> |
|<span data-ttu-id="bf4ae-151">таржетобжектс</span><span class="sxs-lookup"><span data-stu-id="bf4ae-151">targetObjects</span></span>|<span data-ttu-id="bf4ae-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bf4ae-152">String collection</span></span>| <span data-ttu-id="bf4ae-153">Поддерживаются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="bf4ae-153">Following values are supported.</span></span> <span data-ttu-id="bf4ae-154">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-154">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a><span data-ttu-id="bf4ae-155">Связи</span><span class="sxs-lookup"><span data-stu-id="bf4ae-155">Relationships</span></span>

<span data-ttu-id="bf4ae-156">Нет</span><span class="sxs-lookup"><span data-stu-id="bf4ae-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf4ae-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf4ae-157">JSON representation</span></span>

<span data-ttu-id="bf4ae-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf4ae-158">The following is a JSON representation of the resource.</span></span>

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


