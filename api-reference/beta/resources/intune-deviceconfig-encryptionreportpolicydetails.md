---
title: Тип ресурса Енкриптионрепортполицидетаилс
description: Сведения о политике для отчета о шифровании
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9f84f3a0ca0d4b79d73f62dc0607fd332e90e07c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705913"
---
# <a name="encryptionreportpolicydetails-resource-type"></a><span data-ttu-id="ca3fc-103">Тип ресурса Енкриптионрепортполицидетаилс</span><span class="sxs-lookup"><span data-stu-id="ca3fc-103">encryptionReportPolicyDetails resource type</span></span>

<span data-ttu-id="ca3fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca3fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca3fc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca3fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca3fc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca3fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca3fc-107">Сведения о политике для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="ca3fc-107">Policy Details for Encryption Report</span></span>

## <a name="properties"></a><span data-ttu-id="ca3fc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca3fc-108">Properties</span></span>
|<span data-ttu-id="ca3fc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca3fc-109">Property</span></span>|<span data-ttu-id="ca3fc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ca3fc-110">Type</span></span>|<span data-ttu-id="ca3fc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ca3fc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca3fc-112">полициид</span><span class="sxs-lookup"><span data-stu-id="ca3fc-112">policyId</span></span>|<span data-ttu-id="ca3fc-113">Строка</span><span class="sxs-lookup"><span data-stu-id="ca3fc-113">String</span></span>|<span data-ttu-id="ca3fc-114">Идентификатор политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="ca3fc-114">Policy Id for Encryption Report</span></span>|
|<span data-ttu-id="ca3fc-115">policyName</span><span class="sxs-lookup"><span data-stu-id="ca3fc-115">policyName</span></span>|<span data-ttu-id="ca3fc-116">Строка</span><span class="sxs-lookup"><span data-stu-id="ca3fc-116">String</span></span>|<span data-ttu-id="ca3fc-117">Имя политики для отчета о шифровании</span><span class="sxs-lookup"><span data-stu-id="ca3fc-117">Policy Name for Encryption Report</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca3fc-118">Связи</span><span class="sxs-lookup"><span data-stu-id="ca3fc-118">Relationships</span></span>
<span data-ttu-id="ca3fc-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ca3fc-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca3fc-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca3fc-120">JSON Representation</span></span>
<span data-ttu-id="ca3fc-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca3fc-121">Here is a JSON representation of the resource.</span></span>
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





