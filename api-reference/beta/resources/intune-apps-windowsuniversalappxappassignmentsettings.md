---
title: Тип ресурса Виндовсуниверсалаппксаппассигнментсеттингс
description: Содержит свойства, используемые при назначении мобильного приложения Windows Universal AppX группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58e0c656464d962d1a16a7c4651c4379876bf6ae
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153734"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="081e8-103">Тип ресурса Виндовсуниверсалаппксаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="081e8-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="081e8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="081e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="081e8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="081e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="081e8-106">Содержит свойства, используемые при назначении мобильного приложения Windows Universal AppX группе.</span><span class="sxs-lookup"><span data-stu-id="081e8-106">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="081e8-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="081e8-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="081e8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="081e8-108">Properties</span></span>
|<span data-ttu-id="081e8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="081e8-109">Property</span></span>|<span data-ttu-id="081e8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="081e8-110">Type</span></span>|<span data-ttu-id="081e8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="081e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="081e8-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="081e8-112">useDeviceContext</span></span>|<span data-ttu-id="081e8-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="081e8-113">Boolean</span></span>|<span data-ttu-id="081e8-114">Указывает, следует ли использовать контекст выполнения устройства для мобильного приложения Windows Universal AppX.</span><span class="sxs-lookup"><span data-stu-id="081e8-114">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="081e8-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="081e8-115">Relationships</span></span>
<span data-ttu-id="081e8-116">Нет</span><span class="sxs-lookup"><span data-stu-id="081e8-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="081e8-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="081e8-117">JSON Representation</span></span>
<span data-ttu-id="081e8-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="081e8-118">Here is a JSON representation of the resource.</span></span>
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




