---
title: Тип ресурса windows10AssociatedApps
description: Определение приложения, связанного с Windows 10.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b53f2b2ec70a2d7420a754a795905da5b1dcb4a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992754"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="80c60-103">Тип ресурса windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="80c60-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="80c60-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80c60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80c60-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="80c60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80c60-106">Определение приложения, связанного с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="80c60-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="80c60-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="80c60-107">Properties</span></span>
|<span data-ttu-id="80c60-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="80c60-108">Property</span></span>|<span data-ttu-id="80c60-109">Тип</span><span class="sxs-lookup"><span data-stu-id="80c60-109">Type</span></span>|<span data-ttu-id="80c60-110">Описание</span><span class="sxs-lookup"><span data-stu-id="80c60-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80c60-111">Тип</span><span class="sxs-lookup"><span data-stu-id="80c60-111">appType</span></span>|[<span data-ttu-id="80c60-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="80c60-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="80c60-113">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="80c60-113">Application type.</span></span> <span data-ttu-id="80c60-114">Возможные значения: `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="80c60-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="80c60-115">идентификатор</span><span class="sxs-lookup"><span data-stu-id="80c60-115">identifier</span></span>|<span data-ttu-id="80c60-116">String</span><span class="sxs-lookup"><span data-stu-id="80c60-116">String</span></span>|<span data-ttu-id="80c60-117">Идентификацион.</span><span class="sxs-lookup"><span data-stu-id="80c60-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80c60-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="80c60-118">Relationships</span></span>
<span data-ttu-id="80c60-119">Нет</span><span class="sxs-lookup"><span data-stu-id="80c60-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80c60-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80c60-120">JSON Representation</span></span>
<span data-ttu-id="80c60-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80c60-121">Here is a JSON representation of the resource.</span></span>
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





