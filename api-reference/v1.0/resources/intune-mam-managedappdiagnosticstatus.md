---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3a5204a4704eefc2d4e7c8e0d5b3b709e1750667
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937483"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="7429f-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="7429f-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="7429f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7429f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7429f-105">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="7429f-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="7429f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7429f-106">Properties</span></span>
|<span data-ttu-id="7429f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7429f-107">Property</span></span>|<span data-ttu-id="7429f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7429f-108">Type</span></span>|<span data-ttu-id="7429f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7429f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7429f-110">validationName</span><span class="sxs-lookup"><span data-stu-id="7429f-110">validationName</span></span>|<span data-ttu-id="7429f-111">String</span><span class="sxs-lookup"><span data-stu-id="7429f-111">String</span></span>|<span data-ttu-id="7429f-112">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="7429f-112">The validation friendly name</span></span>|
|<span data-ttu-id="7429f-113">state</span><span class="sxs-lookup"><span data-stu-id="7429f-113">state</span></span>|<span data-ttu-id="7429f-114">String</span><span class="sxs-lookup"><span data-stu-id="7429f-114">String</span></span>|<span data-ttu-id="7429f-115">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="7429f-115">The state of the operation</span></span>|
|<span data-ttu-id="7429f-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="7429f-116">mitigationInstruction</span></span>|<span data-ttu-id="7429f-117">String</span><span class="sxs-lookup"><span data-stu-id="7429f-117">String</span></span>|<span data-ttu-id="7429f-118">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="7429f-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="7429f-119">Связи</span><span class="sxs-lookup"><span data-stu-id="7429f-119">Relationships</span></span>
<span data-ttu-id="7429f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="7429f-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7429f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7429f-121">JSON Representation</span></span>
<span data-ttu-id="7429f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7429f-122">Here is a JSON representation of the resource.</span></span>
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



