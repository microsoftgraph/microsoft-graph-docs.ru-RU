---
title: Тип ресурса Виндовсуниверсалаппксаппассигнментсеттингс
description: Содержит свойства, используемые при назначении мобильного приложения Windows Universal AppX группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 693b26142f83bf11d4f10f1da81fcf37cc69f8ed
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271620"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="34cbc-103">Тип ресурса Виндовсуниверсалаппксаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="34cbc-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

<span data-ttu-id="34cbc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34cbc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34cbc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34cbc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34cbc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34cbc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34cbc-107">Содержит свойства, используемые при назначении мобильного приложения Windows Universal AppX группе.</span><span class="sxs-lookup"><span data-stu-id="34cbc-107">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="34cbc-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="34cbc-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34cbc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="34cbc-109">Properties</span></span>
|<span data-ttu-id="34cbc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="34cbc-110">Property</span></span>|<span data-ttu-id="34cbc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="34cbc-111">Type</span></span>|<span data-ttu-id="34cbc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="34cbc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34cbc-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="34cbc-113">useDeviceContext</span></span>|<span data-ttu-id="34cbc-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="34cbc-114">Boolean</span></span>|<span data-ttu-id="34cbc-115">Указывает, следует ли использовать контекст выполнения устройства для мобильного приложения Windows Universal AppX.</span><span class="sxs-lookup"><span data-stu-id="34cbc-115">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34cbc-116">Связи</span><span class="sxs-lookup"><span data-stu-id="34cbc-116">Relationships</span></span>
<span data-ttu-id="34cbc-117">Нет</span><span class="sxs-lookup"><span data-stu-id="34cbc-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34cbc-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34cbc-118">JSON Representation</span></span>
<span data-ttu-id="34cbc-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34cbc-119">Here is a JSON representation of the resource.</span></span>
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




