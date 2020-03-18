---
title: Тип ресурса Манажеддевицерепортедапп
description: Данные приложения для создания отчетов
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6704e4f2f8796be6c246d6deb6f5e0e8821ba411
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788613"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="83565-103">Тип ресурса Манажеддевицерепортедапп</span><span class="sxs-lookup"><span data-stu-id="83565-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="83565-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83565-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83565-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83565-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83565-106">Данные приложения для создания отчетов</span><span class="sxs-lookup"><span data-stu-id="83565-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="83565-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="83565-107">Properties</span></span>
|<span data-ttu-id="83565-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="83565-108">Property</span></span>|<span data-ttu-id="83565-109">Тип</span><span class="sxs-lookup"><span data-stu-id="83565-109">Type</span></span>|<span data-ttu-id="83565-110">Описание</span><span class="sxs-lookup"><span data-stu-id="83565-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83565-111">appId</span><span class="sxs-lookup"><span data-stu-id="83565-111">appId</span></span>|<span data-ttu-id="83565-112">String</span><span class="sxs-lookup"><span data-stu-id="83565-112">String</span></span>|<span data-ttu-id="83565-113">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="83565-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="83565-114">Связи</span><span class="sxs-lookup"><span data-stu-id="83565-114">Relationships</span></span>
<span data-ttu-id="83565-115">Нет</span><span class="sxs-lookup"><span data-stu-id="83565-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83565-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="83565-116">JSON Representation</span></span>
<span data-ttu-id="83565-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83565-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceReportedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceReportedApp",
  "appId": "String"
}
```



