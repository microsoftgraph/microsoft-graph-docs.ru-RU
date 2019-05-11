---
title: Тип ресурса Енкриптионрепортполицидетаилс
description: Сведения о политике для отчета о шифровании
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ddca213c3de3c004a19ebc3877aed1542604933e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946646"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="c985f-103">Тип ресурса Енкриптионрепортполицидетаилс</span><span class="sxs-lookup"><span data-stu-id="c985f-103">encryptionReportPolicyDetails resource type</span></span>

> <span data-ttu-id="c985f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c985f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c985f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c985f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c985f-106">Сведения о политике для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="c985f-106">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="c985f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c985f-107">Properties</span></span>
|<span data-ttu-id="c985f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c985f-108">Property</span></span>|<span data-ttu-id="c985f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c985f-109">Type</span></span>|<span data-ttu-id="c985f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c985f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c985f-111">Полициид</span><span class="sxs-lookup"><span data-stu-id="c985f-111">policyId</span></span>|<span data-ttu-id="c985f-112">Строка</span><span class="sxs-lookup"><span data-stu-id="c985f-112">String</span></span>|<span data-ttu-id="c985f-113">Идентификатор политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="c985f-113">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="c985f-114">policyName</span><span class="sxs-lookup"><span data-stu-id="c985f-114">policyName</span></span>|<span data-ttu-id="c985f-115">Строка</span><span class="sxs-lookup"><span data-stu-id="c985f-115">String</span></span>|<span data-ttu-id="c985f-116">Имя политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="c985f-116">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="c985f-117">Связи</span><span class="sxs-lookup"><span data-stu-id="c985f-117">Relationships</span></span>
<span data-ttu-id="c985f-118">Нет</span><span class="sxs-lookup"><span data-stu-id="c985f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c985f-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c985f-119">JSON Representation</span></span>
<span data-ttu-id="c985f-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c985f-120">Here is a JSON representation of the resource.</span></span>
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




