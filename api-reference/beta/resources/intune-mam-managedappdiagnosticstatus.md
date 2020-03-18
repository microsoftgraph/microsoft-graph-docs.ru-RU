---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6020b6a8875b8e2aff2e92b007364fc3011da216
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42781945"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="312ea-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="312ea-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="312ea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="312ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="312ea-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="312ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="312ea-106">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="312ea-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="312ea-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="312ea-107">Properties</span></span>
|<span data-ttu-id="312ea-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="312ea-108">Property</span></span>|<span data-ttu-id="312ea-109">Тип</span><span class="sxs-lookup"><span data-stu-id="312ea-109">Type</span></span>|<span data-ttu-id="312ea-110">Описание</span><span class="sxs-lookup"><span data-stu-id="312ea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="312ea-111">validationName</span><span class="sxs-lookup"><span data-stu-id="312ea-111">validationName</span></span>|<span data-ttu-id="312ea-112">String</span><span class="sxs-lookup"><span data-stu-id="312ea-112">String</span></span>|<span data-ttu-id="312ea-113">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="312ea-113">The validation friendly name</span></span>|
|<span data-ttu-id="312ea-114">state</span><span class="sxs-lookup"><span data-stu-id="312ea-114">state</span></span>|<span data-ttu-id="312ea-115">String</span><span class="sxs-lookup"><span data-stu-id="312ea-115">String</span></span>|<span data-ttu-id="312ea-116">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="312ea-116">The state of the operation</span></span>|
|<span data-ttu-id="312ea-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="312ea-117">mitigationInstruction</span></span>|<span data-ttu-id="312ea-118">String</span><span class="sxs-lookup"><span data-stu-id="312ea-118">String</span></span>|<span data-ttu-id="312ea-119">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="312ea-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="312ea-120">Связи</span><span class="sxs-lookup"><span data-stu-id="312ea-120">Relationships</span></span>
<span data-ttu-id="312ea-121">Нет</span><span class="sxs-lookup"><span data-stu-id="312ea-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="312ea-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="312ea-122">JSON Representation</span></span>
<span data-ttu-id="312ea-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="312ea-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```



