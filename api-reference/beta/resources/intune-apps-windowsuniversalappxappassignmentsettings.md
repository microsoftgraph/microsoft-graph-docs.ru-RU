---
title: Тип ресурса Виндовсуниверсалаппксаппассигнментсеттингс
description: Содержит свойства, используемые при назначении мобильного приложения Windows Universal AppX группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0fedc16bbec643d792844a7762602fd66af60d34
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949838"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="6bf4b-103">Тип ресурса Виндовсуниверсалаппксаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="6bf4b-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="6bf4b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bf4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bf4b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6bf4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bf4b-106">Содержит свойства, используемые при назначении мобильного приложения Windows Universal AppX группе.</span><span class="sxs-lookup"><span data-stu-id="6bf4b-106">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="6bf4b-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6bf4b-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6bf4b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6bf4b-108">Properties</span></span>
|<span data-ttu-id="6bf4b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6bf4b-109">Property</span></span>|<span data-ttu-id="6bf4b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6bf4b-110">Type</span></span>|<span data-ttu-id="6bf4b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6bf4b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bf4b-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="6bf4b-112">useDeviceContext</span></span>|<span data-ttu-id="6bf4b-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bf4b-113">Boolean</span></span>|<span data-ttu-id="6bf4b-114">Указывает, следует ли использовать контекст выполнения устройства для мобильного приложения Windows Universal AppX.</span><span class="sxs-lookup"><span data-stu-id="6bf4b-114">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bf4b-115">Связи</span><span class="sxs-lookup"><span data-stu-id="6bf4b-115">Relationships</span></span>
<span data-ttu-id="6bf4b-116">Нет</span><span class="sxs-lookup"><span data-stu-id="6bf4b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6bf4b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6bf4b-117">JSON Representation</span></span>
<span data-ttu-id="6bf4b-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6bf4b-118">Here is a JSON representation of the resource.</span></span>
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




