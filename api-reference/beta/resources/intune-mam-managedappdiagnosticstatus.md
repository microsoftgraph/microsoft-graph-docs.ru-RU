---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 98bd1353156c99861749bdb7eac2e686cf96532e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869792"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="cfb3c-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="cfb3c-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="cfb3c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cfb3c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cfb3c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfb3c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cfb3c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cfb3c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cfb3c-107">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="cfb3c-107">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="cfb3c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cfb3c-108">Properties</span></span>
|<span data-ttu-id="cfb3c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cfb3c-109">Property</span></span>|<span data-ttu-id="cfb3c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cfb3c-110">Type</span></span>|<span data-ttu-id="cfb3c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cfb3c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfb3c-112">validationName</span><span class="sxs-lookup"><span data-stu-id="cfb3c-112">validationName</span></span>|<span data-ttu-id="cfb3c-113">String</span><span class="sxs-lookup"><span data-stu-id="cfb3c-113">String</span></span>|<span data-ttu-id="cfb3c-114">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="cfb3c-114">The validation friendly name</span></span>|
|<span data-ttu-id="cfb3c-115">state</span><span class="sxs-lookup"><span data-stu-id="cfb3c-115">state</span></span>|<span data-ttu-id="cfb3c-116">String</span><span class="sxs-lookup"><span data-stu-id="cfb3c-116">String</span></span>|<span data-ttu-id="cfb3c-117">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="cfb3c-117">The state of the operation</span></span>|
|<span data-ttu-id="cfb3c-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="cfb3c-118">mitigationInstruction</span></span>|<span data-ttu-id="cfb3c-119">String</span><span class="sxs-lookup"><span data-stu-id="cfb3c-119">String</span></span>|<span data-ttu-id="cfb3c-120">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="cfb3c-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfb3c-121">Связи</span><span class="sxs-lookup"><span data-stu-id="cfb3c-121">Relationships</span></span>
<span data-ttu-id="cfb3c-122">Нет</span><span class="sxs-lookup"><span data-stu-id="cfb3c-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cfb3c-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cfb3c-123">JSON Representation</span></span>
<span data-ttu-id="cfb3c-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cfb3c-124">Here is a JSON representation of the resource.</span></span>
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





