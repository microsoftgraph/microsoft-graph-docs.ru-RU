---
title: Тип ресурса Оффицеконфигуратионграупассигнменттаржет
description: Целевой объект назначения группы AAD для группы клиентов Office.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 7458b1071b6133f3b46c8412270e30fdd0bf7638
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949313"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="c7bcf-103">Тип ресурса Оффицеконфигуратионграупассигнменттаржет</span><span class="sxs-lookup"><span data-stu-id="c7bcf-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="c7bcf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7bcf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7bcf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7bcf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7bcf-106">Целевой объект назначения группы AAD для группы клиентов Office.</span><span class="sxs-lookup"><span data-stu-id="c7bcf-106">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="c7bcf-107">Наследуется от [оффицеконфигуратионассигнменттаржет](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="c7bcf-107">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7bcf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7bcf-108">Properties</span></span>
|<span data-ttu-id="c7bcf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7bcf-109">Property</span></span>|<span data-ttu-id="c7bcf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c7bcf-110">Type</span></span>|<span data-ttu-id="c7bcf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c7bcf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7bcf-112">groupId</span><span class="sxs-lookup"><span data-stu-id="c7bcf-112">groupId</span></span>|<span data-ttu-id="c7bcf-113">String</span><span class="sxs-lookup"><span data-stu-id="c7bcf-113">String</span></span>|<span data-ttu-id="c7bcf-114">Идентификатор группы AAD, на которую направляться конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="c7bcf-114">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7bcf-115">Связи</span><span class="sxs-lookup"><span data-stu-id="c7bcf-115">Relationships</span></span>
<span data-ttu-id="c7bcf-116">Нет</span><span class="sxs-lookup"><span data-stu-id="c7bcf-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7bcf-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7bcf-117">JSON Representation</span></span>
<span data-ttu-id="c7bcf-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7bcf-118">Here is a JSON representation of the resource.</span></span>
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



