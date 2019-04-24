---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2477039c3a0ebca3de09a4042691045782848b3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465307"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="bd19f-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="bd19f-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="bd19f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd19f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd19f-105">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="bd19f-105">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="bd19f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd19f-106">Properties</span></span>
|<span data-ttu-id="bd19f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd19f-107">Property</span></span>|<span data-ttu-id="bd19f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bd19f-108">Type</span></span>|<span data-ttu-id="bd19f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bd19f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd19f-110">validationName</span><span class="sxs-lookup"><span data-stu-id="bd19f-110">validationName</span></span>|<span data-ttu-id="bd19f-111">String</span><span class="sxs-lookup"><span data-stu-id="bd19f-111">String</span></span>|<span data-ttu-id="bd19f-112">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="bd19f-112">The validation friendly name</span></span>|
|<span data-ttu-id="bd19f-113">state</span><span class="sxs-lookup"><span data-stu-id="bd19f-113">state</span></span>|<span data-ttu-id="bd19f-114">String</span><span class="sxs-lookup"><span data-stu-id="bd19f-114">String</span></span>|<span data-ttu-id="bd19f-115">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="bd19f-115">The state of the operation</span></span>|
|<span data-ttu-id="bd19f-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="bd19f-116">mitigationInstruction</span></span>|<span data-ttu-id="bd19f-117">String</span><span class="sxs-lookup"><span data-stu-id="bd19f-117">String</span></span>|<span data-ttu-id="bd19f-118">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="bd19f-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd19f-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="bd19f-119">Relationships</span></span>
<span data-ttu-id="bd19f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="bd19f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd19f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd19f-121">JSON Representation</span></span>
<span data-ttu-id="bd19f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd19f-122">Here is a JSON representation of the resource.</span></span>
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



