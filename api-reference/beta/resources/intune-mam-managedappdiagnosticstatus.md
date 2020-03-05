---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a701941f4507bdd2378fd2bcf4f441209bdd6869
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527928"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="6bad4-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="6bad4-103">managedAppDiagnosticStatus resource type</span></span>

<span data-ttu-id="6bad4-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6bad4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6bad4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bad4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bad4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6bad4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bad4-107">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="6bad4-107">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="6bad4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6bad4-108">Properties</span></span>
|<span data-ttu-id="6bad4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6bad4-109">Property</span></span>|<span data-ttu-id="6bad4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6bad4-110">Type</span></span>|<span data-ttu-id="6bad4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6bad4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bad4-112">validationName</span><span class="sxs-lookup"><span data-stu-id="6bad4-112">validationName</span></span>|<span data-ttu-id="6bad4-113">String</span><span class="sxs-lookup"><span data-stu-id="6bad4-113">String</span></span>|<span data-ttu-id="6bad4-114">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="6bad4-114">The validation friendly name</span></span>|
|<span data-ttu-id="6bad4-115">state</span><span class="sxs-lookup"><span data-stu-id="6bad4-115">state</span></span>|<span data-ttu-id="6bad4-116">String</span><span class="sxs-lookup"><span data-stu-id="6bad4-116">String</span></span>|<span data-ttu-id="6bad4-117">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="6bad4-117">The state of the operation</span></span>|
|<span data-ttu-id="6bad4-118">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="6bad4-118">mitigationInstruction</span></span>|<span data-ttu-id="6bad4-119">String</span><span class="sxs-lookup"><span data-stu-id="6bad4-119">String</span></span>|<span data-ttu-id="6bad4-120">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="6bad4-120">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bad4-121">Связи</span><span class="sxs-lookup"><span data-stu-id="6bad4-121">Relationships</span></span>
<span data-ttu-id="6bad4-122">Нет</span><span class="sxs-lookup"><span data-stu-id="6bad4-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6bad4-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6bad4-123">JSON Representation</span></span>
<span data-ttu-id="6bad4-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6bad4-124">Here is a JSON representation of the resource.</span></span>
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



