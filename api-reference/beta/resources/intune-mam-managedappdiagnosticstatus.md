---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: tfitzmac
ms.openlocfilehash: 1618c65b46654832fc7706f01cb6d6a9f78926e4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314779"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="e1e56-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="e1e56-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="e1e56-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e1e56-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1e56-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1e56-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1e56-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e1e56-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1e56-107">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="e1e56-107">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="e1e56-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1e56-108">Properties</span></span>
|<span data-ttu-id="e1e56-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1e56-109">Property</span></span>|<span data-ttu-id="e1e56-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e1e56-110">Type</span></span>|<span data-ttu-id="e1e56-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e1e56-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1e56-112">validationName</span><span class="sxs-lookup"><span data-stu-id="e1e56-112">validationName</span></span>|<span data-ttu-id="e1e56-113">String</span><span class="sxs-lookup"><span data-stu-id="e1e56-113">String</span></span>|<span data-ttu-id="e1e56-114">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="e1e56-114">The validation friendly name</span></span>|
|<span data-ttu-id="e1e56-115">state</span><span class="sxs-lookup"><span data-stu-id="e1e56-115">state</span></span>|<span data-ttu-id="e1e56-116">String</span><span class="sxs-lookup"><span data-stu-id="e1e56-116">String</span></span>|<span data-ttu-id="e1e56-117">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="e1e56-117">The state of the operation</span></span>|
|<span data-ttu-id="e1e56-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="e1e56-118">mitigationInstruction</span></span>|<span data-ttu-id="e1e56-119">String</span><span class="sxs-lookup"><span data-stu-id="e1e56-119">String</span></span>|<span data-ttu-id="e1e56-120">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="e1e56-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1e56-121">Связи</span><span class="sxs-lookup"><span data-stu-id="e1e56-121">Relationships</span></span>
<span data-ttu-id="e1e56-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e1e56-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e1e56-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1e56-123">JSON Representation</span></span>
<span data-ttu-id="e1e56-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1e56-124">Here is a JSON representation of the resource.</span></span>
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





