---
title: Тип ресурса win32LobAppRule
description: Базовый сложный тип для хранения данных правила обнаружения или требования для бизнес-приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 086805088c5b36cb3ab61f9117aa337f913f0386
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036754"
---
# <a name="win32lobapprule-resource-type"></a><span data-ttu-id="35d26-103">Тип ресурса win32LobAppRule</span><span class="sxs-lookup"><span data-stu-id="35d26-103">win32LobAppRule resource type</span></span>

<span data-ttu-id="35d26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35d26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35d26-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35d26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35d26-106">Базовый сложный тип для хранения данных правила обнаружения или требования для бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="35d26-106">A base complex type to store the detection or requirement rule data for a Win32 LOB app.</span></span>

## <a name="properties"></a><span data-ttu-id="35d26-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="35d26-107">Properties</span></span>
|<span data-ttu-id="35d26-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="35d26-108">Property</span></span>|<span data-ttu-id="35d26-109">Тип</span><span class="sxs-lookup"><span data-stu-id="35d26-109">Type</span></span>|<span data-ttu-id="35d26-110">Описание</span><span class="sxs-lookup"><span data-stu-id="35d26-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35d26-111">ruleType</span><span class="sxs-lookup"><span data-stu-id="35d26-111">ruleType</span></span>|[<span data-ttu-id="35d26-112">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="35d26-112">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="35d26-113">Тип правила, указывающий назначение правила.</span><span class="sxs-lookup"><span data-stu-id="35d26-113">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="35d26-114">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="35d26-114">Possible values are: `detection`, `requirement`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35d26-115">Связи</span><span class="sxs-lookup"><span data-stu-id="35d26-115">Relationships</span></span>
<span data-ttu-id="35d26-116">Нет</span><span class="sxs-lookup"><span data-stu-id="35d26-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35d26-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35d26-117">JSON Representation</span></span>
<span data-ttu-id="35d26-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35d26-118">Here is a JSON representation of the resource.</span></span>
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





