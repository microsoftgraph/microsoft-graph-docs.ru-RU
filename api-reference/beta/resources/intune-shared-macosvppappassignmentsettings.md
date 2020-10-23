---
title: Тип ресурса Макосвппаппассигнментсеттингс
description: Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2213a0a16ce4e4bb2954d6eebda27efe192a5772
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48681973"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="18c2b-103">Тип ресурса Макосвппаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="18c2b-103">macOsVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="18c2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18c2b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18c2b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18c2b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18c2b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18c2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18c2b-107">Содержит свойства, используемые для назначения мобильному приложению Mac VPP группе.</span><span class="sxs-lookup"><span data-stu-id="18c2b-107">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="18c2b-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="18c2b-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="18c2b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="18c2b-109">Properties</span></span>
|<span data-ttu-id="18c2b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="18c2b-110">Property</span></span>|<span data-ttu-id="18c2b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="18c2b-111">Type</span></span>|<span data-ttu-id="18c2b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="18c2b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18c2b-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="18c2b-113">useDeviceLicensing</span></span>|<span data-ttu-id="18c2b-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="18c2b-114">Boolean</span></span>|<span data-ttu-id="18c2b-115">Указывает, используется ли лицензирование устройств.</span><span class="sxs-lookup"><span data-stu-id="18c2b-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="18c2b-116">унинсталлондевицеремовал</span><span class="sxs-lookup"><span data-stu-id="18c2b-116">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="18c2b-117">Логический</span><span class="sxs-lookup"><span data-stu-id="18c2b-117">Boolean</span></span>|<span data-ttu-id="18c2b-118">Указывает, следует ли удалить приложение, когда устройство удалено из Intune.</span><span class="sxs-lookup"><span data-stu-id="18c2b-118">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18c2b-119">Связи</span><span class="sxs-lookup"><span data-stu-id="18c2b-119">Relationships</span></span>
<span data-ttu-id="18c2b-120">Нет</span><span class="sxs-lookup"><span data-stu-id="18c2b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18c2b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18c2b-121">JSON Representation</span></span>
<span data-ttu-id="18c2b-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18c2b-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "uninstallOnDeviceRemoval": true
}
```





