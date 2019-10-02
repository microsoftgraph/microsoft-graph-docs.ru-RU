---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 33a975318854ab8bfec35ca257ee0c59fc29c188
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356368"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="3f7ac-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="3f7ac-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="3f7ac-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f7ac-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f7ac-105">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="3f7ac-105">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="3f7ac-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f7ac-106">Properties</span></span>
|<span data-ttu-id="3f7ac-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f7ac-107">Property</span></span>|<span data-ttu-id="3f7ac-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3f7ac-108">Type</span></span>|<span data-ttu-id="3f7ac-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3f7ac-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f7ac-110">validationName</span><span class="sxs-lookup"><span data-stu-id="3f7ac-110">validationName</span></span>|<span data-ttu-id="3f7ac-111">String</span><span class="sxs-lookup"><span data-stu-id="3f7ac-111">String</span></span>|<span data-ttu-id="3f7ac-112">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="3f7ac-112">The validation friendly name</span></span>|
|<span data-ttu-id="3f7ac-113">state</span><span class="sxs-lookup"><span data-stu-id="3f7ac-113">state</span></span>|<span data-ttu-id="3f7ac-114">String</span><span class="sxs-lookup"><span data-stu-id="3f7ac-114">String</span></span>|<span data-ttu-id="3f7ac-115">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="3f7ac-115">The state of the operation</span></span>|
|<span data-ttu-id="3f7ac-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="3f7ac-116">mitigationInstruction</span></span>|<span data-ttu-id="3f7ac-117">String</span><span class="sxs-lookup"><span data-stu-id="3f7ac-117">String</span></span>|<span data-ttu-id="3f7ac-118">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="3f7ac-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f7ac-119">Связи</span><span class="sxs-lookup"><span data-stu-id="3f7ac-119">Relationships</span></span>
<span data-ttu-id="3f7ac-120">Нет</span><span class="sxs-lookup"><span data-stu-id="3f7ac-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f7ac-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f7ac-121">JSON Representation</span></span>
<span data-ttu-id="3f7ac-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f7ac-122">Here is a JSON representation of the resource.</span></span>
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




