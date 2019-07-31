---
title: Тип ресурса Енкриптионрепортполицидетаилс
description: Сведения о политике для отчета о шифровании
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d1484e1ed55abb14daccb61e024dc94eb415e031
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004374"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="5b993-103">Тип ресурса Енкриптионрепортполицидетаилс</span><span class="sxs-lookup"><span data-stu-id="5b993-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="5b993-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b993-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b993-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b993-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b993-106">Сведения о политике для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="5b993-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="5b993-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b993-107">Properties</span></span>
|<span data-ttu-id="5b993-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b993-108">Property</span></span>|<span data-ttu-id="5b993-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5b993-109">Type</span></span>|<span data-ttu-id="5b993-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5b993-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b993-111">Полициид</span><span class="sxs-lookup"><span data-stu-id="5b993-111">policyId</span></span>|<span data-ttu-id="5b993-112">String</span><span class="sxs-lookup"><span data-stu-id="5b993-112">String</span></span>|<span data-ttu-id="5b993-113">Идентификатор политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="5b993-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="5b993-114">policyName</span><span class="sxs-lookup"><span data-stu-id="5b993-114">policyName</span></span>|<span data-ttu-id="5b993-115">String</span><span class="sxs-lookup"><span data-stu-id="5b993-115">String</span></span>|<span data-ttu-id="5b993-116">Имя политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="5b993-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b993-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="5b993-117">Relationships</span></span>
<span data-ttu-id="5b993-118">Нет</span><span class="sxs-lookup"><span data-stu-id="5b993-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b993-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b993-119">JSON Representation</span></span>
<span data-ttu-id="5b993-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b993-120">Here is a JSON representation of the resource.</span></span>
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





