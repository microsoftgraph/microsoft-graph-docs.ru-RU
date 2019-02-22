---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf91e1a86955612aa590bee68057e1a7adb2d823
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169008"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="a83e4-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="a83e4-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="a83e4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a83e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a83e4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a83e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a83e4-106">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="a83e4-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="a83e4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a83e4-107">Properties</span></span>
|<span data-ttu-id="a83e4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a83e4-108">Property</span></span>|<span data-ttu-id="a83e4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a83e4-109">Type</span></span>|<span data-ttu-id="a83e4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a83e4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a83e4-111">validationName</span><span class="sxs-lookup"><span data-stu-id="a83e4-111">validationName</span></span>|<span data-ttu-id="a83e4-112">String</span><span class="sxs-lookup"><span data-stu-id="a83e4-112">String</span></span>|<span data-ttu-id="a83e4-113">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="a83e4-113">The validation friendly name</span></span>|
|<span data-ttu-id="a83e4-114">state</span><span class="sxs-lookup"><span data-stu-id="a83e4-114">state</span></span>|<span data-ttu-id="a83e4-115">String</span><span class="sxs-lookup"><span data-stu-id="a83e4-115">String</span></span>|<span data-ttu-id="a83e4-116">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="a83e4-116">The state of the operation</span></span>|
|<span data-ttu-id="a83e4-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="a83e4-117">mitigationInstruction</span></span>|<span data-ttu-id="a83e4-118">String</span><span class="sxs-lookup"><span data-stu-id="a83e4-118">String</span></span>|<span data-ttu-id="a83e4-119">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="a83e4-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="a83e4-120">Связи</span><span class="sxs-lookup"><span data-stu-id="a83e4-120">Relationships</span></span>
<span data-ttu-id="a83e4-121">Нет</span><span class="sxs-lookup"><span data-stu-id="a83e4-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a83e4-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a83e4-122">JSON Representation</span></span>
<span data-ttu-id="a83e4-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a83e4-123">Here is a JSON representation of the resource.</span></span>
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




