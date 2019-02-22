---
title: Тип ресурса windows10AssociatedApps
description: Определение приложения, связанного с Windows 10.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 95f0114bbd39e85c137da2a71b7640ba8051b6dc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146685"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="50dcd-103">Тип ресурса windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="50dcd-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="50dcd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50dcd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50dcd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50dcd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50dcd-106">Определение приложения, связанного с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="50dcd-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="50dcd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="50dcd-107">Properties</span></span>
|<span data-ttu-id="50dcd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="50dcd-108">Property</span></span>|<span data-ttu-id="50dcd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="50dcd-109">Type</span></span>|<span data-ttu-id="50dcd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="50dcd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50dcd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="50dcd-111">appType</span></span>|[<span data-ttu-id="50dcd-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="50dcd-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="50dcd-113">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="50dcd-113">Application type.</span></span> <span data-ttu-id="50dcd-114">Возможные значения: `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="50dcd-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="50dcd-115">идентификатор</span><span class="sxs-lookup"><span data-stu-id="50dcd-115">identifier</span></span>|<span data-ttu-id="50dcd-116">String</span><span class="sxs-lookup"><span data-stu-id="50dcd-116">String</span></span>|<span data-ttu-id="50dcd-117">Идентификацион.</span><span class="sxs-lookup"><span data-stu-id="50dcd-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50dcd-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="50dcd-118">Relationships</span></span>
<span data-ttu-id="50dcd-119">Нет</span><span class="sxs-lookup"><span data-stu-id="50dcd-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50dcd-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50dcd-120">JSON Representation</span></span>
<span data-ttu-id="50dcd-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50dcd-121">Here is a JSON representation of the resource.</span></span>
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




