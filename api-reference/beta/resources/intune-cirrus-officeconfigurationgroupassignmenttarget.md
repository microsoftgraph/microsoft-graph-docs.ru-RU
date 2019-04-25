---
title: Тип ресурса Оффицеконфигуратионграупассигнменттаржет
description: Целевой объект назначения группы AAD для группы клиентов Office.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a3451d4bddec96c1e21cd605b05cb34d96372ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526393"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="9bdd6-103">Тип ресурса Оффицеконфигуратионграупассигнменттаржет</span><span class="sxs-lookup"><span data-stu-id="9bdd6-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="9bdd6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bdd6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bdd6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9bdd6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bdd6-106">Целевой объект назначения группы AAD для группы клиентов Office.</span><span class="sxs-lookup"><span data-stu-id="9bdd6-106">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="9bdd6-107">НаСледуется от [оффицеконфигуратионассигнменттаржет](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd6-107">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9bdd6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9bdd6-108">Properties</span></span>
|<span data-ttu-id="9bdd6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bdd6-109">Property</span></span>|<span data-ttu-id="9bdd6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9bdd6-110">Type</span></span>|<span data-ttu-id="9bdd6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9bdd6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bdd6-112">groupId</span><span class="sxs-lookup"><span data-stu-id="9bdd6-112">groupId</span></span>|<span data-ttu-id="9bdd6-113">String</span><span class="sxs-lookup"><span data-stu-id="9bdd6-113">String</span></span>|<span data-ttu-id="9bdd6-114">Идентификатор группы AAD, на которую направляться конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="9bdd6-114">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9bdd6-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="9bdd6-115">Relationships</span></span>
<span data-ttu-id="9bdd6-116">Нет</span><span class="sxs-lookup"><span data-stu-id="9bdd6-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9bdd6-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9bdd6-117">JSON Representation</span></span>
<span data-ttu-id="9bdd6-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9bdd6-118">Here is a JSON representation of the resource.</span></span>
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



