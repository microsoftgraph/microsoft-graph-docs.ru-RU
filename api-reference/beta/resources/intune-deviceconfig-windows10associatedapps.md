---
title: Тип ресурса windows10AssociatedApps
description: Определение приложения, связанного с Windows 10.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4c9b8acdfffa9380681dc1db2b25d3e451fcdeae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011374"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="627b2-103">Тип ресурса windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="627b2-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="627b2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="627b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="627b2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="627b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="627b2-106">Определение приложения, связанного с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="627b2-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="627b2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="627b2-107">Properties</span></span>
|<span data-ttu-id="627b2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="627b2-108">Property</span></span>|<span data-ttu-id="627b2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="627b2-109">Type</span></span>|<span data-ttu-id="627b2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="627b2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="627b2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="627b2-111">appType</span></span>|[<span data-ttu-id="627b2-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="627b2-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="627b2-113">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="627b2-113">Application type.</span></span> <span data-ttu-id="627b2-114">Возможные значения: `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="627b2-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="627b2-115">идентификатор</span><span class="sxs-lookup"><span data-stu-id="627b2-115">identifier</span></span>|<span data-ttu-id="627b2-116">String</span><span class="sxs-lookup"><span data-stu-id="627b2-116">String</span></span>|<span data-ttu-id="627b2-117">Идентификацион.</span><span class="sxs-lookup"><span data-stu-id="627b2-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="627b2-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="627b2-118">Relationships</span></span>
<span data-ttu-id="627b2-119">Нет</span><span class="sxs-lookup"><span data-stu-id="627b2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="627b2-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="627b2-120">JSON Representation</span></span>
<span data-ttu-id="627b2-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="627b2-121">Here is a JSON representation of the resource.</span></span>
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





