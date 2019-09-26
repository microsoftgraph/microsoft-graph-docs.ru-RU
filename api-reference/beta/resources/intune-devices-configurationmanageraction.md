---
title: Тип ресурса Конфигуратионманажерактион
description: Параметр для действия Тригжерконфигуратионманажерактион
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff71bc6b4094543e3da6d22639014f595a86ce7d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201297"
---
# <a name="configurationmanageraction-resource-type"></a><span data-ttu-id="888c2-103">Тип ресурса Конфигуратионманажерактион</span><span class="sxs-lookup"><span data-stu-id="888c2-103">configurationManagerAction resource type</span></span>

> <span data-ttu-id="888c2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="888c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="888c2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="888c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="888c2-106">Параметр для действия Тригжерконфигуратионманажерактион</span><span class="sxs-lookup"><span data-stu-id="888c2-106">Parameter for action triggerConfigurationManagerAction</span></span>

## <a name="properties"></a><span data-ttu-id="888c2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="888c2-107">Properties</span></span>
|<span data-ttu-id="888c2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="888c2-108">Property</span></span>|<span data-ttu-id="888c2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="888c2-109">Type</span></span>|<span data-ttu-id="888c2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="888c2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="888c2-111">action</span><span class="sxs-lookup"><span data-stu-id="888c2-111">action</span></span>|[<span data-ttu-id="888c2-112">конфигуратионманажерактионтипе</span><span class="sxs-lookup"><span data-stu-id="888c2-112">configurationManagerActionType</span></span>](../resources/intune-devices-configurationmanageractiontype.md)|<span data-ttu-id="888c2-113">Тип действия для триггера в клиенте Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="888c2-113">The action type to trigger on Configuration Manager client.</span></span> <span data-ttu-id="888c2-114">Возможные значения: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span><span class="sxs-lookup"><span data-stu-id="888c2-114">Possible values are: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="888c2-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="888c2-115">Relationships</span></span>
<span data-ttu-id="888c2-116">Нет</span><span class="sxs-lookup"><span data-stu-id="888c2-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="888c2-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="888c2-117">JSON Representation</span></span>
<span data-ttu-id="888c2-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="888c2-118">Here is a JSON representation of the resource.</span></span>
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



