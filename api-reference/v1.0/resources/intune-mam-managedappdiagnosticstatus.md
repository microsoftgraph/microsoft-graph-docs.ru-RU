---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2477039c3a0ebca3de09a4042691045782848b3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261553"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="144ca-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="144ca-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="144ca-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="144ca-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="144ca-105">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="144ca-105">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="144ca-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="144ca-106">Properties</span></span>
|<span data-ttu-id="144ca-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="144ca-107">Property</span></span>|<span data-ttu-id="144ca-108">Тип</span><span class="sxs-lookup"><span data-stu-id="144ca-108">Type</span></span>|<span data-ttu-id="144ca-109">Описание</span><span class="sxs-lookup"><span data-stu-id="144ca-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="144ca-110">validationName</span><span class="sxs-lookup"><span data-stu-id="144ca-110">validationName</span></span>|<span data-ttu-id="144ca-111">String</span><span class="sxs-lookup"><span data-stu-id="144ca-111">String</span></span>|<span data-ttu-id="144ca-112">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="144ca-112">The validation friendly name</span></span>|
|<span data-ttu-id="144ca-113">state</span><span class="sxs-lookup"><span data-stu-id="144ca-113">state</span></span>|<span data-ttu-id="144ca-114">String</span><span class="sxs-lookup"><span data-stu-id="144ca-114">String</span></span>|<span data-ttu-id="144ca-115">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="144ca-115">The state of the operation</span></span>|
|<span data-ttu-id="144ca-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="144ca-116">mitigationInstruction</span></span>|<span data-ttu-id="144ca-117">String</span><span class="sxs-lookup"><span data-stu-id="144ca-117">String</span></span>|<span data-ttu-id="144ca-118">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="144ca-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="144ca-119">Связи</span><span class="sxs-lookup"><span data-stu-id="144ca-119">Relationships</span></span>
<span data-ttu-id="144ca-120">Нет</span><span class="sxs-lookup"><span data-stu-id="144ca-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="144ca-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="144ca-121">JSON Representation</span></span>
<span data-ttu-id="144ca-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="144ca-122">Here is a JSON representation of the resource.</span></span>
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



