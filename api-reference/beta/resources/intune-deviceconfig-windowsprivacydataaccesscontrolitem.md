---
title: Тип ресурса Виндовспривацидатаакцессконтролитем
description: Указание уровня контроля доступа для каждой категории данных о конфиденциальности
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 077af30aa9abe14ccc74c57a964074475d07cd4c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337708"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a><span data-ttu-id="3c5c3-103">Тип ресурса Виндовспривацидатаакцессконтролитем</span><span class="sxs-lookup"><span data-stu-id="3c5c3-103">windowsPrivacyDataAccessControlItem resource type</span></span>

> <span data-ttu-id="3c5c3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c5c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c5c3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c5c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c5c3-106">Указание уровня контроля доступа для каждой категории данных о конфиденциальности</span><span class="sxs-lookup"><span data-stu-id="3c5c3-106">Specify access control level per privacy data category</span></span>

## <a name="methods"></a><span data-ttu-id="3c5c3-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3c5c3-107">Methods</span></span>
|<span data-ttu-id="3c5c3-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3c5c3-108">Method</span></span>|<span data-ttu-id="3c5c3-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3c5c3-109">Return Type</span></span>|<span data-ttu-id="3c5c3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3c5c3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3c5c3-111">Список Виндовспривацидатаакцессконтролитемс</span><span class="sxs-lookup"><span data-stu-id="3c5c3-111">List windowsPrivacyDataAccessControlItems</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|<span data-ttu-id="3c5c3-112">Коллекция [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="3c5c3-112">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="3c5c3-113">Список свойств и связей объектов [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="3c5c3-113">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>|
|[<span data-ttu-id="3c5c3-114">Получение Виндовспривацидатаакцессконтролитем</span><span class="sxs-lookup"><span data-stu-id="3c5c3-114">Get windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[<span data-ttu-id="3c5c3-115">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="3c5c3-115">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="3c5c3-116">Чтение свойств и связей объекта [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="3c5c3-116">Read properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="3c5c3-117">Создание Виндовспривацидатаакцессконтролитем</span><span class="sxs-lookup"><span data-stu-id="3c5c3-117">Create windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[<span data-ttu-id="3c5c3-118">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="3c5c3-118">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="3c5c3-119">Создание нового объекта [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="3c5c3-119">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="3c5c3-120">Удаление Виндовспривацидатаакцессконтролитем</span><span class="sxs-lookup"><span data-stu-id="3c5c3-120">Delete windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|<span data-ttu-id="3c5c3-121">Нет</span><span class="sxs-lookup"><span data-stu-id="3c5c3-121">None</span></span>|<span data-ttu-id="3c5c3-122">Удаляет объект [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span><span class="sxs-lookup"><span data-stu-id="3c5c3-122">Deletes a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>|
|[<span data-ttu-id="3c5c3-123">Обновление Виндовспривацидатаакцессконтролитем</span><span class="sxs-lookup"><span data-stu-id="3c5c3-123">Update windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[<span data-ttu-id="3c5c3-124">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="3c5c3-124">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="3c5c3-125">Обновление свойств объекта [виндовспривацидатаакцессконтролитем](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) .</span><span class="sxs-lookup"><span data-stu-id="3c5c3-125">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3c5c3-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c5c3-126">Properties</span></span>
|<span data-ttu-id="3c5c3-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c5c3-127">Property</span></span>|<span data-ttu-id="3c5c3-128">Тип</span><span class="sxs-lookup"><span data-stu-id="3c5c3-128">Type</span></span>|<span data-ttu-id="3c5c3-129">Описание</span><span class="sxs-lookup"><span data-stu-id="3c5c3-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c5c3-130">id</span><span class="sxs-lookup"><span data-stu-id="3c5c3-130">id</span></span>|<span data-ttu-id="3c5c3-131">Строка</span><span class="sxs-lookup"><span data-stu-id="3c5c3-131">String</span></span>|<span data-ttu-id="3c5c3-132">Ключ Виндовспривацидатаакцессконтролитем.</span><span class="sxs-lookup"><span data-stu-id="3c5c3-132">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="3c5c3-133">accessLevel</span><span class="sxs-lookup"><span data-stu-id="3c5c3-133">accessLevel</span></span>|[<span data-ttu-id="3c5c3-134">виндовспривацидатаакцесслевел</span><span class="sxs-lookup"><span data-stu-id="3c5c3-134">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="3c5c3-135">Указывает уровень доступа для категории данных о конфиденциальности, в которую будет передано указанное приложение.</span><span class="sxs-lookup"><span data-stu-id="3c5c3-135">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="3c5c3-136">Возможные значения: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span><span class="sxs-lookup"><span data-stu-id="3c5c3-136">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="3c5c3-137">Категория "</span><span class="sxs-lookup"><span data-stu-id="3c5c3-137">dataCategory</span></span>|[<span data-ttu-id="3c5c3-138">виндовспривацидатакатегори</span><span class="sxs-lookup"><span data-stu-id="3c5c3-138">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="3c5c3-139">Указывает категорию данных о конфиденциальности, к которой будет применяться конкретное управление доступом.</span><span class="sxs-lookup"><span data-stu-id="3c5c3-139">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="3c5c3-140">Возможные значения: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar` `callHistory` `camera` `contacts` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices` `microphone` `motion`,,,,,,,,,,,,,,,,,,,,, `diagnosticsInfo` `email` `location` `messaging` .</span><span class="sxs-lookup"><span data-stu-id="3c5c3-140">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="3c5c3-141">апппаккажефамилинаме</span><span class="sxs-lookup"><span data-stu-id="3c5c3-141">appPackageFamilyName</span></span>|<span data-ttu-id="3c5c3-142">String</span><span class="sxs-lookup"><span data-stu-id="3c5c3-142">String</span></span>|<span data-ttu-id="3c5c3-143">Имя семейства пакетов для приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="3c5c3-143">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="3c5c3-144">Если этот параметр установлен, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="3c5c3-144">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="3c5c3-145">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="3c5c3-145">appDisplayName</span></span>|<span data-ttu-id="3c5c3-146">String</span><span class="sxs-lookup"><span data-stu-id="3c5c3-146">String</span></span>|<span data-ttu-id="3c5c3-147">Имя семейства пакетов для приложения Windows.</span><span class="sxs-lookup"><span data-stu-id="3c5c3-147">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="3c5c3-148">Если этот параметр установлен, уровень доступа применяется к указанному приложению.</span><span class="sxs-lookup"><span data-stu-id="3c5c3-148">When set, the access level applies to the specified application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c5c3-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="3c5c3-149">Relationships</span></span>
<span data-ttu-id="3c5c3-150">Нет</span><span class="sxs-lookup"><span data-stu-id="3c5c3-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c5c3-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c5c3-151">JSON Representation</span></span>
<span data-ttu-id="3c5c3-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c5c3-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPrivacyDataAccessControlItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "String (identifier)",
  "accessLevel": "String",
  "dataCategory": "String",
  "appPackageFamilyName": "String",
  "appDisplayName": "String"
}
```



