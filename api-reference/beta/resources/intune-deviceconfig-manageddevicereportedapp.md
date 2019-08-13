---
title: Тип ресурса Манажеддевицерепортедапп
description: Данные приложения для создания отчетов
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6561a6cee5a02f46c3347a1919c93c3807250fa8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368830"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="6ff01-103">Тип ресурса Манажеддевицерепортедапп</span><span class="sxs-lookup"><span data-stu-id="6ff01-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="6ff01-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ff01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ff01-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ff01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ff01-106">Данные приложения для создания отчетов</span><span class="sxs-lookup"><span data-stu-id="6ff01-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="6ff01-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ff01-107">Properties</span></span>
|<span data-ttu-id="6ff01-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ff01-108">Property</span></span>|<span data-ttu-id="6ff01-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6ff01-109">Type</span></span>|<span data-ttu-id="6ff01-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6ff01-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ff01-111">appId</span><span class="sxs-lookup"><span data-stu-id="6ff01-111">appId</span></span>|<span data-ttu-id="6ff01-112">String</span><span class="sxs-lookup"><span data-stu-id="6ff01-112">String</span></span>|<span data-ttu-id="6ff01-113">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="6ff01-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ff01-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="6ff01-114">Relationships</span></span>
<span data-ttu-id="6ff01-115">Нет</span><span class="sxs-lookup"><span data-stu-id="6ff01-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ff01-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ff01-116">JSON Representation</span></span>
<span data-ttu-id="6ff01-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ff01-117">Here is a JSON representation of the resource.</span></span>
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



