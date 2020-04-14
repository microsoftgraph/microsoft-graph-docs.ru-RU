---
title: Тип ресурса Енкриптионрепортполицидетаилс
description: Сведения о политике для отчета о шифровании
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8a92037429908af4ff53ea45b9b5f9b65a5a436
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460067"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="09ca7-103">Тип ресурса Енкриптионрепортполицидетаилс</span><span class="sxs-lookup"><span data-stu-id="09ca7-103">encryptionReportPolicyDetails resource type</span></span>

<span data-ttu-id="09ca7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09ca7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09ca7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09ca7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09ca7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09ca7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09ca7-107">Сведения о политике для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="09ca7-107">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="09ca7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="09ca7-108">Properties</span></span>
|<span data-ttu-id="09ca7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="09ca7-109">Property</span></span>|<span data-ttu-id="09ca7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="09ca7-110">Type</span></span>|<span data-ttu-id="09ca7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="09ca7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09ca7-112">полициид</span><span class="sxs-lookup"><span data-stu-id="09ca7-112">policyId</span></span>|<span data-ttu-id="09ca7-113">String</span><span class="sxs-lookup"><span data-stu-id="09ca7-113">String</span></span>|<span data-ttu-id="09ca7-114">Идентификатор политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="09ca7-114">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="09ca7-115">policyName</span><span class="sxs-lookup"><span data-stu-id="09ca7-115">policyName</span></span>|<span data-ttu-id="09ca7-116">String</span><span class="sxs-lookup"><span data-stu-id="09ca7-116">String</span></span>|<span data-ttu-id="09ca7-117">Имя политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="09ca7-117">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="09ca7-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="09ca7-118">Relationships</span></span>
<span data-ttu-id="09ca7-119">Нет</span><span class="sxs-lookup"><span data-stu-id="09ca7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09ca7-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09ca7-120">JSON Representation</span></span>
<span data-ttu-id="09ca7-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09ca7-121">Here is a JSON representation of the resource.</span></span>
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



