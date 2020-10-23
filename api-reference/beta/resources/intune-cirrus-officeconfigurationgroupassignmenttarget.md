---
title: Тип ресурса Оффицеконфигуратионграупассигнменттаржет
description: Целевой объект назначения группы AAD для группы клиентов Office.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bcfb80008880f6e2cd15119a3dda796a37a18250
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723979"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="357cb-103">Тип ресурса Оффицеконфигуратионграупассигнменттаржет</span><span class="sxs-lookup"><span data-stu-id="357cb-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="357cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="357cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="357cb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="357cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="357cb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="357cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="357cb-107">Целевой объект назначения группы AAD для группы клиентов Office.</span><span class="sxs-lookup"><span data-stu-id="357cb-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="357cb-108">Наследуется от [оффицеконфигуратионассигнменттаржет](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="357cb-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="357cb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="357cb-109">Properties</span></span>
|<span data-ttu-id="357cb-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="357cb-110">Property</span></span>|<span data-ttu-id="357cb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="357cb-111">Type</span></span>|<span data-ttu-id="357cb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="357cb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="357cb-113">groupId</span><span class="sxs-lookup"><span data-stu-id="357cb-113">groupId</span></span>|<span data-ttu-id="357cb-114">String</span><span class="sxs-lookup"><span data-stu-id="357cb-114">String</span></span>|<span data-ttu-id="357cb-115">Идентификатор группы AAD, на которую направляться конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="357cb-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="357cb-116">Связи</span><span class="sxs-lookup"><span data-stu-id="357cb-116">Relationships</span></span>
<span data-ttu-id="357cb-117">Нет</span><span class="sxs-lookup"><span data-stu-id="357cb-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="357cb-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="357cb-118">JSON Representation</span></span>
<span data-ttu-id="357cb-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="357cb-119">Here is a JSON representation of the resource.</span></span>
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





