---
title: Тип ресурса windows10AssociatedApps
description: Определение приложения, связанного с Windows 10.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 44b754ba08e8fde1366fda67640582d8552bc4f3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787209"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="1c8f9-103">Тип ресурса windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="1c8f9-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="1c8f9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c8f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c8f9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c8f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c8f9-106">Определение приложения, связанного с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="1c8f9-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="1c8f9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c8f9-107">Properties</span></span>
|<span data-ttu-id="1c8f9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c8f9-108">Property</span></span>|<span data-ttu-id="1c8f9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1c8f9-109">Type</span></span>|<span data-ttu-id="1c8f9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1c8f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c8f9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1c8f9-111">appType</span></span>|[<span data-ttu-id="1c8f9-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="1c8f9-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="1c8f9-113">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="1c8f9-113">Application type.</span></span> <span data-ttu-id="1c8f9-114">Возможные значения: `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="1c8f9-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="1c8f9-115">идентификатор</span><span class="sxs-lookup"><span data-stu-id="1c8f9-115">identifier</span></span>|<span data-ttu-id="1c8f9-116">String</span><span class="sxs-lookup"><span data-stu-id="1c8f9-116">String</span></span>|<span data-ttu-id="1c8f9-117">Идентификацион.</span><span class="sxs-lookup"><span data-stu-id="1c8f9-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c8f9-118">Связи</span><span class="sxs-lookup"><span data-stu-id="1c8f9-118">Relationships</span></span>
<span data-ttu-id="1c8f9-119">Нет</span><span class="sxs-lookup"><span data-stu-id="1c8f9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c8f9-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1c8f9-120">JSON Representation</span></span>
<span data-ttu-id="1c8f9-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c8f9-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```



