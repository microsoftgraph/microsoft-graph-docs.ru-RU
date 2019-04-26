---
title: Тип ресурса Манажеддевицерепортедапп
description: Данные приложения для создания отчетов
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b243cbc5c3c06de6af3e2e0f1263b589edf86f48
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572796"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="4d96d-103">Тип ресурса Манажеддевицерепортедапп</span><span class="sxs-lookup"><span data-stu-id="4d96d-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="4d96d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d96d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d96d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d96d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d96d-106">Данные приложения для создания отчетов</span><span class="sxs-lookup"><span data-stu-id="4d96d-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="4d96d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d96d-107">Properties</span></span>
|<span data-ttu-id="4d96d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d96d-108">Property</span></span>|<span data-ttu-id="4d96d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4d96d-109">Type</span></span>|<span data-ttu-id="4d96d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4d96d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d96d-111">appId</span><span class="sxs-lookup"><span data-stu-id="4d96d-111">appId</span></span>|<span data-ttu-id="4d96d-112">String</span><span class="sxs-lookup"><span data-stu-id="4d96d-112">String</span></span>|<span data-ttu-id="4d96d-113">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="4d96d-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d96d-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="4d96d-114">Relationships</span></span>
<span data-ttu-id="4d96d-115">Нет</span><span class="sxs-lookup"><span data-stu-id="4d96d-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d96d-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d96d-116">JSON Representation</span></span>
<span data-ttu-id="4d96d-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d96d-117">Here is a JSON representation of the resource.</span></span>
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





