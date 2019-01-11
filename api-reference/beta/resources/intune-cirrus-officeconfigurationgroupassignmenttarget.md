---
title: Тип ресурса officeConfigurationGroupAssignmentTarget
description: Настройка клиента Office AAD группы конечного назначения.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b2fe6a668c1f490c167fe61496af14cf2654cebb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814772"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="52ba5-103">Тип ресурса officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="52ba5-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="52ba5-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="52ba5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52ba5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52ba5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52ba5-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="52ba5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52ba5-107">Настройка клиента Office AAD группы конечного назначения.</span><span class="sxs-lookup"><span data-stu-id="52ba5-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="52ba5-108">Наследуется от [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="52ba5-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="52ba5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="52ba5-109">Properties</span></span>
|<span data-ttu-id="52ba5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="52ba5-110">Property</span></span>|<span data-ttu-id="52ba5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="52ba5-111">Type</span></span>|<span data-ttu-id="52ba5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="52ba5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52ba5-113">groupId</span><span class="sxs-lookup"><span data-stu-id="52ba5-113">groupId</span></span>|<span data-ttu-id="52ba5-114">Строка</span><span class="sxs-lookup"><span data-stu-id="52ba5-114">String</span></span>|<span data-ttu-id="52ba5-115">Идентификатор группы AAD мы ориентация для настройки устройств.</span><span class="sxs-lookup"><span data-stu-id="52ba5-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52ba5-116">Связи</span><span class="sxs-lookup"><span data-stu-id="52ba5-116">Relationships</span></span>
<span data-ttu-id="52ba5-117">Нет</span><span class="sxs-lookup"><span data-stu-id="52ba5-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="52ba5-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52ba5-118">JSON Representation</span></span>
<span data-ttu-id="52ba5-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52ba5-119">Here is a JSON representation of the resource.</span></span>
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



