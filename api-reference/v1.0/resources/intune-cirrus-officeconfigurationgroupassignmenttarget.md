---
title: тип ресурса officeConfigurationGroupAssignmentTarget
description: Office клиентской конфигурации целевого назначения группы AAD.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d951db7a71474cc405f4b7f97419f1a06dd502d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755574"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="300ba-103">тип ресурса officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="300ba-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="300ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="300ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="300ba-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="300ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="300ba-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="300ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="300ba-107">Office клиентской конфигурации целевого назначения группы AAD.</span><span class="sxs-lookup"><span data-stu-id="300ba-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="300ba-108">Наследует [от officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="300ba-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="300ba-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="300ba-109">Properties</span></span>
|<span data-ttu-id="300ba-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="300ba-110">Property</span></span>|<span data-ttu-id="300ba-111">Тип</span><span class="sxs-lookup"><span data-stu-id="300ba-111">Type</span></span>|<span data-ttu-id="300ba-112">Описание</span><span class="sxs-lookup"><span data-stu-id="300ba-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="300ba-113">groupId</span><span class="sxs-lookup"><span data-stu-id="300ba-113">groupId</span></span>|<span data-ttu-id="300ba-114">String</span><span class="sxs-lookup"><span data-stu-id="300ba-114">String</span></span>|<span data-ttu-id="300ba-115">Id группы AAD, на который ориентирована конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="300ba-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="300ba-116">Связи</span><span class="sxs-lookup"><span data-stu-id="300ba-116">Relationships</span></span>
<span data-ttu-id="300ba-117">Нет</span><span class="sxs-lookup"><span data-stu-id="300ba-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="300ba-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="300ba-118">JSON Representation</span></span>
<span data-ttu-id="300ba-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="300ba-119">Here is a JSON representation of the resource.</span></span>
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




