---
title: Тип ресурса Логжедонусер
description: ВоШедший в систему пользователь
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5dfaa8bbaa879fc48c5f6ea31d1b7b14e998820
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148932"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="ee9ea-103">Тип ресурса Логжедонусер</span><span class="sxs-lookup"><span data-stu-id="ee9ea-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="ee9ea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee9ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee9ea-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee9ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee9ea-106">ВоШедший в систему пользователь</span><span class="sxs-lookup"><span data-stu-id="ee9ea-106">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="ee9ea-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee9ea-107">Properties</span></span>
|<span data-ttu-id="ee9ea-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee9ea-108">Property</span></span>|<span data-ttu-id="ee9ea-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ee9ea-109">Type</span></span>|<span data-ttu-id="ee9ea-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ee9ea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee9ea-111">userId</span><span class="sxs-lookup"><span data-stu-id="ee9ea-111">userId</span></span>|<span data-ttu-id="ee9ea-112">String</span><span class="sxs-lookup"><span data-stu-id="ee9ea-112">String</span></span>|<span data-ttu-id="ee9ea-113">Идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="ee9ea-113">User id</span></span>|
|<span data-ttu-id="ee9ea-114">Ластлогондатетиме</span><span class="sxs-lookup"><span data-stu-id="ee9ea-114">lastLogOnDateTime</span></span>|<span data-ttu-id="ee9ea-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee9ea-115">DateTimeOffset</span></span>|<span data-ttu-id="ee9ea-116">Дата и время, когда пользователь входит в систему</span><span class="sxs-lookup"><span data-stu-id="ee9ea-116">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee9ea-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="ee9ea-117">Relationships</span></span>
<span data-ttu-id="ee9ea-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ee9ea-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee9ea-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee9ea-119">JSON Representation</span></span>
<span data-ttu-id="ee9ea-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee9ea-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```




