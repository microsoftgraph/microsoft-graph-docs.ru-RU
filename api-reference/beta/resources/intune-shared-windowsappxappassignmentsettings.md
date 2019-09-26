---
title: Тип ресурса Виндовсаппксаппассигнментсеттингс
description: Содержит свойства, используемые при назначении мобильного приложения Windows AppX группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d56949f60ba2ae24091fe7b1ed871d43ba449f5d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201199"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="9b241-103">Тип ресурса Виндовсаппксаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="9b241-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="9b241-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b241-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b241-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b241-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b241-106">Содержит свойства, используемые при назначении мобильного приложения Windows AppX группе.</span><span class="sxs-lookup"><span data-stu-id="9b241-106">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>


<span data-ttu-id="9b241-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="9b241-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9b241-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b241-108">Properties</span></span>
|<span data-ttu-id="9b241-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b241-109">Property</span></span>|<span data-ttu-id="9b241-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9b241-110">Type</span></span>|<span data-ttu-id="9b241-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9b241-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b241-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="9b241-112">useDeviceContext</span></span>|<span data-ttu-id="9b241-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b241-113">Boolean</span></span>|<span data-ttu-id="9b241-114">Указывает, следует ли использовать контекст выполнения устройства для мобильного приложения Windows AppX.</span><span class="sxs-lookup"><span data-stu-id="9b241-114">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b241-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="9b241-115">Relationships</span></span>
<span data-ttu-id="9b241-116">Нет</span><span class="sxs-lookup"><span data-stu-id="9b241-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b241-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b241-117">JSON Representation</span></span>
<span data-ttu-id="9b241-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b241-118">Here is a JSON representation of the resource.</span></span>
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



