---
title: Тип ресурса Енкриптионрепортполицидетаилс
description: Сведения о политике для отчета о шифровании
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 874af3d0bf98cbfc5884a4f3387eb8d55323acaf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294580"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="a19f3-103">Тип ресурса Енкриптионрепортполицидетаилс</span><span class="sxs-lookup"><span data-stu-id="a19f3-103">encryptionReportPolicyDetails resource type</span></span>

<span data-ttu-id="a19f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a19f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a19f3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a19f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a19f3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a19f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a19f3-107">Сведения о политике для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="a19f3-107">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="a19f3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a19f3-108">Properties</span></span>
|<span data-ttu-id="a19f3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a19f3-109">Property</span></span>|<span data-ttu-id="a19f3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a19f3-110">Type</span></span>|<span data-ttu-id="a19f3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a19f3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a19f3-112">полициид</span><span class="sxs-lookup"><span data-stu-id="a19f3-112">policyId</span></span>|<span data-ttu-id="a19f3-113">String</span><span class="sxs-lookup"><span data-stu-id="a19f3-113">String</span></span>|<span data-ttu-id="a19f3-114">Идентификатор политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="a19f3-114">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="a19f3-115">policyName</span><span class="sxs-lookup"><span data-stu-id="a19f3-115">policyName</span></span>|<span data-ttu-id="a19f3-116">String</span><span class="sxs-lookup"><span data-stu-id="a19f3-116">String</span></span>|<span data-ttu-id="a19f3-117">Имя политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="a19f3-117">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="a19f3-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a19f3-118">Relationships</span></span>
<span data-ttu-id="a19f3-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a19f3-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a19f3-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a19f3-120">JSON Representation</span></span>
<span data-ttu-id="a19f3-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a19f3-121">Here is a JSON representation of the resource.</span></span>
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




