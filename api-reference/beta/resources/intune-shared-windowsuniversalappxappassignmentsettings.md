---
title: Тип ресурса Виндовсуниверсалаппксаппассигнментсеттингс
description: Содержит свойства, используемые при назначении мобильного приложения Windows Universal AppX группе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 26a1876879955d6db404cb521e10f4e07c8db043
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42766793"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="6bf97-103">Тип ресурса Виндовсуниверсалаппксаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="6bf97-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="6bf97-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bf97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bf97-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6bf97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bf97-106">Содержит свойства, используемые при назначении мобильного приложения Windows Universal AppX группе.</span><span class="sxs-lookup"><span data-stu-id="6bf97-106">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="6bf97-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6bf97-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6bf97-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6bf97-108">Properties</span></span>
|<span data-ttu-id="6bf97-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6bf97-109">Property</span></span>|<span data-ttu-id="6bf97-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6bf97-110">Type</span></span>|<span data-ttu-id="6bf97-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6bf97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bf97-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="6bf97-112">useDeviceContext</span></span>|<span data-ttu-id="6bf97-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bf97-113">Boolean</span></span>|<span data-ttu-id="6bf97-114">Указывает, следует ли использовать контекст выполнения устройства для мобильного приложения Windows Universal AppX.</span><span class="sxs-lookup"><span data-stu-id="6bf97-114">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bf97-115">Связи</span><span class="sxs-lookup"><span data-stu-id="6bf97-115">Relationships</span></span>
<span data-ttu-id="6bf97-116">Нет</span><span class="sxs-lookup"><span data-stu-id="6bf97-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6bf97-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6bf97-117">JSON Representation</span></span>
<span data-ttu-id="6bf97-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6bf97-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUniversalAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```



