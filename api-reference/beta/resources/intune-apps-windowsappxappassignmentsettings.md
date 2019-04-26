---
title: Тип ресурса Виндовсаппксаппассигнментсеттингс
description: Содержит свойства, используемые при назначении мобильного приложения Windows AppX группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f15af8bf60dae2b40473eb23a1093f9e73bda7b6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557861"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="d9473-103">Тип ресурса Виндовсаппксаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="d9473-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="d9473-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9473-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9473-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9473-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9473-106">Содержит свойства, используемые при назначении мобильного приложения Windows AppX группе.</span><span class="sxs-lookup"><span data-stu-id="d9473-106">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>


<span data-ttu-id="d9473-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="d9473-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d9473-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9473-108">Properties</span></span>
|<span data-ttu-id="d9473-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9473-109">Property</span></span>|<span data-ttu-id="d9473-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d9473-110">Type</span></span>|<span data-ttu-id="d9473-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d9473-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9473-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="d9473-112">useDeviceContext</span></span>|<span data-ttu-id="d9473-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9473-113">Boolean</span></span>|<span data-ttu-id="d9473-114">Указывает, следует ли использовать контекст выполнения устройства для мобильного приложения Windows AppX.</span><span class="sxs-lookup"><span data-stu-id="d9473-114">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9473-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="d9473-115">Relationships</span></span>
<span data-ttu-id="d9473-116">Нет</span><span class="sxs-lookup"><span data-stu-id="d9473-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9473-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9473-117">JSON Representation</span></span>
<span data-ttu-id="d9473-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9473-118">Here is a JSON representation of the resource.</span></span>
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





