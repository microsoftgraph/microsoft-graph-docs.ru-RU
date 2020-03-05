---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9bb957258f43eeb9303876bcc0fa41a4b622cc45
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448412"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="ba84d-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="ba84d-103">managedAppDiagnosticStatus resource type</span></span>

<span data-ttu-id="ba84d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ba84d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba84d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba84d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba84d-106">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="ba84d-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="ba84d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba84d-107">Properties</span></span>
|<span data-ttu-id="ba84d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba84d-108">Property</span></span>|<span data-ttu-id="ba84d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ba84d-109">Type</span></span>|<span data-ttu-id="ba84d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ba84d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba84d-111">validationName</span><span class="sxs-lookup"><span data-stu-id="ba84d-111">validationName</span></span>|<span data-ttu-id="ba84d-112">String</span><span class="sxs-lookup"><span data-stu-id="ba84d-112">String</span></span>|<span data-ttu-id="ba84d-113">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="ba84d-113">The validation friendly name</span></span>|
|<span data-ttu-id="ba84d-114">state</span><span class="sxs-lookup"><span data-stu-id="ba84d-114">state</span></span>|<span data-ttu-id="ba84d-115">String</span><span class="sxs-lookup"><span data-stu-id="ba84d-115">String</span></span>|<span data-ttu-id="ba84d-116">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="ba84d-116">The state of the operation</span></span>|
|<span data-ttu-id="ba84d-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="ba84d-117">mitigationInstruction</span></span>|<span data-ttu-id="ba84d-118">String</span><span class="sxs-lookup"><span data-stu-id="ba84d-118">String</span></span>|<span data-ttu-id="ba84d-119">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="ba84d-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba84d-120">Связи</span><span class="sxs-lookup"><span data-stu-id="ba84d-120">Relationships</span></span>
<span data-ttu-id="ba84d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="ba84d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba84d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba84d-122">JSON Representation</span></span>
<span data-ttu-id="ba84d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba84d-123">Here is a JSON representation of the resource.</span></span>
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




