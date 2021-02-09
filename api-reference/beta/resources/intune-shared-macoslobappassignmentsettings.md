---
title: Тип ресурса macOsLobAppAssignmentSettings
description: Содержит свойства, используемые для назначения группы приложения для Mac LOB.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3e00019e2ed7609aa02fc3f16b2076027617fcab
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161004"
---
# <a name="macoslobappassignmentsettings-resource-type"></a><span data-ttu-id="e1a11-103">Тип ресурса macOsLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="e1a11-103">macOsLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="e1a11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1a11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1a11-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1a11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1a11-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1a11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1a11-107">Содержит свойства, используемые для назначения группы приложения для Mac LOB.</span><span class="sxs-lookup"><span data-stu-id="e1a11-107">Contains properties used to assign an Mac LOB  app to a group.</span></span>


<span data-ttu-id="e1a11-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e1a11-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e1a11-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1a11-109">Properties</span></span>
|<span data-ttu-id="e1a11-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1a11-110">Property</span></span>|<span data-ttu-id="e1a11-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e1a11-111">Type</span></span>|<span data-ttu-id="e1a11-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e1a11-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1a11-113">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="e1a11-113">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="e1a11-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1a11-114">Boolean</span></span>|<span data-ttu-id="e1a11-115">Следует ли удалить приложение при удалении устройства из Intune.</span><span class="sxs-lookup"><span data-stu-id="e1a11-115">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1a11-116">Связи</span><span class="sxs-lookup"><span data-stu-id="e1a11-116">Relationships</span></span>
<span data-ttu-id="e1a11-117">Нет</span><span class="sxs-lookup"><span data-stu-id="e1a11-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1a11-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1a11-118">JSON Representation</span></span>
<span data-ttu-id="e1a11-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1a11-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsLobAppAssignmentSettings",
  "uninstallOnDeviceRemoval": true
}
```




