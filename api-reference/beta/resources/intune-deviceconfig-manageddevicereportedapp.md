---
title: Тип ресурса managedDeviceReportedApp
description: Данные приложения для создания отчетов
author: tfitzmac
ms.openlocfilehash: 7fd01c5fd7553769653abd6e16ecc9ec40a79b8a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359495"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="00e63-103">Тип ресурса managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="00e63-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="00e63-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="00e63-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00e63-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00e63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00e63-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="00e63-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00e63-107">Данные приложения для создания отчетов</span><span class="sxs-lookup"><span data-stu-id="00e63-107">Application data for reporting</span></span>
## <a name="properties"></a><span data-ttu-id="00e63-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="00e63-108">Properties</span></span>
|<span data-ttu-id="00e63-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="00e63-109">Property</span></span>|<span data-ttu-id="00e63-110">Тип</span><span class="sxs-lookup"><span data-stu-id="00e63-110">Type</span></span>|<span data-ttu-id="00e63-111">Описание</span><span class="sxs-lookup"><span data-stu-id="00e63-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00e63-112">appId</span><span class="sxs-lookup"><span data-stu-id="00e63-112">appId</span></span>|<span data-ttu-id="00e63-113">String</span><span class="sxs-lookup"><span data-stu-id="00e63-113">String</span></span>|<span data-ttu-id="00e63-114">Идентификатор приложения или его пакета</span><span class="sxs-lookup"><span data-stu-id="00e63-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="00e63-115">Связи</span><span class="sxs-lookup"><span data-stu-id="00e63-115">Relationships</span></span>
<span data-ttu-id="00e63-116">Нет</span><span class="sxs-lookup"><span data-stu-id="00e63-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="00e63-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00e63-117">JSON Representation</span></span>
<span data-ttu-id="00e63-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00e63-118">Here is a JSON representation of the resource.</span></span>
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





