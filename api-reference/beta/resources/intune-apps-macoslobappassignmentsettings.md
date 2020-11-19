---
title: Тип ресурса Макослобаппассигнментсеттингс
description: Содержит свойства, используемые для назначения бизнес-приложения Mac группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3e00019e2ed7609aa02fc3f16b2076027617fcab
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302234"
---
# <a name="macoslobappassignmentsettings-resource-type"></a><span data-ttu-id="a9f0a-103">Тип ресурса Макослобаппассигнментсеттингс</span><span class="sxs-lookup"><span data-stu-id="a9f0a-103">macOsLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="a9f0a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9f0a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9f0a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9f0a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9f0a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9f0a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9f0a-107">Содержит свойства, используемые для назначения бизнес-приложения Mac группе.</span><span class="sxs-lookup"><span data-stu-id="a9f0a-107">Contains properties used to assign an Mac LOB  app to a group.</span></span>


<span data-ttu-id="a9f0a-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a9f0a-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a9f0a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9f0a-109">Properties</span></span>
|<span data-ttu-id="a9f0a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9f0a-110">Property</span></span>|<span data-ttu-id="a9f0a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a9f0a-111">Type</span></span>|<span data-ttu-id="a9f0a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a9f0a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9f0a-113">унинсталлондевицеремовал</span><span class="sxs-lookup"><span data-stu-id="a9f0a-113">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="a9f0a-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9f0a-114">Boolean</span></span>|<span data-ttu-id="a9f0a-115">Указывает, следует ли удалить приложение, когда устройство удалено из Intune.</span><span class="sxs-lookup"><span data-stu-id="a9f0a-115">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9f0a-116">Связи</span><span class="sxs-lookup"><span data-stu-id="a9f0a-116">Relationships</span></span>
<span data-ttu-id="a9f0a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="a9f0a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9f0a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9f0a-118">JSON Representation</span></span>
<span data-ttu-id="a9f0a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9f0a-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsLobAppAssignmentSettings",
  "uninstallOnDeviceRemoval": true
}
```




