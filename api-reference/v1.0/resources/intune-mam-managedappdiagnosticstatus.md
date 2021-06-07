---
title: Тип ресурса managedAppDiagnosticStatus
description: Представляет состояние диагностики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 824bcb13741240b1f5bc462312004892ccd5c051
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751323"
---
# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="06099-103">Тип ресурса managedAppDiagnosticStatus</span><span class="sxs-lookup"><span data-stu-id="06099-103">managedAppDiagnosticStatus resource type</span></span>

<span data-ttu-id="06099-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06099-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06099-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06099-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06099-106">Представляет состояние диагностики.</span><span class="sxs-lookup"><span data-stu-id="06099-106">Represents diagnostics status.</span></span>

## <a name="properties"></a><span data-ttu-id="06099-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="06099-107">Properties</span></span>
|<span data-ttu-id="06099-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="06099-108">Property</span></span>|<span data-ttu-id="06099-109">Тип</span><span class="sxs-lookup"><span data-stu-id="06099-109">Type</span></span>|<span data-ttu-id="06099-110">Описание</span><span class="sxs-lookup"><span data-stu-id="06099-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06099-111">validationName</span><span class="sxs-lookup"><span data-stu-id="06099-111">validationName</span></span>|<span data-ttu-id="06099-112">String</span><span class="sxs-lookup"><span data-stu-id="06099-112">String</span></span>|<span data-ttu-id="06099-113">Понятное имя проверки</span><span class="sxs-lookup"><span data-stu-id="06099-113">The validation friendly name</span></span>|
|<span data-ttu-id="06099-114">state</span><span class="sxs-lookup"><span data-stu-id="06099-114">state</span></span>|<span data-ttu-id="06099-115">String</span><span class="sxs-lookup"><span data-stu-id="06099-115">String</span></span>|<span data-ttu-id="06099-116">Состояние операции</span><span class="sxs-lookup"><span data-stu-id="06099-116">The state of the operation</span></span>|
|<span data-ttu-id="06099-117">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="06099-117">mitigationInstruction</span></span>|<span data-ttu-id="06099-118">String</span><span class="sxs-lookup"><span data-stu-id="06099-118">String</span></span>|<span data-ttu-id="06099-119">Инструкции по исправлению неудачной проверки</span><span class="sxs-lookup"><span data-stu-id="06099-119">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="06099-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="06099-120">Relationships</span></span>
<span data-ttu-id="06099-121">Нет</span><span class="sxs-lookup"><span data-stu-id="06099-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06099-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06099-122">JSON Representation</span></span>
<span data-ttu-id="06099-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06099-123">Here is a JSON representation of the resource.</span></span>
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




