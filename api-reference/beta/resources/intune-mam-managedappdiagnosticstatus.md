---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a896a17a2a79db6eea2ac2ece0973175506bac4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940766"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="7c0b6-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="7c0b6-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="7c0b6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c0b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c0b6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c0b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c0b6-106">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="7c0b6-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="7c0b6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c0b6-107">Properties</span></span>
|<span data-ttu-id="7c0b6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c0b6-108">Property</span></span>|<span data-ttu-id="7c0b6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7c0b6-109">Type</span></span>|<span data-ttu-id="7c0b6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7c0b6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c0b6-111">validationName</span><span class="sxs-lookup"><span data-stu-id="7c0b6-111">validationName</span></span>|<span data-ttu-id="7c0b6-112">Строка</span><span class="sxs-lookup"><span data-stu-id="7c0b6-112">String</span></span>|<span data-ttu-id="7c0b6-113">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="7c0b6-113">The validation friendly name</span></span>|
|<span data-ttu-id="7c0b6-114">state</span><span class="sxs-lookup"><span data-stu-id="7c0b6-114">state</span></span>|<span data-ttu-id="7c0b6-115">String</span><span class="sxs-lookup"><span data-stu-id="7c0b6-115">String</span></span>|<span data-ttu-id="7c0b6-116">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="7c0b6-116">The state of the operation</span></span>|
|<span data-ttu-id="7c0b6-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="7c0b6-117">mitigationInstruction</span></span>|<span data-ttu-id="7c0b6-118">String</span><span class="sxs-lookup"><span data-stu-id="7c0b6-118">String</span></span>|<span data-ttu-id="7c0b6-119">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="7c0b6-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c0b6-120">Связи</span><span class="sxs-lookup"><span data-stu-id="7c0b6-120">Relationships</span></span>
<span data-ttu-id="7c0b6-121">Нет</span><span class="sxs-lookup"><span data-stu-id="7c0b6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c0b6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c0b6-122">JSON Representation</span></span>
<span data-ttu-id="7c0b6-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c0b6-123">Here is a JSON representation of the resource.</span></span>
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




