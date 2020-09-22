---
title: Тип ресурса Девицеманажементсеттингфилеконстраинт
description: Ограничение, обеспечивающее расширение файла, приемлемо для данного параметра
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 79936cf26519329563d1216c8f2576faec3e4f77
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061191"
---
# <a name="devicemanagementsettingfileconstraint-resource-type"></a><span data-ttu-id="57c55-103">Тип ресурса Девицеманажементсеттингфилеконстраинт</span><span class="sxs-lookup"><span data-stu-id="57c55-103">deviceManagementSettingFileConstraint resource type</span></span>

<span data-ttu-id="57c55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57c55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57c55-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57c55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57c55-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57c55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57c55-107">Ограничение, обеспечивающее расширение файла, приемлемо для данного параметра</span><span class="sxs-lookup"><span data-stu-id="57c55-107">Constraint enforcing the file extension is acceptable for a given setting</span></span>


<span data-ttu-id="57c55-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="57c55-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="57c55-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="57c55-109">Properties</span></span>
|<span data-ttu-id="57c55-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="57c55-110">Property</span></span>|<span data-ttu-id="57c55-111">Тип</span><span class="sxs-lookup"><span data-stu-id="57c55-111">Type</span></span>|<span data-ttu-id="57c55-112">Описание</span><span class="sxs-lookup"><span data-stu-id="57c55-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57c55-113">суппортедекстенсионс</span><span class="sxs-lookup"><span data-stu-id="57c55-113">supportedExtensions</span></span>|<span data-ttu-id="57c55-114">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="57c55-114">String collection</span></span>|<span data-ttu-id="57c55-115">Допустимые расширения файлов для отправки для этого параметра</span><span class="sxs-lookup"><span data-stu-id="57c55-115">Acceptable file extensions to upload for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="57c55-116">Связи</span><span class="sxs-lookup"><span data-stu-id="57c55-116">Relationships</span></span>
<span data-ttu-id="57c55-117">Нет</span><span class="sxs-lookup"><span data-stu-id="57c55-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57c55-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57c55-118">JSON Representation</span></span>
<span data-ttu-id="57c55-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57c55-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingFileConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingFileConstraint",
  "supportedExtensions": [
    "String"
  ]
}
```






