---
title: Тип ресурса windows10AssociatedApps
description: Определение приложения, связанного с Windows 10.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d8dc45852b0bd97b7000edd55e74bb9407587d7e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466281"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="2ff2f-103">Тип ресурса windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="2ff2f-103">windows10AssociatedApps resource type</span></span>

<span data-ttu-id="2ff2f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ff2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ff2f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ff2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ff2f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ff2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ff2f-107">Определение приложения, связанного с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="2ff2f-107">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="2ff2f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ff2f-108">Properties</span></span>
|<span data-ttu-id="2ff2f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ff2f-109">Property</span></span>|<span data-ttu-id="2ff2f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2ff2f-110">Type</span></span>|<span data-ttu-id="2ff2f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2ff2f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ff2f-112">Тип</span><span class="sxs-lookup"><span data-stu-id="2ff2f-112">appType</span></span>|[<span data-ttu-id="2ff2f-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="2ff2f-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="2ff2f-114">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="2ff2f-114">Application type.</span></span> <span data-ttu-id="2ff2f-115">Возможные значения: `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="2ff2f-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="2ff2f-116">идентификатор</span><span class="sxs-lookup"><span data-stu-id="2ff2f-116">identifier</span></span>|<span data-ttu-id="2ff2f-117">String</span><span class="sxs-lookup"><span data-stu-id="2ff2f-117">String</span></span>|<span data-ttu-id="2ff2f-118">Идентификацион.</span><span class="sxs-lookup"><span data-stu-id="2ff2f-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ff2f-119">Связи</span><span class="sxs-lookup"><span data-stu-id="2ff2f-119">Relationships</span></span>
<span data-ttu-id="2ff2f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="2ff2f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ff2f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ff2f-121">JSON Representation</span></span>
<span data-ttu-id="2ff2f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ff2f-122">Here is a JSON representation of the resource.</span></span>
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



