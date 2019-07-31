---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0804b83f819a2f083493418e0cd1240702c2e425
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998431"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="8d0c2-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="8d0c2-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="8d0c2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d0c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d0c2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d0c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d0c2-106">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="8d0c2-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="8d0c2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d0c2-107">Properties</span></span>
|<span data-ttu-id="8d0c2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d0c2-108">Property</span></span>|<span data-ttu-id="8d0c2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8d0c2-109">Type</span></span>|<span data-ttu-id="8d0c2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8d0c2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d0c2-111">validationName</span><span class="sxs-lookup"><span data-stu-id="8d0c2-111">validationName</span></span>|<span data-ttu-id="8d0c2-112">String</span><span class="sxs-lookup"><span data-stu-id="8d0c2-112">String</span></span>|<span data-ttu-id="8d0c2-113">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="8d0c2-113">The validation friendly name</span></span>|
|<span data-ttu-id="8d0c2-114">state</span><span class="sxs-lookup"><span data-stu-id="8d0c2-114">state</span></span>|<span data-ttu-id="8d0c2-115">String</span><span class="sxs-lookup"><span data-stu-id="8d0c2-115">String</span></span>|<span data-ttu-id="8d0c2-116">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="8d0c2-116">The state of the operation</span></span>|
|<span data-ttu-id="8d0c2-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="8d0c2-117">mitigationInstruction</span></span>|<span data-ttu-id="8d0c2-118">String</span><span class="sxs-lookup"><span data-stu-id="8d0c2-118">String</span></span>|<span data-ttu-id="8d0c2-119">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="8d0c2-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d0c2-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="8d0c2-120">Relationships</span></span>
<span data-ttu-id="8d0c2-121">Нет</span><span class="sxs-lookup"><span data-stu-id="8d0c2-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d0c2-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d0c2-122">JSON Representation</span></span>
<span data-ttu-id="8d0c2-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d0c2-123">Here is a JSON representation of the resource.</span></span>
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





