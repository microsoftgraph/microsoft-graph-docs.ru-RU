---
title: Тип ресурса Конфигуратионманажерактион
description: Параметр для действия Тригжерконфигуратионманажерактион
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 04d78d751f6cdd2978aa9cc65942acf312482202
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785100"
---
# <a name="configurationmanageraction-resource-type"></a><span data-ttu-id="28c8d-103">Тип ресурса Конфигуратионманажерактион</span><span class="sxs-lookup"><span data-stu-id="28c8d-103">configurationManagerAction resource type</span></span>

> <span data-ttu-id="28c8d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28c8d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28c8d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28c8d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28c8d-106">Параметр для действия Тригжерконфигуратионманажерактион</span><span class="sxs-lookup"><span data-stu-id="28c8d-106">Parameter for action triggerConfigurationManagerAction</span></span>

## <a name="properties"></a><span data-ttu-id="28c8d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="28c8d-107">Properties</span></span>
|<span data-ttu-id="28c8d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="28c8d-108">Property</span></span>|<span data-ttu-id="28c8d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="28c8d-109">Type</span></span>|<span data-ttu-id="28c8d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="28c8d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28c8d-111">action</span><span class="sxs-lookup"><span data-stu-id="28c8d-111">action</span></span>|[<span data-ttu-id="28c8d-112">configurationManagerActionType</span><span class="sxs-lookup"><span data-stu-id="28c8d-112">configurationManagerActionType</span></span>](../resources/intune-devices-configurationmanageractiontype.md)|<span data-ttu-id="28c8d-113">Тип действия для триггера в клиенте Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="28c8d-113">The action type to trigger on Configuration Manager client.</span></span> <span data-ttu-id="28c8d-114">Возможные значения: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span><span class="sxs-lookup"><span data-stu-id="28c8d-114">Possible values are: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28c8d-115">Связи</span><span class="sxs-lookup"><span data-stu-id="28c8d-115">Relationships</span></span>
<span data-ttu-id="28c8d-116">Нет</span><span class="sxs-lookup"><span data-stu-id="28c8d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28c8d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28c8d-117">JSON Representation</span></span>
<span data-ttu-id="28c8d-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28c8d-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerAction",
  "action": "String"
}
```



