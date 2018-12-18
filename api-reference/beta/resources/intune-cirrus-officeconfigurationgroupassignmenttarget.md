---
title: Тип ресурса officeConfigurationGroupAssignmentTarget
description: Настройка клиента Office AAD группы конечного назначения.
author: tfitzmac
ms.openlocfilehash: 82008de6e5cb64885e9e2d5804a00956da2ff434
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335870"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="569f4-103">Тип ресурса officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="569f4-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="569f4-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="569f4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="569f4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="569f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="569f4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="569f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="569f4-107">Настройка клиента Office AAD группы конечного назначения.</span><span class="sxs-lookup"><span data-stu-id="569f4-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="569f4-108">Наследуется от [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="569f4-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="569f4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="569f4-109">Properties</span></span>
|<span data-ttu-id="569f4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="569f4-110">Property</span></span>|<span data-ttu-id="569f4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="569f4-111">Type</span></span>|<span data-ttu-id="569f4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="569f4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="569f4-113">groupId</span><span class="sxs-lookup"><span data-stu-id="569f4-113">groupId</span></span>|<span data-ttu-id="569f4-114">Строка</span><span class="sxs-lookup"><span data-stu-id="569f4-114">String</span></span>|<span data-ttu-id="569f4-115">Идентификатор группы AAD мы ориентация для настройки устройств.</span><span class="sxs-lookup"><span data-stu-id="569f4-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="569f4-116">Связи</span><span class="sxs-lookup"><span data-stu-id="569f4-116">Relationships</span></span>
<span data-ttu-id="569f4-117">Нет</span><span class="sxs-lookup"><span data-stu-id="569f4-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="569f4-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="569f4-118">JSON Representation</span></span>
<span data-ttu-id="569f4-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="569f4-119">Here is a JSON representation of the resource.</span></span>
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



