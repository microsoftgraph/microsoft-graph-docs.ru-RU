---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 74743a345688699ac25399e92af53f17afe86626
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030341"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="6649b-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="6649b-103">managedAppDiagnosticStatus resource type</span></span>

<span data-ttu-id="6649b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6649b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6649b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6649b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6649b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6649b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6649b-107">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="6649b-107">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="6649b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6649b-108">Properties</span></span>
|<span data-ttu-id="6649b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6649b-109">Property</span></span>|<span data-ttu-id="6649b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6649b-110">Type</span></span>|<span data-ttu-id="6649b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6649b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6649b-112">validationName</span><span class="sxs-lookup"><span data-stu-id="6649b-112">validationName</span></span>|<span data-ttu-id="6649b-113">String</span><span class="sxs-lookup"><span data-stu-id="6649b-113">String</span></span>|<span data-ttu-id="6649b-114">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="6649b-114">The validation friendly name</span></span>|
|<span data-ttu-id="6649b-115">state</span><span class="sxs-lookup"><span data-stu-id="6649b-115">state</span></span>|<span data-ttu-id="6649b-116">String</span><span class="sxs-lookup"><span data-stu-id="6649b-116">String</span></span>|<span data-ttu-id="6649b-117">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="6649b-117">The state of the operation</span></span>|
|<span data-ttu-id="6649b-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="6649b-118">mitigationInstruction</span></span>|<span data-ttu-id="6649b-119">String</span><span class="sxs-lookup"><span data-stu-id="6649b-119">String</span></span>|<span data-ttu-id="6649b-120">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="6649b-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="6649b-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="6649b-121">Relationships</span></span>
<span data-ttu-id="6649b-122">Нет</span><span class="sxs-lookup"><span data-stu-id="6649b-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6649b-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6649b-123">JSON Representation</span></span>
<span data-ttu-id="6649b-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6649b-124">Here is a JSON representation of the resource.</span></span>
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






