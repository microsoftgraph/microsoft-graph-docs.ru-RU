---
title: monitoringSettings resource type
description: Параметры автоматизированного мониторинга и реагирования в развертывании.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: aff5fa9571628783521dcc5ae0113e767915c2c7
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068085"
---
# <a name="monitoringsettings-resource-type"></a><span data-ttu-id="cff98-103">monitoringSettings resource type</span><span class="sxs-lookup"><span data-stu-id="cff98-103">monitoringSettings resource type</span></span>

<span data-ttu-id="cff98-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="cff98-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cff98-105">Параметры автоматизированного мониторинга и реагирования в развертывании.</span><span class="sxs-lookup"><span data-stu-id="cff98-105">Settings controlling automated monitoring and response in a deployment.</span></span>

## <a name="properties"></a><span data-ttu-id="cff98-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cff98-106">Properties</span></span>
|<span data-ttu-id="cff98-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cff98-107">Property</span></span>|<span data-ttu-id="cff98-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cff98-108">Type</span></span>|<span data-ttu-id="cff98-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cff98-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cff98-110">monitoringRules</span><span class="sxs-lookup"><span data-stu-id="cff98-110">monitoringRules</span></span>|<span data-ttu-id="cff98-111">[коллекция microsoft.graph.windowsUpdates.monitoringRule](../resources/windowsupdates-monitoringrule.md)</span><span class="sxs-lookup"><span data-stu-id="cff98-111">[microsoft.graph.windowsUpdates.monitoringRule](../resources/windowsupdates-monitoringrule.md) collection</span></span>|<span data-ttu-id="cff98-112">Указывает правила, по которым сигналы мониторинга могут вызывать действия при развертывании.</span><span class="sxs-lookup"><span data-stu-id="cff98-112">Specifies the rules through which monitoring signals can trigger actions on the deployment.</span></span> <span data-ttu-id="cff98-113">Правила объединяются с помощью "или".</span><span class="sxs-lookup"><span data-stu-id="cff98-113">Rules are combined using "or".</span></span>|

## <a name="relationships"></a><span data-ttu-id="cff98-114">Связи</span><span class="sxs-lookup"><span data-stu-id="cff98-114">Relationships</span></span>
<span data-ttu-id="cff98-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cff98-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cff98-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cff98-116">JSON representation</span></span>
<span data-ttu-id="cff98-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cff98-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.monitoringSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.monitoringSettings",
  "monitoringRules": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.monitoringRule"
    }
  ]
}
```

