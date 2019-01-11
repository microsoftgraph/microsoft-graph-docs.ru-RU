---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f471a71c10a225f2bb5af77399932402f154538d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872123"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="0f671-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="0f671-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="0f671-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0f671-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f671-105">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="0f671-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="0f671-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f671-106">Properties</span></span>
|<span data-ttu-id="0f671-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f671-107">Property</span></span>|<span data-ttu-id="0f671-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0f671-108">Type</span></span>|<span data-ttu-id="0f671-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0f671-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f671-110">validationName</span><span class="sxs-lookup"><span data-stu-id="0f671-110">validationName</span></span>|<span data-ttu-id="0f671-111">String</span><span class="sxs-lookup"><span data-stu-id="0f671-111">String</span></span>|<span data-ttu-id="0f671-112">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="0f671-112">The validation friendly name</span></span>|
|<span data-ttu-id="0f671-113">state</span><span class="sxs-lookup"><span data-stu-id="0f671-113">state</span></span>|<span data-ttu-id="0f671-114">String</span><span class="sxs-lookup"><span data-stu-id="0f671-114">String</span></span>|<span data-ttu-id="0f671-115">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="0f671-115">The state of the operation</span></span>|
|<span data-ttu-id="0f671-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="0f671-116">mitigationInstruction</span></span>|<span data-ttu-id="0f671-117">String</span><span class="sxs-lookup"><span data-stu-id="0f671-117">String</span></span>|<span data-ttu-id="0f671-118">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="0f671-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f671-119">Связи</span><span class="sxs-lookup"><span data-stu-id="0f671-119">Relationships</span></span>
<span data-ttu-id="0f671-120">Нет</span><span class="sxs-lookup"><span data-stu-id="0f671-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f671-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f671-121">JSON Representation</span></span>
<span data-ttu-id="0f671-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f671-122">Here is a JSON representation of the resource.</span></span>
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



