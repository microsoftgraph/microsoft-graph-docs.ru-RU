---
title: Тип ресурса Виндовсаппксаппассигнментсеттингс
description: Содержит свойства, используемые при назначении мобильного приложения Windows AppX группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bba16c9a98bbdbf584cd7a0cba1c4634bf90b31
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949873"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="d4209-103">Тип ресурса Виндовсаппксаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="d4209-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="d4209-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4209-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4209-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4209-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4209-106">Содержит свойства, используемые при назначении мобильного приложения Windows AppX группе.</span><span class="sxs-lookup"><span data-stu-id="d4209-106">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>


<span data-ttu-id="d4209-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="d4209-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d4209-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4209-108">Properties</span></span>
|<span data-ttu-id="d4209-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4209-109">Property</span></span>|<span data-ttu-id="d4209-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d4209-110">Type</span></span>|<span data-ttu-id="d4209-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d4209-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4209-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="d4209-112">useDeviceContext</span></span>|<span data-ttu-id="d4209-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4209-113">Boolean</span></span>|<span data-ttu-id="d4209-114">Указывает, следует ли использовать контекст выполнения устройства для мобильного приложения Windows AppX.</span><span class="sxs-lookup"><span data-stu-id="d4209-114">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4209-115">Связи</span><span class="sxs-lookup"><span data-stu-id="d4209-115">Relationships</span></span>
<span data-ttu-id="d4209-116">Нет</span><span class="sxs-lookup"><span data-stu-id="d4209-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4209-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4209-117">JSON Representation</span></span>
<span data-ttu-id="d4209-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4209-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```




