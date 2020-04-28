---
title: Тип ресурса Конфигуратионманажерактион
description: Параметр для действия Тригжерконфигуратионманажерактион
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 978049100f365786299035511e8795833631a9e0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465138"
---
# <a name="configurationmanageraction-resource-type"></a><span data-ttu-id="a01e4-103">Тип ресурса Конфигуратионманажерактион</span><span class="sxs-lookup"><span data-stu-id="a01e4-103">configurationManagerAction resource type</span></span>

<span data-ttu-id="a01e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a01e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a01e4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a01e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a01e4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a01e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a01e4-107">Параметр для действия Тригжерконфигуратионманажерактион</span><span class="sxs-lookup"><span data-stu-id="a01e4-107">Parameter for action triggerConfigurationManagerAction</span></span>

## <a name="properties"></a><span data-ttu-id="a01e4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a01e4-108">Properties</span></span>
|<span data-ttu-id="a01e4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a01e4-109">Property</span></span>|<span data-ttu-id="a01e4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a01e4-110">Type</span></span>|<span data-ttu-id="a01e4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a01e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a01e4-112">action</span><span class="sxs-lookup"><span data-stu-id="a01e4-112">action</span></span>|[<span data-ttu-id="a01e4-113">configurationManagerActionType</span><span class="sxs-lookup"><span data-stu-id="a01e4-113">configurationManagerActionType</span></span>](../resources/intune-devices-configurationmanageractiontype.md)|<span data-ttu-id="a01e4-114">Тип действия для триггера в клиенте Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="a01e4-114">The action type to trigger on Configuration Manager client.</span></span> <span data-ttu-id="a01e4-115">Возможные значения: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span><span class="sxs-lookup"><span data-stu-id="a01e4-115">Possible values are: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a01e4-116">Связи</span><span class="sxs-lookup"><span data-stu-id="a01e4-116">Relationships</span></span>
<span data-ttu-id="a01e4-117">Нет</span><span class="sxs-lookup"><span data-stu-id="a01e4-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a01e4-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a01e4-118">JSON Representation</span></span>
<span data-ttu-id="a01e4-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a01e4-119">Here is a JSON representation of the resource.</span></span>
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



