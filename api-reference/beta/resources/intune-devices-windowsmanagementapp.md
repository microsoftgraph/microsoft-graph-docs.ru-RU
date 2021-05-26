---
title: тип ресурса windowsManagementApp
description: Windows управления приложением.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 540ba41779e64c57b5c74c7acf004172a1567c37
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665576"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="f6761-103">тип ресурса windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="f6761-103">windowsManagementApp resource type</span></span>

<span data-ttu-id="f6761-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6761-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6761-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6761-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6761-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6761-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6761-107">Windows управления приложением.</span><span class="sxs-lookup"><span data-stu-id="f6761-107">Windows management app entity.</span></span>

## <a name="methods"></a><span data-ttu-id="f6761-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f6761-108">Methods</span></span>
|<span data-ttu-id="f6761-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f6761-109">Method</span></span>|<span data-ttu-id="f6761-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f6761-110">Return Type</span></span>|<span data-ttu-id="f6761-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f6761-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f6761-112">Get windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="f6761-112">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="f6761-113">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="f6761-113">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="f6761-114">Чтение свойств и связей [объекта WindowsManagementApp.](../resources/intune-devices-windowsmanagementapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6761-114">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="f6761-115">Обновление WindowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="f6761-115">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="f6761-116">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="f6761-116">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="f6761-117">Обновление свойств объекта [WindowsManagementApp.](../resources/intune-devices-windowsmanagementapp.md)</span><span class="sxs-lookup"><span data-stu-id="f6761-117">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="f6761-118">действие setAsManagedInstaller</span><span class="sxs-lookup"><span data-stu-id="f6761-118">setAsManagedInstaller action</span></span>](../api/intune-devices-windowsmanagementapp-setasmanagedinstaller.md)|<span data-ttu-id="f6761-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f6761-119">None</span></span>|<span data-ttu-id="f6761-120">Настройка состояния управляемого установщика для клиента вызываемого</span><span class="sxs-lookup"><span data-stu-id="f6761-120">Set the Managed Installer status for the caller tenant</span></span>|

## <a name="properties"></a><span data-ttu-id="f6761-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6761-121">Properties</span></span>
|<span data-ttu-id="f6761-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6761-122">Property</span></span>|<span data-ttu-id="f6761-123">Тип</span><span class="sxs-lookup"><span data-stu-id="f6761-123">Type</span></span>|<span data-ttu-id="f6761-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f6761-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6761-125">id</span><span class="sxs-lookup"><span data-stu-id="f6761-125">id</span></span>|<span data-ttu-id="f6761-126">Строка</span><span class="sxs-lookup"><span data-stu-id="f6761-126">String</span></span>|<span data-ttu-id="f6761-127">Уникальный идентификатор для приложения Windows управления</span><span class="sxs-lookup"><span data-stu-id="f6761-127">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="f6761-128">availableVersion</span><span class="sxs-lookup"><span data-stu-id="f6761-128">availableVersion</span></span>|<span data-ttu-id="f6761-129">Строка</span><span class="sxs-lookup"><span data-stu-id="f6761-129">String</span></span>|<span data-ttu-id="f6761-130">Windows доступной версии приложения для управления.</span><span class="sxs-lookup"><span data-stu-id="f6761-130">Windows management app available version.</span></span>|
|<span data-ttu-id="f6761-131">managedInstaller</span><span class="sxs-lookup"><span data-stu-id="f6761-131">managedInstaller</span></span>|[<span data-ttu-id="f6761-132">managedInstallerStatus</span><span class="sxs-lookup"><span data-stu-id="f6761-132">managedInstallerStatus</span></span>](../resources/intune-devices-managedinstallerstatus.md)|<span data-ttu-id="f6761-133">Состояние управляемого установщика.</span><span class="sxs-lookup"><span data-stu-id="f6761-133">Managed Installer Status.</span></span> <span data-ttu-id="f6761-134">Возможные значения: `disabled`, `enabled`.</span><span class="sxs-lookup"><span data-stu-id="f6761-134">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="f6761-135">managedInstallerConfiguredDateTime</span><span class="sxs-lookup"><span data-stu-id="f6761-135">managedInstallerConfiguredDateTime</span></span>|<span data-ttu-id="f6761-136">Строка</span><span class="sxs-lookup"><span data-stu-id="f6761-136">String</span></span>|<span data-ttu-id="f6761-137">Настроено время даты управляемого установщика</span><span class="sxs-lookup"><span data-stu-id="f6761-137">Managed Installer Configured Date Time</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6761-138">Связи</span><span class="sxs-lookup"><span data-stu-id="f6761-138">Relationships</span></span>
|<span data-ttu-id="f6761-139">Связь</span><span class="sxs-lookup"><span data-stu-id="f6761-139">Relationship</span></span>|<span data-ttu-id="f6761-140">Тип</span><span class="sxs-lookup"><span data-stu-id="f6761-140">Type</span></span>|<span data-ttu-id="f6761-141">Описание</span><span class="sxs-lookup"><span data-stu-id="f6761-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6761-142">healthStates</span><span class="sxs-lookup"><span data-stu-id="f6761-142">healthStates</span></span>|<span data-ttu-id="f6761-143">[коллекция windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)</span><span class="sxs-lookup"><span data-stu-id="f6761-143">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="f6761-144">Список состояния здоровья для установленного приложения Windows управления.</span><span class="sxs-lookup"><span data-stu-id="f6761-144">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6761-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6761-145">JSON Representation</span></span>
<span data-ttu-id="f6761-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6761-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String",
  "managedInstaller": "String",
  "managedInstallerConfiguredDateTime": "String"
}
```




