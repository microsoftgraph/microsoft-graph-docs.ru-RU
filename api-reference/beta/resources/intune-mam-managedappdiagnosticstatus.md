---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 907f9940b7cbb4a35f69e0792092e14c99aebdae
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996297"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="f98b1-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="f98b1-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="f98b1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f98b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f98b1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f98b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f98b1-106">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="f98b1-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="f98b1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f98b1-107">Properties</span></span>
|<span data-ttu-id="f98b1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f98b1-108">Property</span></span>|<span data-ttu-id="f98b1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f98b1-109">Type</span></span>|<span data-ttu-id="f98b1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f98b1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f98b1-111">validationName</span><span class="sxs-lookup"><span data-stu-id="f98b1-111">validationName</span></span>|<span data-ttu-id="f98b1-112">String</span><span class="sxs-lookup"><span data-stu-id="f98b1-112">String</span></span>|<span data-ttu-id="f98b1-113">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="f98b1-113">The validation friendly name</span></span>|
|<span data-ttu-id="f98b1-114">state</span><span class="sxs-lookup"><span data-stu-id="f98b1-114">state</span></span>|<span data-ttu-id="f98b1-115">String</span><span class="sxs-lookup"><span data-stu-id="f98b1-115">String</span></span>|<span data-ttu-id="f98b1-116">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="f98b1-116">The state of the operation</span></span>|
|<span data-ttu-id="f98b1-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="f98b1-117">mitigationInstruction</span></span>|<span data-ttu-id="f98b1-118">String</span><span class="sxs-lookup"><span data-stu-id="f98b1-118">String</span></span>|<span data-ttu-id="f98b1-119">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="f98b1-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="f98b1-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="f98b1-120">Relationships</span></span>
<span data-ttu-id="f98b1-121">Нет</span><span class="sxs-lookup"><span data-stu-id="f98b1-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f98b1-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f98b1-122">JSON Representation</span></span>
<span data-ttu-id="f98b1-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f98b1-123">Here is a JSON representation of the resource.</span></span>
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





