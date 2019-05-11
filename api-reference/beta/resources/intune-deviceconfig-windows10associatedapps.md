---
title: Тип ресурса windows10AssociatedApps
description: Определение приложения, связанного с Windows 10.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fca7f8876ba0ea455d2bd7f537fe162f125e1dc9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944386"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="58cdf-103">Тип ресурса windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="58cdf-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="58cdf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58cdf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58cdf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58cdf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58cdf-106">Определение приложения, связанного с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="58cdf-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="58cdf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="58cdf-107">Properties</span></span>
|<span data-ttu-id="58cdf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="58cdf-108">Property</span></span>|<span data-ttu-id="58cdf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="58cdf-109">Type</span></span>|<span data-ttu-id="58cdf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="58cdf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58cdf-111">Тип</span><span class="sxs-lookup"><span data-stu-id="58cdf-111">appType</span></span>|[<span data-ttu-id="58cdf-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="58cdf-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="58cdf-113">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="58cdf-113">Application type.</span></span> <span data-ttu-id="58cdf-114">Возможные значения: `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="58cdf-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="58cdf-115">идентификатор</span><span class="sxs-lookup"><span data-stu-id="58cdf-115">identifier</span></span>|<span data-ttu-id="58cdf-116">Строка</span><span class="sxs-lookup"><span data-stu-id="58cdf-116">String</span></span>|<span data-ttu-id="58cdf-117">Идентификацион.</span><span class="sxs-lookup"><span data-stu-id="58cdf-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58cdf-118">Связи</span><span class="sxs-lookup"><span data-stu-id="58cdf-118">Relationships</span></span>
<span data-ttu-id="58cdf-119">Нет</span><span class="sxs-lookup"><span data-stu-id="58cdf-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58cdf-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58cdf-120">JSON Representation</span></span>
<span data-ttu-id="58cdf-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58cdf-121">Here is a JSON representation of the resource.</span></span>
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




