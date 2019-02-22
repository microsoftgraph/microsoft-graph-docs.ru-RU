---
title: Тип ресурса Виндовсаппксаппассигнментсеттингс
description: Содержит свойства, используемые при назначении мобильного приложения Windows AppX группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83e384167984f1eda640ef1faa1f4241b1badbbb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167580"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="c0aa1-103">Тип ресурса Виндовсаппксаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="c0aa1-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="c0aa1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0aa1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0aa1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0aa1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0aa1-106">Содержит свойства, используемые при назначении мобильного приложения Windows AppX группе.</span><span class="sxs-lookup"><span data-stu-id="c0aa1-106">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>


<span data-ttu-id="c0aa1-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="c0aa1-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c0aa1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0aa1-108">Properties</span></span>
|<span data-ttu-id="c0aa1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0aa1-109">Property</span></span>|<span data-ttu-id="c0aa1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c0aa1-110">Type</span></span>|<span data-ttu-id="c0aa1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c0aa1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0aa1-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="c0aa1-112">useDeviceContext</span></span>|<span data-ttu-id="c0aa1-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0aa1-113">Boolean</span></span>|<span data-ttu-id="c0aa1-114">Указывает, следует ли использовать контекст выполнения устройства для мобильного приложения Windows AppX.</span><span class="sxs-lookup"><span data-stu-id="c0aa1-114">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0aa1-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="c0aa1-115">Relationships</span></span>
<span data-ttu-id="c0aa1-116">Нет</span><span class="sxs-lookup"><span data-stu-id="c0aa1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0aa1-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0aa1-117">JSON Representation</span></span>
<span data-ttu-id="c0aa1-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0aa1-118">Here is a JSON representation of the resource.</span></span>
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




