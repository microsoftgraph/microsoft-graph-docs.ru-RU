---
title: Тип ресурса Виндовсуниверсалаппксаппассигнментсеттингс
description: Содержит свойства, используемые при назначении мобильного приложения Windows Universal AppX группе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dc945c303d49a97aeb45bf72e4fb8b5ffb7ab377
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447973"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="18be7-103">Тип ресурса Виндовсуниверсалаппксаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="18be7-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

<span data-ttu-id="18be7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18be7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18be7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18be7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18be7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18be7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18be7-107">Содержит свойства, используемые при назначении мобильного приложения Windows Universal AppX группе.</span><span class="sxs-lookup"><span data-stu-id="18be7-107">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="18be7-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="18be7-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="18be7-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="18be7-109">Properties</span></span>
|<span data-ttu-id="18be7-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="18be7-110">Property</span></span>|<span data-ttu-id="18be7-111">Тип</span><span class="sxs-lookup"><span data-stu-id="18be7-111">Type</span></span>|<span data-ttu-id="18be7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="18be7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18be7-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="18be7-113">useDeviceContext</span></span>|<span data-ttu-id="18be7-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="18be7-114">Boolean</span></span>|<span data-ttu-id="18be7-115">Указывает, следует ли использовать контекст выполнения устройства для мобильного приложения Windows Universal AppX.</span><span class="sxs-lookup"><span data-stu-id="18be7-115">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18be7-116">Связи</span><span class="sxs-lookup"><span data-stu-id="18be7-116">Relationships</span></span>
<span data-ttu-id="18be7-117">Нет</span><span class="sxs-lookup"><span data-stu-id="18be7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18be7-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18be7-118">JSON Representation</span></span>
<span data-ttu-id="18be7-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18be7-119">Here is a JSON representation of the resource.</span></span>
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



