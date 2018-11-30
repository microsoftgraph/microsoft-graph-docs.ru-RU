---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
ms.openlocfilehash: 44284b54692e4a123b1837bbfb0f5f04a2b01a2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082276"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="e6ed2-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="e6ed2-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="e6ed2-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e6ed2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6ed2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6ed2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6ed2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e6ed2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6ed2-107">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="e6ed2-107">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="e6ed2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6ed2-108">Properties</span></span>
|<span data-ttu-id="e6ed2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6ed2-109">Property</span></span>|<span data-ttu-id="e6ed2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e6ed2-110">Type</span></span>|<span data-ttu-id="e6ed2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e6ed2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6ed2-112">validationName</span><span class="sxs-lookup"><span data-stu-id="e6ed2-112">validationName</span></span>|<span data-ttu-id="e6ed2-113">String</span><span class="sxs-lookup"><span data-stu-id="e6ed2-113">String</span></span>|<span data-ttu-id="e6ed2-114">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="e6ed2-114">The validation friendly name</span></span>|
|<span data-ttu-id="e6ed2-115">state</span><span class="sxs-lookup"><span data-stu-id="e6ed2-115">state</span></span>|<span data-ttu-id="e6ed2-116">String</span><span class="sxs-lookup"><span data-stu-id="e6ed2-116">String</span></span>|<span data-ttu-id="e6ed2-117">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="e6ed2-117">The state of the operation</span></span>|
|<span data-ttu-id="e6ed2-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="e6ed2-118">mitigationInstruction</span></span>|<span data-ttu-id="e6ed2-119">String</span><span class="sxs-lookup"><span data-stu-id="e6ed2-119">String</span></span>|<span data-ttu-id="e6ed2-120">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="e6ed2-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6ed2-121">Связи</span><span class="sxs-lookup"><span data-stu-id="e6ed2-121">Relationships</span></span>
<span data-ttu-id="e6ed2-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e6ed2-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e6ed2-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6ed2-123">JSON Representation</span></span>
<span data-ttu-id="e6ed2-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6ed2-124">Here is a JSON representation of the resource.</span></span>
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





