---
title: Тип ресурса Енкриптионрепортполицидетаилс
description: Сведения о политике для отчета о шифровании
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7271329a7536a6359bbc9662427e65e21ea39d8b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325612"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="e9fdc-103">Тип ресурса Енкриптионрепортполицидетаилс</span><span class="sxs-lookup"><span data-stu-id="e9fdc-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="e9fdc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9fdc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9fdc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9fdc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9fdc-106">Сведения о политике для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="e9fdc-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="e9fdc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9fdc-107">Properties</span></span>
|<span data-ttu-id="e9fdc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9fdc-108">Property</span></span>|<span data-ttu-id="e9fdc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e9fdc-109">Type</span></span>|<span data-ttu-id="e9fdc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e9fdc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9fdc-111">полициид</span><span class="sxs-lookup"><span data-stu-id="e9fdc-111">policyId</span></span>|<span data-ttu-id="e9fdc-112">String</span><span class="sxs-lookup"><span data-stu-id="e9fdc-112">String</span></span>|<span data-ttu-id="e9fdc-113">Идентификатор политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="e9fdc-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="e9fdc-114">policyName</span><span class="sxs-lookup"><span data-stu-id="e9fdc-114">policyName</span></span>|<span data-ttu-id="e9fdc-115">String</span><span class="sxs-lookup"><span data-stu-id="e9fdc-115">String</span></span>|<span data-ttu-id="e9fdc-116">Имя политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="e9fdc-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9fdc-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="e9fdc-117">Relationships</span></span>
<span data-ttu-id="e9fdc-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e9fdc-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9fdc-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9fdc-119">JSON Representation</span></span>
<span data-ttu-id="e9fdc-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9fdc-120">Here is a JSON representation of the resource.</span></span>
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



