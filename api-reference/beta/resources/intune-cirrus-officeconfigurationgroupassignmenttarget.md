---
title: Тип ресурса Оффицеконфигуратионграупассигнменттаржет
description: Целевой объект назначения группы AAD для группы клиентов Office.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d951db7a71474cc405f4b7f97419f1a06dd502d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294986"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="89f71-103">Тип ресурса Оффицеконфигуратионграупассигнменттаржет</span><span class="sxs-lookup"><span data-stu-id="89f71-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="89f71-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89f71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89f71-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89f71-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89f71-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89f71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89f71-107">Целевой объект назначения группы AAD для группы клиентов Office.</span><span class="sxs-lookup"><span data-stu-id="89f71-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="89f71-108">Наследуется от [оффицеконфигуратионассигнменттаржет](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="89f71-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="89f71-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="89f71-109">Properties</span></span>
|<span data-ttu-id="89f71-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="89f71-110">Property</span></span>|<span data-ttu-id="89f71-111">Тип</span><span class="sxs-lookup"><span data-stu-id="89f71-111">Type</span></span>|<span data-ttu-id="89f71-112">Описание</span><span class="sxs-lookup"><span data-stu-id="89f71-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89f71-113">groupId</span><span class="sxs-lookup"><span data-stu-id="89f71-113">groupId</span></span>|<span data-ttu-id="89f71-114">String</span><span class="sxs-lookup"><span data-stu-id="89f71-114">String</span></span>|<span data-ttu-id="89f71-115">Идентификатор группы AAD, на которую направляться конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="89f71-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89f71-116">Связи</span><span class="sxs-lookup"><span data-stu-id="89f71-116">Relationships</span></span>
<span data-ttu-id="89f71-117">Нет</span><span class="sxs-lookup"><span data-stu-id="89f71-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89f71-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89f71-118">JSON Representation</span></span>
<span data-ttu-id="89f71-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89f71-119">Here is a JSON representation of the resource.</span></span>
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




