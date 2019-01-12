---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 210edaf8eb039db928d612337aa7c8e0642c9ee3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987190"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="82292-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="82292-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="82292-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="82292-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82292-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82292-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82292-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="82292-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82292-107">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="82292-107">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="82292-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="82292-108">Properties</span></span>
|<span data-ttu-id="82292-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="82292-109">Property</span></span>|<span data-ttu-id="82292-110">Тип</span><span class="sxs-lookup"><span data-stu-id="82292-110">Type</span></span>|<span data-ttu-id="82292-111">Описание</span><span class="sxs-lookup"><span data-stu-id="82292-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82292-112">validationName</span><span class="sxs-lookup"><span data-stu-id="82292-112">validationName</span></span>|<span data-ttu-id="82292-113">String</span><span class="sxs-lookup"><span data-stu-id="82292-113">String</span></span>|<span data-ttu-id="82292-114">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="82292-114">The validation friendly name</span></span>|
|<span data-ttu-id="82292-115">state</span><span class="sxs-lookup"><span data-stu-id="82292-115">state</span></span>|<span data-ttu-id="82292-116">String</span><span class="sxs-lookup"><span data-stu-id="82292-116">String</span></span>|<span data-ttu-id="82292-117">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="82292-117">The state of the operation</span></span>|
|<span data-ttu-id="82292-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="82292-118">mitigationInstruction</span></span>|<span data-ttu-id="82292-119">String</span><span class="sxs-lookup"><span data-stu-id="82292-119">String</span></span>|<span data-ttu-id="82292-120">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="82292-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="82292-121">Связи</span><span class="sxs-lookup"><span data-stu-id="82292-121">Relationships</span></span>
<span data-ttu-id="82292-122">Нет</span><span class="sxs-lookup"><span data-stu-id="82292-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="82292-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="82292-123">JSON Representation</span></span>
<span data-ttu-id="82292-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82292-124">Here is a JSON representation of the resource.</span></span>
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





