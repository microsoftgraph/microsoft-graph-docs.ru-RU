---
title: Тип ресурса officeConfigurationGroupAssignmentTarget
description: Настройка клиента Office AAD группы конечного назначения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 411af117999498050288405874bd6b5baff5b6b5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422749"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="58c32-103">Тип ресурса officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="58c32-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="58c32-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="58c32-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="58c32-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58c32-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58c32-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58c32-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58c32-107">Настройка клиента Office AAD группы конечного назначения.</span><span class="sxs-lookup"><span data-stu-id="58c32-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="58c32-108">Наследуется от [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="58c32-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="58c32-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="58c32-109">Properties</span></span>
|<span data-ttu-id="58c32-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="58c32-110">Property</span></span>|<span data-ttu-id="58c32-111">Тип</span><span class="sxs-lookup"><span data-stu-id="58c32-111">Type</span></span>|<span data-ttu-id="58c32-112">Описание</span><span class="sxs-lookup"><span data-stu-id="58c32-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58c32-113">groupId</span><span class="sxs-lookup"><span data-stu-id="58c32-113">groupId</span></span>|<span data-ttu-id="58c32-114">String</span><span class="sxs-lookup"><span data-stu-id="58c32-114">String</span></span>|<span data-ttu-id="58c32-115">Идентификатор группы AAD мы ориентация для настройки устройств.</span><span class="sxs-lookup"><span data-stu-id="58c32-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58c32-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="58c32-116">Relationships</span></span>
<span data-ttu-id="58c32-117">Нет</span><span class="sxs-lookup"><span data-stu-id="58c32-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58c32-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58c32-118">JSON Representation</span></span>
<span data-ttu-id="58c32-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58c32-119">Here is a JSON representation of the resource.</span></span>
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



