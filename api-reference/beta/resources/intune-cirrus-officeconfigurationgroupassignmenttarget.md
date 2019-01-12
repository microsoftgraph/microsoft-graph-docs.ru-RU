---
title: Тип ресурса officeConfigurationGroupAssignmentTarget
description: Настройка клиента Office AAD группы конечного назначения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9d59a6adc5478d619187e5414ac92170cbdedd49
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926381"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="5dc8f-103">Тип ресурса officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5dc8f-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="5dc8f-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5dc8f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5dc8f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5dc8f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5dc8f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5dc8f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5dc8f-107">Настройка клиента Office AAD группы конечного назначения.</span><span class="sxs-lookup"><span data-stu-id="5dc8f-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="5dc8f-108">Наследуется от [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="5dc8f-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5dc8f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5dc8f-109">Properties</span></span>
|<span data-ttu-id="5dc8f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5dc8f-110">Property</span></span>|<span data-ttu-id="5dc8f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5dc8f-111">Type</span></span>|<span data-ttu-id="5dc8f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5dc8f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dc8f-113">groupId</span><span class="sxs-lookup"><span data-stu-id="5dc8f-113">groupId</span></span>|<span data-ttu-id="5dc8f-114">Строка</span><span class="sxs-lookup"><span data-stu-id="5dc8f-114">String</span></span>|<span data-ttu-id="5dc8f-115">Идентификатор группы AAD мы ориентация для настройки устройств.</span><span class="sxs-lookup"><span data-stu-id="5dc8f-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5dc8f-116">Связи</span><span class="sxs-lookup"><span data-stu-id="5dc8f-116">Relationships</span></span>
<span data-ttu-id="5dc8f-117">Нет</span><span class="sxs-lookup"><span data-stu-id="5dc8f-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5dc8f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5dc8f-118">JSON Representation</span></span>
<span data-ttu-id="5dc8f-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5dc8f-119">Here is a JSON representation of the resource.</span></span>
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



