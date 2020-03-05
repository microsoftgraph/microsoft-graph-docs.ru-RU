---
title: Тип ресурса Девицеманажементсеттингфилеконстраинт
description: Ограничение, обеспечивающее расширение файла, приемлемо для данного параметра
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1757f3d6d7e6e60a9c45e95e531a142fabbb95f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525252"
---
# <a name="devicemanagementsettingfileconstraint-resource-type"></a><span data-ttu-id="8b87b-103">Тип ресурса Девицеманажементсеттингфилеконстраинт</span><span class="sxs-lookup"><span data-stu-id="8b87b-103">deviceManagementSettingFileConstraint resource type</span></span>

<span data-ttu-id="8b87b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8b87b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b87b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b87b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b87b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b87b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b87b-107">Ограничение, обеспечивающее расширение файла, приемлемо для данного параметра</span><span class="sxs-lookup"><span data-stu-id="8b87b-107">Constraint enforcing the file extension is acceptable for a given setting</span></span>


<span data-ttu-id="8b87b-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="8b87b-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8b87b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b87b-109">Properties</span></span>
|<span data-ttu-id="8b87b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b87b-110">Property</span></span>|<span data-ttu-id="8b87b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8b87b-111">Type</span></span>|<span data-ttu-id="8b87b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8b87b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b87b-113">суппортедекстенсионс</span><span class="sxs-lookup"><span data-stu-id="8b87b-113">supportedExtensions</span></span>|<span data-ttu-id="8b87b-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8b87b-114">String collection</span></span>|<span data-ttu-id="8b87b-115">Допустимые расширения файлов для отправки для этого параметра</span><span class="sxs-lookup"><span data-stu-id="8b87b-115">Acceptable file extensions to upload for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b87b-116">Связи</span><span class="sxs-lookup"><span data-stu-id="8b87b-116">Relationships</span></span>
<span data-ttu-id="8b87b-117">Нет</span><span class="sxs-lookup"><span data-stu-id="8b87b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b87b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b87b-118">JSON Representation</span></span>
<span data-ttu-id="8b87b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b87b-119">Here is a JSON representation of the resource.</span></span>
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



