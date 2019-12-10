---
title: Тип ресурса Девицеманажементсеттингфилеконстраинт
description: Ограничение, обеспечивающее расширение файла, приемлемо для данного параметра
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60ff6a00e30e328daf2330e39511956ec1ab1f18
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39924628"
---
# <a name="devicemanagementsettingfileconstraint-resource-type"></a><span data-ttu-id="db468-103">Тип ресурса Девицеманажементсеттингфилеконстраинт</span><span class="sxs-lookup"><span data-stu-id="db468-103">deviceManagementSettingFileConstraint resource type</span></span>

> <span data-ttu-id="db468-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db468-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db468-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db468-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db468-106">Ограничение, обеспечивающее расширение файла, приемлемо для данного параметра</span><span class="sxs-lookup"><span data-stu-id="db468-106">Constraint enforcing the file extension is acceptable for a given setting</span></span>


<span data-ttu-id="db468-107">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="db468-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="db468-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="db468-108">Properties</span></span>
|<span data-ttu-id="db468-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="db468-109">Property</span></span>|<span data-ttu-id="db468-110">Тип</span><span class="sxs-lookup"><span data-stu-id="db468-110">Type</span></span>|<span data-ttu-id="db468-111">Описание</span><span class="sxs-lookup"><span data-stu-id="db468-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db468-112">суппортедекстенсионс</span><span class="sxs-lookup"><span data-stu-id="db468-112">supportedExtensions</span></span>|<span data-ttu-id="db468-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="db468-113">String collection</span></span>|<span data-ttu-id="db468-114">Допустимые расширения файлов для отправки для этого параметра</span><span class="sxs-lookup"><span data-stu-id="db468-114">Acceptable file extensions to upload for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="db468-115">Связи</span><span class="sxs-lookup"><span data-stu-id="db468-115">Relationships</span></span>
<span data-ttu-id="db468-116">Нет</span><span class="sxs-lookup"><span data-stu-id="db468-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db468-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db468-117">JSON Representation</span></span>
<span data-ttu-id="db468-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db468-118">Here is a JSON representation of the resource.</span></span>
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



