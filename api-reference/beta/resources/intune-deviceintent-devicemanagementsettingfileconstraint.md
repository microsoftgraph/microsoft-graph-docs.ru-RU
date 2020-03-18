---
title: Тип ресурса Девицеманажементсеттингфилеконстраинт
description: Ограничение, обеспечивающее расширение файла, приемлемо для данного параметра
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9a9e5a3f4ce8cec54dbdd0f1a690b039b2da0524
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785325"
---
# <a name="devicemanagementsettingfileconstraint-resource-type"></a><span data-ttu-id="a8cbc-103">Тип ресурса Девицеманажементсеттингфилеконстраинт</span><span class="sxs-lookup"><span data-stu-id="a8cbc-103">deviceManagementSettingFileConstraint resource type</span></span>

> <span data-ttu-id="a8cbc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8cbc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8cbc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8cbc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8cbc-106">Ограничение, обеспечивающее расширение файла, приемлемо для данного параметра</span><span class="sxs-lookup"><span data-stu-id="a8cbc-106">Constraint enforcing the file extension is acceptable for a given setting</span></span>


<span data-ttu-id="a8cbc-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="a8cbc-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a8cbc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8cbc-108">Properties</span></span>
|<span data-ttu-id="a8cbc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8cbc-109">Property</span></span>|<span data-ttu-id="a8cbc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a8cbc-110">Type</span></span>|<span data-ttu-id="a8cbc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a8cbc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8cbc-112">суппортедекстенсионс</span><span class="sxs-lookup"><span data-stu-id="a8cbc-112">supportedExtensions</span></span>|<span data-ttu-id="a8cbc-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a8cbc-113">String collection</span></span>|<span data-ttu-id="a8cbc-114">Допустимые расширения файлов для отправки для этого параметра</span><span class="sxs-lookup"><span data-stu-id="a8cbc-114">Acceptable file extensions to upload for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8cbc-115">Связи</span><span class="sxs-lookup"><span data-stu-id="a8cbc-115">Relationships</span></span>
<span data-ttu-id="a8cbc-116">Нет</span><span class="sxs-lookup"><span data-stu-id="a8cbc-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8cbc-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8cbc-117">JSON Representation</span></span>
<span data-ttu-id="a8cbc-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8cbc-118">Here is a JSON representation of the resource.</span></span>
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



