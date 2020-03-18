---
title: Тип ресурса Оффицеконфигуратионграупассигнменттаржет
description: Целевой объект назначения группы AAD для группы клиентов Office.
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b27ecf9284dcf4ddf52502dab524e5d77d346f1f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797306"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="124c0-103">Тип ресурса Оффицеконфигуратионграупассигнменттаржет</span><span class="sxs-lookup"><span data-stu-id="124c0-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="124c0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="124c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="124c0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="124c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="124c0-106">Целевой объект назначения группы AAD для группы клиентов Office.</span><span class="sxs-lookup"><span data-stu-id="124c0-106">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="124c0-107">Наследуется от [оффицеконфигуратионассигнменттаржет](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="124c0-107">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="124c0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="124c0-108">Properties</span></span>
|<span data-ttu-id="124c0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="124c0-109">Property</span></span>|<span data-ttu-id="124c0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="124c0-110">Type</span></span>|<span data-ttu-id="124c0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="124c0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="124c0-112">groupId</span><span class="sxs-lookup"><span data-stu-id="124c0-112">groupId</span></span>|<span data-ttu-id="124c0-113">String</span><span class="sxs-lookup"><span data-stu-id="124c0-113">String</span></span>|<span data-ttu-id="124c0-114">Идентификатор группы AAD, на которую направляться конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="124c0-114">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="124c0-115">Связи</span><span class="sxs-lookup"><span data-stu-id="124c0-115">Relationships</span></span>
<span data-ttu-id="124c0-116">Нет</span><span class="sxs-lookup"><span data-stu-id="124c0-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="124c0-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="124c0-117">JSON Representation</span></span>
<span data-ttu-id="124c0-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="124c0-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



