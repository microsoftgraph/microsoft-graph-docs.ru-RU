---
title: Тип ресурса Виндовсуниверсалаппксаппассигнментсеттингс
description: Содержит свойства, используемые при назначении мобильного приложения Windows Universal AppX группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eeb724c9701b9bf0e82aa4d77689e8c2f58fe552
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558386"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="b0463-103">Тип ресурса Виндовсуниверсалаппксаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="b0463-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="b0463-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0463-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0463-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0463-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0463-106">Содержит свойства, используемые при назначении мобильного приложения Windows Universal AppX группе.</span><span class="sxs-lookup"><span data-stu-id="b0463-106">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="b0463-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b0463-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0463-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0463-108">Properties</span></span>
|<span data-ttu-id="b0463-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0463-109">Property</span></span>|<span data-ttu-id="b0463-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b0463-110">Type</span></span>|<span data-ttu-id="b0463-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b0463-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0463-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="b0463-112">useDeviceContext</span></span>|<span data-ttu-id="b0463-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0463-113">Boolean</span></span>|<span data-ttu-id="b0463-114">Указывает, следует ли использовать контекст выполнения устройства для мобильного приложения Windows Universal AppX.</span><span class="sxs-lookup"><span data-stu-id="b0463-114">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0463-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="b0463-115">Relationships</span></span>
<span data-ttu-id="b0463-116">Нет</span><span class="sxs-lookup"><span data-stu-id="b0463-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0463-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0463-117">JSON Representation</span></span>
<span data-ttu-id="b0463-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0463-118">Here is a JSON representation of the resource.</span></span>
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





