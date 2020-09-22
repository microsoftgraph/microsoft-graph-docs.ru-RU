---
title: Тип ресурса win32LobAppRule
description: Базовый сложный тип для хранения данных правила обнаружения или требования для бизнес-приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 78873e384208a9825ae02432c22cd55e84921a9d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092736"
---
# <a name="win32lobapprule-resource-type"></a><span data-ttu-id="aea85-103">Тип ресурса win32LobAppRule</span><span class="sxs-lookup"><span data-stu-id="aea85-103">win32LobAppRule resource type</span></span>

<span data-ttu-id="aea85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aea85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aea85-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aea85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aea85-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aea85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aea85-107">Базовый сложный тип для хранения данных правила обнаружения или требования для бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="aea85-107">A base complex type to store the detection or requirement rule data for a Win32 LOB app.</span></span>

## <a name="properties"></a><span data-ttu-id="aea85-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="aea85-108">Properties</span></span>
|<span data-ttu-id="aea85-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="aea85-109">Property</span></span>|<span data-ttu-id="aea85-110">Тип</span><span class="sxs-lookup"><span data-stu-id="aea85-110">Type</span></span>|<span data-ttu-id="aea85-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aea85-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aea85-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="aea85-112">ruleType</span></span>|[<span data-ttu-id="aea85-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="aea85-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="aea85-114">Тип правила, указывающий назначение правила.</span><span class="sxs-lookup"><span data-stu-id="aea85-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="aea85-115">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="aea85-115">Possible values are: `detection`, `requirement`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aea85-116">Связи</span><span class="sxs-lookup"><span data-stu-id="aea85-116">Relationships</span></span>
<span data-ttu-id="aea85-117">Нет</span><span class="sxs-lookup"><span data-stu-id="aea85-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aea85-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aea85-118">JSON Representation</span></span>
<span data-ttu-id="aea85-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aea85-119">Here is a JSON representation of the resource.</span></span>
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






