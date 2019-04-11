---
title: Тип ресурса windows10AssociatedApps
description: Определение приложения, связанного с Windows 10.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22adbc6be90718f95a574443c8bd2f96a55f2ee4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784644"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="2d3d0-103">Тип ресурса windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="2d3d0-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="2d3d0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d3d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d3d0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d3d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d3d0-106">Определение приложения, связанного с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="2d3d0-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="2d3d0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d3d0-107">Properties</span></span>
|<span data-ttu-id="2d3d0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d3d0-108">Property</span></span>|<span data-ttu-id="2d3d0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2d3d0-109">Type</span></span>|<span data-ttu-id="2d3d0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2d3d0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d3d0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2d3d0-111">appType</span></span>|[<span data-ttu-id="2d3d0-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="2d3d0-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="2d3d0-113">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="2d3d0-113">Application type.</span></span> <span data-ttu-id="2d3d0-114">Возможные значения: `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="2d3d0-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="2d3d0-115">идентификатор</span><span class="sxs-lookup"><span data-stu-id="2d3d0-115">identifier</span></span>|<span data-ttu-id="2d3d0-116">String</span><span class="sxs-lookup"><span data-stu-id="2d3d0-116">String</span></span>|<span data-ttu-id="2d3d0-117">Идентификацион.</span><span class="sxs-lookup"><span data-stu-id="2d3d0-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d3d0-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="2d3d0-118">Relationships</span></span>
<span data-ttu-id="2d3d0-119">Нет</span><span class="sxs-lookup"><span data-stu-id="2d3d0-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d3d0-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d3d0-120">JSON Representation</span></span>
<span data-ttu-id="2d3d0-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d3d0-121">Here is a JSON representation of the resource.</span></span>
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





