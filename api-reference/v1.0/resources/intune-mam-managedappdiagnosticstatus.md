---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: tfitzmac
ms.openlocfilehash: 7f0cd0d5b11c4d902f51dd422add2373e8e8df9e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340686"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="dad07-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="dad07-103">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="dad07-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dad07-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dad07-105">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="dad07-105">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="dad07-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="dad07-106">Properties</span></span>
|<span data-ttu-id="dad07-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="dad07-107">Property</span></span>|<span data-ttu-id="dad07-108">Тип</span><span class="sxs-lookup"><span data-stu-id="dad07-108">Type</span></span>|<span data-ttu-id="dad07-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dad07-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dad07-110">validationName</span><span class="sxs-lookup"><span data-stu-id="dad07-110">validationName</span></span>|<span data-ttu-id="dad07-111">String</span><span class="sxs-lookup"><span data-stu-id="dad07-111">String</span></span>|<span data-ttu-id="dad07-112">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="dad07-112">The validation friendly name</span></span>|
|<span data-ttu-id="dad07-113">state</span><span class="sxs-lookup"><span data-stu-id="dad07-113">state</span></span>|<span data-ttu-id="dad07-114">String</span><span class="sxs-lookup"><span data-stu-id="dad07-114">String</span></span>|<span data-ttu-id="dad07-115">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="dad07-115">The state of the operation</span></span>|
|<span data-ttu-id="dad07-116">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="dad07-116">mitigationInstruction</span></span>|<span data-ttu-id="dad07-117">String</span><span class="sxs-lookup"><span data-stu-id="dad07-117">String</span></span>|<span data-ttu-id="dad07-118">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="dad07-118">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="dad07-119">Связи</span><span class="sxs-lookup"><span data-stu-id="dad07-119">Relationships</span></span>
<span data-ttu-id="dad07-120">Нет</span><span class="sxs-lookup"><span data-stu-id="dad07-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dad07-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dad07-121">JSON Representation</span></span>
<span data-ttu-id="dad07-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dad07-122">Here is a JSON representation of the resource.</span></span>
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



