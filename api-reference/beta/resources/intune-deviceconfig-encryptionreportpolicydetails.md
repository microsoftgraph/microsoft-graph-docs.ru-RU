---
title: Тип ресурса Енкриптионрепортполицидетаилс
description: Сведения о политике для отчета о шифровании
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91bebb9449b64ce6a5c2ab6c766171bde60ad737
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526460"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="fb742-103">Тип ресурса Енкриптионрепортполицидетаилс</span><span class="sxs-lookup"><span data-stu-id="fb742-103">encryptionReportPolicyDetails resource type</span></span>

<span data-ttu-id="fb742-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fb742-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb742-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb742-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb742-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb742-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb742-107">Сведения о политике для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="fb742-107">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="fb742-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb742-108">Properties</span></span>
|<span data-ttu-id="fb742-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb742-109">Property</span></span>|<span data-ttu-id="fb742-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fb742-110">Type</span></span>|<span data-ttu-id="fb742-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fb742-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb742-112">полициид</span><span class="sxs-lookup"><span data-stu-id="fb742-112">policyId</span></span>|<span data-ttu-id="fb742-113">String</span><span class="sxs-lookup"><span data-stu-id="fb742-113">String</span></span>|<span data-ttu-id="fb742-114">Идентификатор политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="fb742-114">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="fb742-115">policyName</span><span class="sxs-lookup"><span data-stu-id="fb742-115">policyName</span></span>|<span data-ttu-id="fb742-116">String</span><span class="sxs-lookup"><span data-stu-id="fb742-116">String</span></span>|<span data-ttu-id="fb742-117">Имя политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="fb742-117">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb742-118">Связи</span><span class="sxs-lookup"><span data-stu-id="fb742-118">Relationships</span></span>
<span data-ttu-id="fb742-119">Нет</span><span class="sxs-lookup"><span data-stu-id="fb742-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb742-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb742-120">JSON Representation</span></span>
<span data-ttu-id="fb742-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb742-121">Here is a JSON representation of the resource.</span></span>
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



