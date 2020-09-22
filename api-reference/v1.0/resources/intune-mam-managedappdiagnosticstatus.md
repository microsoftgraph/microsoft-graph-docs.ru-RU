---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c708da33594087b61b1c28e2ebac5b8872541838
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041311"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="b8259-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="b8259-103">managedAppDiagnosticStatus resource type</span></span>

<span data-ttu-id="b8259-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8259-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8259-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8259-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8259-106">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="b8259-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="b8259-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8259-107">Properties</span></span>
|<span data-ttu-id="b8259-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8259-108">Property</span></span>|<span data-ttu-id="b8259-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b8259-109">Type</span></span>|<span data-ttu-id="b8259-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b8259-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8259-111">validationName</span><span class="sxs-lookup"><span data-stu-id="b8259-111">validationName</span></span>|<span data-ttu-id="b8259-112">String</span><span class="sxs-lookup"><span data-stu-id="b8259-112">String</span></span>|<span data-ttu-id="b8259-113">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="b8259-113">The validation friendly name</span></span>|
|<span data-ttu-id="b8259-114">state</span><span class="sxs-lookup"><span data-stu-id="b8259-114">state</span></span>|<span data-ttu-id="b8259-115">String</span><span class="sxs-lookup"><span data-stu-id="b8259-115">String</span></span>|<span data-ttu-id="b8259-116">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="b8259-116">The state of the operation</span></span>|
|<span data-ttu-id="b8259-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="b8259-117">mitigationInstruction</span></span>|<span data-ttu-id="b8259-118">String</span><span class="sxs-lookup"><span data-stu-id="b8259-118">String</span></span>|<span data-ttu-id="b8259-119">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="b8259-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8259-120">Связи</span><span class="sxs-lookup"><span data-stu-id="b8259-120">Relationships</span></span>
<span data-ttu-id="b8259-121">Нет</span><span class="sxs-lookup"><span data-stu-id="b8259-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8259-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8259-122">JSON Representation</span></span>
<span data-ttu-id="b8259-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8259-123">Here is a JSON representation of the resource.</span></span>
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









