---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 919b6bdbc5559aff42fae9748e494b57294806b8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332123"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="5597d-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="5597d-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="5597d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5597d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5597d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5597d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5597d-106">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="5597d-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="5597d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5597d-107">Properties</span></span>
|<span data-ttu-id="5597d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5597d-108">Property</span></span>|<span data-ttu-id="5597d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5597d-109">Type</span></span>|<span data-ttu-id="5597d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5597d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5597d-111">validationName</span><span class="sxs-lookup"><span data-stu-id="5597d-111">validationName</span></span>|<span data-ttu-id="5597d-112">String</span><span class="sxs-lookup"><span data-stu-id="5597d-112">String</span></span>|<span data-ttu-id="5597d-113">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="5597d-113">The validation friendly name</span></span>|
|<span data-ttu-id="5597d-114">state</span><span class="sxs-lookup"><span data-stu-id="5597d-114">state</span></span>|<span data-ttu-id="5597d-115">String</span><span class="sxs-lookup"><span data-stu-id="5597d-115">String</span></span>|<span data-ttu-id="5597d-116">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="5597d-116">The state of the operation</span></span>|
|<span data-ttu-id="5597d-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="5597d-117">mitigationInstruction</span></span>|<span data-ttu-id="5597d-118">String</span><span class="sxs-lookup"><span data-stu-id="5597d-118">String</span></span>|<span data-ttu-id="5597d-119">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="5597d-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="5597d-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="5597d-120">Relationships</span></span>
<span data-ttu-id="5597d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="5597d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5597d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5597d-122">JSON Representation</span></span>
<span data-ttu-id="5597d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5597d-123">Here is a JSON representation of the resource.</span></span>
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



