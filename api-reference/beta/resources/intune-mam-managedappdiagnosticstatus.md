---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 588338589d90ad54db43810d5fd45541cea483eb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459125"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="44c14-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="44c14-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="44c14-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44c14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44c14-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44c14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44c14-106">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="44c14-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="44c14-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="44c14-107">Properties</span></span>
|<span data-ttu-id="44c14-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="44c14-108">Property</span></span>|<span data-ttu-id="44c14-109">Тип</span><span class="sxs-lookup"><span data-stu-id="44c14-109">Type</span></span>|<span data-ttu-id="44c14-110">Описание</span><span class="sxs-lookup"><span data-stu-id="44c14-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44c14-111">validationName</span><span class="sxs-lookup"><span data-stu-id="44c14-111">validationName</span></span>|<span data-ttu-id="44c14-112">String</span><span class="sxs-lookup"><span data-stu-id="44c14-112">String</span></span>|<span data-ttu-id="44c14-113">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="44c14-113">The validation friendly name</span></span>|
|<span data-ttu-id="44c14-114">state</span><span class="sxs-lookup"><span data-stu-id="44c14-114">state</span></span>|<span data-ttu-id="44c14-115">String</span><span class="sxs-lookup"><span data-stu-id="44c14-115">String</span></span>|<span data-ttu-id="44c14-116">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="44c14-116">The state of the operation</span></span>|
|<span data-ttu-id="44c14-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="44c14-117">mitigationInstruction</span></span>|<span data-ttu-id="44c14-118">String</span><span class="sxs-lookup"><span data-stu-id="44c14-118">String</span></span>|<span data-ttu-id="44c14-119">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="44c14-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="44c14-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="44c14-120">Relationships</span></span>
<span data-ttu-id="44c14-121">Нет</span><span class="sxs-lookup"><span data-stu-id="44c14-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44c14-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44c14-122">JSON Representation</span></span>
<span data-ttu-id="44c14-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44c14-123">Here is a JSON representation of the resource.</span></span>
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





