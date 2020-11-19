---
title: Тип ресурса win32LobAppRule
description: Базовый сложный тип для хранения данных правила обнаружения или требования для бизнес-приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 317910873f46cd813617e8f14c149644aa8e5103
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49261030"
---
# <a name="win32lobapprule-resource-type"></a><span data-ttu-id="138d7-103">Тип ресурса win32LobAppRule</span><span class="sxs-lookup"><span data-stu-id="138d7-103">win32LobAppRule resource type</span></span>

<span data-ttu-id="138d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="138d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="138d7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="138d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="138d7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="138d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="138d7-107">Базовый сложный тип для хранения данных правила обнаружения или требования для бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="138d7-107">A base complex type to store the detection or requirement rule data for a Win32 LOB app.</span></span>

## <a name="properties"></a><span data-ttu-id="138d7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="138d7-108">Properties</span></span>
|<span data-ttu-id="138d7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="138d7-109">Property</span></span>|<span data-ttu-id="138d7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="138d7-110">Type</span></span>|<span data-ttu-id="138d7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="138d7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="138d7-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="138d7-112">ruleType</span></span>|[<span data-ttu-id="138d7-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="138d7-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="138d7-114">Тип правила, указывающий назначение правила.</span><span class="sxs-lookup"><span data-stu-id="138d7-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="138d7-115">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="138d7-115">Possible values are: `detection`, `requirement`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="138d7-116">Связи</span><span class="sxs-lookup"><span data-stu-id="138d7-116">Relationships</span></span>
<span data-ttu-id="138d7-117">Нет</span><span class="sxs-lookup"><span data-stu-id="138d7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="138d7-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="138d7-118">JSON Representation</span></span>
<span data-ttu-id="138d7-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="138d7-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRule",
  "ruleType": "String"
}
```




