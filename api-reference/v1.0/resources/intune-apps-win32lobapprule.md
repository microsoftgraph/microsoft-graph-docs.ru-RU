---
title: тип ресурса win32LobAppRule
description: Базовый сложный тип для хранения данных правил обнаружения или требования для приложения LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1494aa6089bac73ae14612804009237bb9a5b2fc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758962"
---
# <a name="win32lobapprule-resource-type"></a><span data-ttu-id="2b919-103">тип ресурса win32LobAppRule</span><span class="sxs-lookup"><span data-stu-id="2b919-103">win32LobAppRule resource type</span></span>

<span data-ttu-id="2b919-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b919-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b919-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b919-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b919-106">Базовый сложный тип для хранения данных правил обнаружения или требования для приложения LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="2b919-106">A base complex type to store the detection or requirement rule data for a Win32 LOB app.</span></span>

## <a name="properties"></a><span data-ttu-id="2b919-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b919-107">Properties</span></span>
|<span data-ttu-id="2b919-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b919-108">Property</span></span>|<span data-ttu-id="2b919-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2b919-109">Type</span></span>|<span data-ttu-id="2b919-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2b919-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b919-111">ruleType</span><span class="sxs-lookup"><span data-stu-id="2b919-111">ruleType</span></span>|[<span data-ttu-id="2b919-112">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="2b919-112">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="2b919-113">Тип правила, указывающий цель правила.</span><span class="sxs-lookup"><span data-stu-id="2b919-113">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="2b919-114">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="2b919-114">Possible values are: `detection`, `requirement`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b919-115">Связи</span><span class="sxs-lookup"><span data-stu-id="2b919-115">Relationships</span></span>
<span data-ttu-id="2b919-116">Нет</span><span class="sxs-lookup"><span data-stu-id="2b919-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b919-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b919-117">JSON Representation</span></span>
<span data-ttu-id="2b919-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b919-118">Here is a JSON representation of the resource.</span></span>
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




