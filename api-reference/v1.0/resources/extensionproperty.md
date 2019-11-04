---
title: Тип ресурса Екстенсионпроперти
description: Представляет расширение каталога
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 81bda27c0bee96fbac30e4f586e5ffb4a78bac09
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939504"
---
# <a name="extensionproperty-resource-type"></a><span data-ttu-id="cc2f4-103">Тип ресурса Екстенсионпроперти</span><span class="sxs-lookup"><span data-stu-id="cc2f4-103">extensionProperty resource type</span></span>

<span data-ttu-id="cc2f4-104">Представляет расширение каталога, которое можно использовать для добавления настраиваемого свойства к объектам каталога без использования внешнего хранилища данных.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-104">Represents a directory extension that can be used to add a custom property to directory objects without requiring an external data store.</span></span> <span data-ttu-id="cc2f4-105">Например, если в Организации есть бизнес-приложение, для которого требуется идентификатор Skype для каждого пользователя в каталоге, Microsoft Graph можно использовать для регистрации нового свойства с именем Скипеид в объекте пользователя каталога, а затем для записи значения в новое свойство. для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-105">For example, if an organization has a line of business (LOB) application that requires a Skype ID for each user in the directory, Microsoft Graph can be used to register a new property named skypeId on the directory’s User object, and then write a value to the new property for a specific user.</span></span>

<span data-ttu-id="cc2f4-106">Расширения можно добавлять в ресурсы " [пользователь](user.md)", " [Группа](group.md)", " [Организация](organization.md)", " [устройство](device.md)" и "ресурсы [приложения](application.md) ".</span><span class="sxs-lookup"><span data-stu-id="cc2f4-106">Extensions can be added to [user](user.md), [group](group.md), [organization](organization.md), [device](device.md), [application](application.md) resources.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="cc2f4-107">Расширения схемы Azure AD, описанные в этой статье, доступны только в целях обеспечения обратной совместимости в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-107">Azure AD schema extensions described here are available in Microsoft Graph for backwards compatibility reasons only.</span></span>
> <span data-ttu-id="cc2f4-108">Он позволяет использовать Microsoft Graph, чтобы продолжить управление свойствами расширения, добавленными через Azure AD Graph или [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect).</span><span class="sxs-lookup"><span data-stu-id="cc2f4-108">It allows you to use Microsoft Graph to continue to manage extension properties added through Azure AD Graph or [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-azure-ad-connect).</span></span>
> <span data-ttu-id="cc2f4-109">Для новых настраиваемых расширений рекомендуется использовать расширения схемы Microsoft Graph для [добавления пользовательских данных в ресурсы](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="cc2f4-109">For new custom extensions, we recommend that you use Microsoft Graph schema extensions for [adding custom data to resources](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="cc2f4-110">Методы</span><span class="sxs-lookup"><span data-stu-id="cc2f4-110">Methods</span></span>

| <span data-ttu-id="cc2f4-111">Метод</span><span class="sxs-lookup"><span data-stu-id="cc2f4-111">Method</span></span>       | <span data-ttu-id="cc2f4-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cc2f4-112">Return Type</span></span> | <span data-ttu-id="cc2f4-113">Описание</span><span class="sxs-lookup"><span data-stu-id="cc2f4-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cc2f4-114">Создание расширения</span><span class="sxs-lookup"><span data-stu-id="cc2f4-114">Create extension</span></span>](../api/application-post-extensionproperty.md) | [<span data-ttu-id="cc2f4-115">екстенсионпроперти</span><span class="sxs-lookup"><span data-stu-id="cc2f4-115">extensionProperty</span></span>](extensionProperty.md) | <span data-ttu-id="cc2f4-116">Создание свойства расширения для объекта Application.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-116">Create an extension property on an application object.</span></span> |
| [<span data-ttu-id="cc2f4-117">Расширения списка</span><span class="sxs-lookup"><span data-stu-id="cc2f4-117">List extensions</span></span>](../api/application-list-extensionproperty.md) | <span data-ttu-id="cc2f4-118">Коллекция [екстенсионпроперти](extensionProperty.md)</span><span class="sxs-lookup"><span data-stu-id="cc2f4-118">[extensionProperty](extensionProperty.md) collection</span></span> | <span data-ttu-id="cc2f4-119">Список свойств расширения для объекта Application.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-119">List extension properties on an application object.</span></span> |
| [<span data-ttu-id="cc2f4-120">Удаление расширения</span><span class="sxs-lookup"><span data-stu-id="cc2f4-120">Delete extension</span></span>](../api/application-delete-extensionproperty.md) | <span data-ttu-id="cc2f4-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-121">None</span></span> | <span data-ttu-id="cc2f4-122">Удаление свойства расширения из объекта Application.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-122">Delete an extension property from an application object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cc2f4-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc2f4-123">Properties</span></span>

| <span data-ttu-id="cc2f4-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc2f4-124">Property</span></span>     | <span data-ttu-id="cc2f4-125">Тип</span><span class="sxs-lookup"><span data-stu-id="cc2f4-125">Type</span></span>        | <span data-ttu-id="cc2f4-126">Описание</span><span class="sxs-lookup"><span data-stu-id="cc2f4-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cc2f4-127">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="cc2f4-127">appDisplayName</span></span>|<span data-ttu-id="cc2f4-128">String</span><span class="sxs-lookup"><span data-stu-id="cc2f4-128">String</span></span>| <span data-ttu-id="cc2f4-129">Отображаемое имя объекта приложения, для которого определено это свойство расширения.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-129">Display name of the application object on which this extension property is defined.</span></span> <span data-ttu-id="cc2f4-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-130">Read-only.</span></span> |
|<span data-ttu-id="cc2f4-131">dataType</span><span class="sxs-lookup"><span data-stu-id="cc2f4-131">dataType</span></span>|<span data-ttu-id="cc2f4-132">String</span><span class="sxs-lookup"><span data-stu-id="cc2f4-132">String</span></span>| <span data-ttu-id="cc2f4-133">Задает тип данных значения, которое может содержать свойство Extension.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-133">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="cc2f4-134">Поддерживаются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="cc2f4-134">Following values are supported.</span></span> <span data-ttu-id="cc2f4-135">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-135">Not nullable.</span></span> <ul><li><span data-ttu-id="cc2f4-136">`Binary`– 256 байт (максимум)</span><span class="sxs-lookup"><span data-stu-id="cc2f4-136">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="cc2f4-137">`DateTime`-Должен быть указан в формате ISO 8601.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-137">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="cc2f4-138">Данные времени будут храниться в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-138">Will be stored in UTC.</span></span></li><li><span data-ttu-id="cc2f4-139">`Integer`— значение 32 — бит.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-139">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="cc2f4-140">`LargeInteger`— значение 64 — бит.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-140">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="cc2f4-141">`String`– 256 символов максимум</span><span class="sxs-lookup"><span data-stu-id="cc2f4-141">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="cc2f4-142">иссинцедфромонпремисес</span><span class="sxs-lookup"><span data-stu-id="cc2f4-142">isSyncedFromOnPremises</span></span>|<span data-ttu-id="cc2f4-143">Логический</span><span class="sxs-lookup"><span data-stu-id="cc2f4-143">Boolean</span></span>| <span data-ttu-id="cc2f4-144">Указывает, было ли это свойство расширения сикнед из локального каталога с помощью Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-144">Indicates if this extension property was sycned from onpremises directory using Azure AD Connect.</span></span> <span data-ttu-id="cc2f4-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-145">Read-only.</span></span> |
|<span data-ttu-id="cc2f4-146">name</span><span class="sxs-lookup"><span data-stu-id="cc2f4-146">name</span></span>|<span data-ttu-id="cc2f4-147">Строка</span><span class="sxs-lookup"><span data-stu-id="cc2f4-147">String</span></span>| <span data-ttu-id="cc2f4-148">Имя свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-148">Name of the extension property.</span></span> <span data-ttu-id="cc2f4-149">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-149">Not nullable.</span></span> |
|<span data-ttu-id="cc2f4-150">таржетобжектс</span><span class="sxs-lookup"><span data-stu-id="cc2f4-150">targetObjects</span></span>|<span data-ttu-id="cc2f4-151">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cc2f4-151">String collection</span></span>| <span data-ttu-id="cc2f4-152">Поддерживаются следующие значения:</span><span class="sxs-lookup"><span data-stu-id="cc2f4-152">Following values are supported.</span></span> <span data-ttu-id="cc2f4-153">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-153">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|

## <a name="relationships"></a><span data-ttu-id="cc2f4-154">Связи</span><span class="sxs-lookup"><span data-stu-id="cc2f4-154">Relationships</span></span>

<span data-ttu-id="cc2f4-155">Нет</span><span class="sxs-lookup"><span data-stu-id="cc2f4-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc2f4-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc2f4-156">JSON representation</span></span>

<span data-ttu-id="cc2f4-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc2f4-157">The following is a JSON representation of the resource.</span></span>

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
