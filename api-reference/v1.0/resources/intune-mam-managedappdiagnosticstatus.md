---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
ms.openlocfilehash: 8a462b49231323288d66a660c769ce7359cb5ab3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026827"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="fa69a-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="fa69a-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="fa69a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fa69a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa69a-105">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="fa69a-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="fa69a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa69a-106">Properties</span></span>
|<span data-ttu-id="fa69a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa69a-107">Property</span></span>|<span data-ttu-id="fa69a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fa69a-108">Type</span></span>|<span data-ttu-id="fa69a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fa69a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa69a-110">validationName</span><span class="sxs-lookup"><span data-stu-id="fa69a-110">validationName</span></span>|<span data-ttu-id="fa69a-111">String</span><span class="sxs-lookup"><span data-stu-id="fa69a-111">String</span></span>|<span data-ttu-id="fa69a-112">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="fa69a-112">The validation friendly name</span></span>|
|<span data-ttu-id="fa69a-113">state</span><span class="sxs-lookup"><span data-stu-id="fa69a-113">state</span></span>|<span data-ttu-id="fa69a-114">String</span><span class="sxs-lookup"><span data-stu-id="fa69a-114">String</span></span>|<span data-ttu-id="fa69a-115">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="fa69a-115">The state of the operation</span></span>|
|<span data-ttu-id="fa69a-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="fa69a-116">mitigationInstruction</span></span>|<span data-ttu-id="fa69a-117">String</span><span class="sxs-lookup"><span data-stu-id="fa69a-117">String</span></span>|<span data-ttu-id="fa69a-118">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="fa69a-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa69a-119">Связи</span><span class="sxs-lookup"><span data-stu-id="fa69a-119">Relationships</span></span>
<span data-ttu-id="fa69a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="fa69a-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fa69a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa69a-121">JSON Representation</span></span>
<span data-ttu-id="fa69a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa69a-122">Here is a JSON representation of the resource.</span></span>
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



