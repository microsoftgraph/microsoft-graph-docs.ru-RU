---
title: Тип ресурса Логжедонусер
description: Вошедший в систему пользователь
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e013b89eefbcdb1bf180ff90341388db9c05dcf4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995156"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="95a0f-103">Тип ресурса Логжедонусер</span><span class="sxs-lookup"><span data-stu-id="95a0f-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="95a0f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95a0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95a0f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95a0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95a0f-106">Вошедший в систему пользователь</span><span class="sxs-lookup"><span data-stu-id="95a0f-106">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="95a0f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="95a0f-107">Properties</span></span>
|<span data-ttu-id="95a0f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="95a0f-108">Property</span></span>|<span data-ttu-id="95a0f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="95a0f-109">Type</span></span>|<span data-ttu-id="95a0f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="95a0f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95a0f-111">userId</span><span class="sxs-lookup"><span data-stu-id="95a0f-111">userId</span></span>|<span data-ttu-id="95a0f-112">String</span><span class="sxs-lookup"><span data-stu-id="95a0f-112">String</span></span>|<span data-ttu-id="95a0f-113">Идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="95a0f-113">User id</span></span>|
|<span data-ttu-id="95a0f-114">Ластлогондатетиме</span><span class="sxs-lookup"><span data-stu-id="95a0f-114">lastLogOnDateTime</span></span>|<span data-ttu-id="95a0f-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95a0f-115">DateTimeOffset</span></span>|<span data-ttu-id="95a0f-116">Дата и время, когда пользователь входит в систему</span><span class="sxs-lookup"><span data-stu-id="95a0f-116">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="95a0f-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="95a0f-117">Relationships</span></span>
<span data-ttu-id="95a0f-118">Нет</span><span class="sxs-lookup"><span data-stu-id="95a0f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95a0f-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95a0f-119">JSON Representation</span></span>
<span data-ttu-id="95a0f-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95a0f-120">Here is a JSON representation of the resource.</span></span>
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





