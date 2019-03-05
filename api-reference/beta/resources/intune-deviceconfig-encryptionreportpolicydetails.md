---
title: Тип ресурса Енкриптионрепортполицидетаилс
description: Сведения о политике для отчета о шифровании
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9232acd2a155169385956b9d20b3011c963090a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177919"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="bbeb5-103">Тип ресурса Енкриптионрепортполицидетаилс</span><span class="sxs-lookup"><span data-stu-id="bbeb5-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="bbeb5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbeb5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbeb5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bbeb5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbeb5-106">Сведения о политике для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="bbeb5-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="bbeb5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbeb5-107">Properties</span></span>
|<span data-ttu-id="bbeb5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbeb5-108">Property</span></span>|<span data-ttu-id="bbeb5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bbeb5-109">Type</span></span>|<span data-ttu-id="bbeb5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bbeb5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbeb5-111">Полициид</span><span class="sxs-lookup"><span data-stu-id="bbeb5-111">policyId</span></span>|<span data-ttu-id="bbeb5-112">String</span><span class="sxs-lookup"><span data-stu-id="bbeb5-112">String</span></span>|<span data-ttu-id="bbeb5-113">Идентификатор политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="bbeb5-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="bbeb5-114">policyName</span><span class="sxs-lookup"><span data-stu-id="bbeb5-114">policyName</span></span>|<span data-ttu-id="bbeb5-115">String</span><span class="sxs-lookup"><span data-stu-id="bbeb5-115">String</span></span>|<span data-ttu-id="bbeb5-116">Имя политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="bbeb5-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbeb5-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="bbeb5-117">Relationships</span></span>
<span data-ttu-id="bbeb5-118">Нет</span><span class="sxs-lookup"><span data-stu-id="bbeb5-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbeb5-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bbeb5-119">JSON Representation</span></span>
<span data-ttu-id="bbeb5-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bbeb5-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.encryptionReportPolicyDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.encryptionReportPolicyDetails",
  "policyId": "String",
  "policyName": "String"
}
```




