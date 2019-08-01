---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 79a89b7084ea006352ad0bc423d0833acfaae86e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038047"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="4ed8a-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="4ed8a-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="4ed8a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ed8a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ed8a-105">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="4ed8a-105">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="4ed8a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ed8a-106">Properties</span></span>
|<span data-ttu-id="4ed8a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ed8a-107">Property</span></span>|<span data-ttu-id="4ed8a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4ed8a-108">Type</span></span>|<span data-ttu-id="4ed8a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4ed8a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ed8a-110">validationName</span><span class="sxs-lookup"><span data-stu-id="4ed8a-110">validationName</span></span>|<span data-ttu-id="4ed8a-111">String</span><span class="sxs-lookup"><span data-stu-id="4ed8a-111">String</span></span>|<span data-ttu-id="4ed8a-112">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="4ed8a-112">The validation friendly name</span></span>|
|<span data-ttu-id="4ed8a-113">state</span><span class="sxs-lookup"><span data-stu-id="4ed8a-113">state</span></span>|<span data-ttu-id="4ed8a-114">String</span><span class="sxs-lookup"><span data-stu-id="4ed8a-114">String</span></span>|<span data-ttu-id="4ed8a-115">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="4ed8a-115">The state of the operation</span></span>|
|<span data-ttu-id="4ed8a-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="4ed8a-116">mitigationInstruction</span></span>|<span data-ttu-id="4ed8a-117">String</span><span class="sxs-lookup"><span data-stu-id="4ed8a-117">String</span></span>|<span data-ttu-id="4ed8a-118">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="4ed8a-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ed8a-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="4ed8a-119">Relationships</span></span>
<span data-ttu-id="4ed8a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="4ed8a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ed8a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ed8a-121">JSON Representation</span></span>
<span data-ttu-id="4ed8a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ed8a-122">Here is a JSON representation of the resource.</span></span>
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



