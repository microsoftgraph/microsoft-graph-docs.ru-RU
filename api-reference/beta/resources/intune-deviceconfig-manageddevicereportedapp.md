---
title: Тип ресурса managedDeviceReportedApp
description: Данные приложения для создания отчетов
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 104503083f5f599bc366de2ca8082fd9fdf3102e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422609"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="0e64c-103">Тип ресурса managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="0e64c-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="0e64c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0e64c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0e64c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e64c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e64c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e64c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e64c-107">Данные приложения для создания отчетов</span><span class="sxs-lookup"><span data-stu-id="0e64c-107">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="0e64c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e64c-108">Properties</span></span>
|<span data-ttu-id="0e64c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e64c-109">Property</span></span>|<span data-ttu-id="0e64c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0e64c-110">Type</span></span>|<span data-ttu-id="0e64c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0e64c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e64c-112">appId</span><span class="sxs-lookup"><span data-stu-id="0e64c-112">appId</span></span>|<span data-ttu-id="0e64c-113">String</span><span class="sxs-lookup"><span data-stu-id="0e64c-113">String</span></span>|<span data-ttu-id="0e64c-114">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="0e64c-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e64c-115">Связи</span><span class="sxs-lookup"><span data-stu-id="0e64c-115">Relationships</span></span>
<span data-ttu-id="0e64c-116">Нет</span><span class="sxs-lookup"><span data-stu-id="0e64c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e64c-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e64c-117">JSON Representation</span></span>
<span data-ttu-id="0e64c-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e64c-118">Here is a JSON representation of the resource.</span></span>
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




