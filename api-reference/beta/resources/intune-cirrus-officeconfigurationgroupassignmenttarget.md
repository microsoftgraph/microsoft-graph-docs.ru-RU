---
title: Тип ресурса officeConfigurationGroupAssignmentTarget
description: Настройка клиента Office AAD группы конечного назначения.
ms.openlocfilehash: 263e48bfc5800231a9f36159e802f65294e6ac02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080660"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="5d6b1-103">Тип ресурса officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5d6b1-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="5d6b1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5d6b1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d6b1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d6b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d6b1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5d6b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d6b1-107">Настройка клиента Office AAD группы конечного назначения.</span><span class="sxs-lookup"><span data-stu-id="5d6b1-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="5d6b1-108">Наследуется от [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="5d6b1-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5d6b1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d6b1-109">Properties</span></span>
|<span data-ttu-id="5d6b1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d6b1-110">Property</span></span>|<span data-ttu-id="5d6b1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5d6b1-111">Type</span></span>|<span data-ttu-id="5d6b1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5d6b1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d6b1-113">groupId</span><span class="sxs-lookup"><span data-stu-id="5d6b1-113">groupId</span></span>|<span data-ttu-id="5d6b1-114">String</span><span class="sxs-lookup"><span data-stu-id="5d6b1-114">String</span></span>|<span data-ttu-id="5d6b1-115">Идентификатор группы AAD мы ориентация для настройки устройств.</span><span class="sxs-lookup"><span data-stu-id="5d6b1-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d6b1-116">Связи</span><span class="sxs-lookup"><span data-stu-id="5d6b1-116">Relationships</span></span>
<span data-ttu-id="5d6b1-117">Нет</span><span class="sxs-lookup"><span data-stu-id="5d6b1-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5d6b1-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5d6b1-118">JSON Representation</span></span>
<span data-ttu-id="5d6b1-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d6b1-119">Here is a JSON representation of the resource.</span></span>
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



