---
title: Тип ресурса Оффицеконфигуратионграупассигнменттаржет
description: Целевой объект назначения группы AAD для группы клиентов Office.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9e09d73695c542c24fe6be297dec9496794d95fc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454285"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="5b1c9-103">Тип ресурса Оффицеконфигуратионграупассигнменттаржет</span><span class="sxs-lookup"><span data-stu-id="5b1c9-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="5b1c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b1c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b1c9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b1c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b1c9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b1c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b1c9-107">Целевой объект назначения группы AAD для группы клиентов Office.</span><span class="sxs-lookup"><span data-stu-id="5b1c9-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="5b1c9-108">Наследуется от [оффицеконфигуратионассигнменттаржет](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="5b1c9-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5b1c9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b1c9-109">Properties</span></span>
|<span data-ttu-id="5b1c9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b1c9-110">Property</span></span>|<span data-ttu-id="5b1c9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5b1c9-111">Type</span></span>|<span data-ttu-id="5b1c9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5b1c9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b1c9-113">groupId</span><span class="sxs-lookup"><span data-stu-id="5b1c9-113">groupId</span></span>|<span data-ttu-id="5b1c9-114">String</span><span class="sxs-lookup"><span data-stu-id="5b1c9-114">String</span></span>|<span data-ttu-id="5b1c9-115">Идентификатор группы AAD, на которую направляться конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="5b1c9-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b1c9-116">Связи</span><span class="sxs-lookup"><span data-stu-id="5b1c9-116">Relationships</span></span>
<span data-ttu-id="5b1c9-117">Нет</span><span class="sxs-lookup"><span data-stu-id="5b1c9-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b1c9-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b1c9-118">JSON Representation</span></span>
<span data-ttu-id="5b1c9-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b1c9-119">Here is a JSON representation of the resource.</span></span>
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



