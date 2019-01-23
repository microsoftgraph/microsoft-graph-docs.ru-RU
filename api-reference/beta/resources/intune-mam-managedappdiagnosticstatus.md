---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 665ca55c67f5facb22eaf976e81737fed3dacf76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407363"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="0d94e-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="0d94e-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="0d94e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0d94e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0d94e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d94e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0d94e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d94e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d94e-107">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="0d94e-107">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="0d94e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d94e-108">Properties</span></span>
|<span data-ttu-id="0d94e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d94e-109">Property</span></span>|<span data-ttu-id="0d94e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0d94e-110">Type</span></span>|<span data-ttu-id="0d94e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0d94e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d94e-112">validationName</span><span class="sxs-lookup"><span data-stu-id="0d94e-112">validationName</span></span>|<span data-ttu-id="0d94e-113">String</span><span class="sxs-lookup"><span data-stu-id="0d94e-113">String</span></span>|<span data-ttu-id="0d94e-114">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="0d94e-114">The validation friendly name</span></span>|
|<span data-ttu-id="0d94e-115">state</span><span class="sxs-lookup"><span data-stu-id="0d94e-115">state</span></span>|<span data-ttu-id="0d94e-116">String</span><span class="sxs-lookup"><span data-stu-id="0d94e-116">String</span></span>|<span data-ttu-id="0d94e-117">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="0d94e-117">The state of the operation</span></span>|
|<span data-ttu-id="0d94e-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="0d94e-118">mitigationInstruction</span></span>|<span data-ttu-id="0d94e-119">String</span><span class="sxs-lookup"><span data-stu-id="0d94e-119">String</span></span>|<span data-ttu-id="0d94e-120">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="0d94e-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d94e-121">Связи</span><span class="sxs-lookup"><span data-stu-id="0d94e-121">Relationships</span></span>
<span data-ttu-id="0d94e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="0d94e-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d94e-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d94e-123">JSON Representation</span></span>
<span data-ttu-id="0d94e-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d94e-124">Here is a JSON representation of the resource.</span></span>
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




