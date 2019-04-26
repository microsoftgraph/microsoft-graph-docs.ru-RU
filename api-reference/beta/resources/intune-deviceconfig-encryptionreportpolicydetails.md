---
title: Тип ресурса Енкриптионрепортполицидетаилс
description: Сведения о политике для отчета о шифровании
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c9903b54483fc6f77cd183abee0e54b10acf9cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556300"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="3ee1c-103">Тип ресурса Енкриптионрепортполицидетаилс</span><span class="sxs-lookup"><span data-stu-id="3ee1c-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="3ee1c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ee1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ee1c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ee1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ee1c-106">Сведения о политике для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="3ee1c-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="3ee1c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ee1c-107">Properties</span></span>
|<span data-ttu-id="3ee1c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ee1c-108">Property</span></span>|<span data-ttu-id="3ee1c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3ee1c-109">Type</span></span>|<span data-ttu-id="3ee1c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3ee1c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ee1c-111">Полициид</span><span class="sxs-lookup"><span data-stu-id="3ee1c-111">policyId</span></span>|<span data-ttu-id="3ee1c-112">String</span><span class="sxs-lookup"><span data-stu-id="3ee1c-112">String</span></span>|<span data-ttu-id="3ee1c-113">Идентификатор политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="3ee1c-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="3ee1c-114">policyName</span><span class="sxs-lookup"><span data-stu-id="3ee1c-114">policyName</span></span>|<span data-ttu-id="3ee1c-115">String</span><span class="sxs-lookup"><span data-stu-id="3ee1c-115">String</span></span>|<span data-ttu-id="3ee1c-116">Имя политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="3ee1c-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ee1c-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="3ee1c-117">Relationships</span></span>
<span data-ttu-id="3ee1c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="3ee1c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ee1c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ee1c-119">JSON Representation</span></span>
<span data-ttu-id="3ee1c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ee1c-120">Here is a JSON representation of the resource.</span></span>
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





