---
title: тип ресурса officeConfigurationGroupAssignmentTarget
description: Office клиентской конфигурации целевого назначения группы AAD.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d951db7a71474cc405f4b7f97419f1a06dd502d
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52667145"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="47244-103">тип ресурса officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="47244-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="47244-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47244-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47244-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47244-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47244-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47244-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47244-107">Office клиентской конфигурации целевого назначения группы AAD.</span><span class="sxs-lookup"><span data-stu-id="47244-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="47244-108">Наследует [от officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="47244-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="47244-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="47244-109">Properties</span></span>
|<span data-ttu-id="47244-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="47244-110">Property</span></span>|<span data-ttu-id="47244-111">Тип</span><span class="sxs-lookup"><span data-stu-id="47244-111">Type</span></span>|<span data-ttu-id="47244-112">Описание</span><span class="sxs-lookup"><span data-stu-id="47244-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47244-113">groupId</span><span class="sxs-lookup"><span data-stu-id="47244-113">groupId</span></span>|<span data-ttu-id="47244-114">String</span><span class="sxs-lookup"><span data-stu-id="47244-114">String</span></span>|<span data-ttu-id="47244-115">Id группы AAD, на который ориентирована конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="47244-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47244-116">Связи</span><span class="sxs-lookup"><span data-stu-id="47244-116">Relationships</span></span>
<span data-ttu-id="47244-117">Нет</span><span class="sxs-lookup"><span data-stu-id="47244-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47244-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47244-118">JSON Representation</span></span>
<span data-ttu-id="47244-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47244-119">Here is a JSON representation of the resource.</span></span>
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




