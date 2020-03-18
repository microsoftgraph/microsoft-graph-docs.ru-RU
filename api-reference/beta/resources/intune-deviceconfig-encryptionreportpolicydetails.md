---
title: Тип ресурса Енкриптионрепортполицидетаилс
description: Сведения о политике для отчета о шифровании
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd802c6a13789f9179d4f2940bc78a80f1ff15d0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791788"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="c89b4-103">Тип ресурса Енкриптионрепортполицидетаилс</span><span class="sxs-lookup"><span data-stu-id="c89b4-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="c89b4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c89b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c89b4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c89b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c89b4-106">Сведения о политике для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="c89b4-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="c89b4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c89b4-107">Properties</span></span>
|<span data-ttu-id="c89b4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c89b4-108">Property</span></span>|<span data-ttu-id="c89b4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c89b4-109">Type</span></span>|<span data-ttu-id="c89b4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c89b4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c89b4-111">полициид</span><span class="sxs-lookup"><span data-stu-id="c89b4-111">policyId</span></span>|<span data-ttu-id="c89b4-112">String</span><span class="sxs-lookup"><span data-stu-id="c89b4-112">String</span></span>|<span data-ttu-id="c89b4-113">Идентификатор политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="c89b4-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="c89b4-114">policyName</span><span class="sxs-lookup"><span data-stu-id="c89b4-114">policyName</span></span>|<span data-ttu-id="c89b4-115">String</span><span class="sxs-lookup"><span data-stu-id="c89b4-115">String</span></span>|<span data-ttu-id="c89b4-116">Имя политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="c89b4-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="c89b4-117">Связи</span><span class="sxs-lookup"><span data-stu-id="c89b4-117">Relationships</span></span>
<span data-ttu-id="c89b4-118">Нет</span><span class="sxs-lookup"><span data-stu-id="c89b4-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c89b4-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c89b4-119">JSON Representation</span></span>
<span data-ttu-id="c89b4-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c89b4-120">Here is a JSON representation of the resource.</span></span>
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



