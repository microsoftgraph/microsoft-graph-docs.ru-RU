---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a8c7eb75b2bb8b146c9b227562d7b9cdabe8da41
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445757"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="5bbd2-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="5bbd2-103">managedAppDiagnosticStatus resource type</span></span>

<span data-ttu-id="5bbd2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bbd2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5bbd2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5bbd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bbd2-106">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="5bbd2-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="5bbd2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5bbd2-107">Properties</span></span>
|<span data-ttu-id="5bbd2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5bbd2-108">Property</span></span>|<span data-ttu-id="5bbd2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5bbd2-109">Type</span></span>|<span data-ttu-id="5bbd2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5bbd2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bbd2-111">validationName</span><span class="sxs-lookup"><span data-stu-id="5bbd2-111">validationName</span></span>|<span data-ttu-id="5bbd2-112">String</span><span class="sxs-lookup"><span data-stu-id="5bbd2-112">String</span></span>|<span data-ttu-id="5bbd2-113">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="5bbd2-113">The validation friendly name</span></span>|
|<span data-ttu-id="5bbd2-114">state</span><span class="sxs-lookup"><span data-stu-id="5bbd2-114">state</span></span>|<span data-ttu-id="5bbd2-115">String</span><span class="sxs-lookup"><span data-stu-id="5bbd2-115">String</span></span>|<span data-ttu-id="5bbd2-116">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="5bbd2-116">The state of the operation</span></span>|
|<span data-ttu-id="5bbd2-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="5bbd2-117">mitigationInstruction</span></span>|<span data-ttu-id="5bbd2-118">String</span><span class="sxs-lookup"><span data-stu-id="5bbd2-118">String</span></span>|<span data-ttu-id="5bbd2-119">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="5bbd2-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="5bbd2-120">Связи</span><span class="sxs-lookup"><span data-stu-id="5bbd2-120">Relationships</span></span>
<span data-ttu-id="5bbd2-121">Нет</span><span class="sxs-lookup"><span data-stu-id="5bbd2-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5bbd2-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5bbd2-122">JSON Representation</span></span>
<span data-ttu-id="5bbd2-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5bbd2-123">Here is a JSON representation of the resource.</span></span>
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







