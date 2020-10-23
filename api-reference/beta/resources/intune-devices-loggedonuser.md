---
title: Тип ресурса Логжедонусер
description: Вошедший в систему пользователь
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c37ca746a2adc1ea1cba92839bce3903f947e4d6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729308"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="b18c7-103">Тип ресурса Логжедонусер</span><span class="sxs-lookup"><span data-stu-id="b18c7-103">loggedOnUser resource type</span></span>

<span data-ttu-id="b18c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b18c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b18c7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b18c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b18c7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b18c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b18c7-107">Вошедший в систему пользователь</span><span class="sxs-lookup"><span data-stu-id="b18c7-107">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="b18c7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b18c7-108">Properties</span></span>
|<span data-ttu-id="b18c7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b18c7-109">Property</span></span>|<span data-ttu-id="b18c7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b18c7-110">Type</span></span>|<span data-ttu-id="b18c7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b18c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b18c7-112">userId</span><span class="sxs-lookup"><span data-stu-id="b18c7-112">userId</span></span>|<span data-ttu-id="b18c7-113">String</span><span class="sxs-lookup"><span data-stu-id="b18c7-113">String</span></span>|<span data-ttu-id="b18c7-114">Идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="b18c7-114">User id</span></span>|
|<span data-ttu-id="b18c7-115">ластлогондатетиме</span><span class="sxs-lookup"><span data-stu-id="b18c7-115">lastLogOnDateTime</span></span>|<span data-ttu-id="b18c7-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b18c7-116">DateTimeOffset</span></span>|<span data-ttu-id="b18c7-117">Дата и время, когда пользователь входит в систему</span><span class="sxs-lookup"><span data-stu-id="b18c7-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="b18c7-118">Связи</span><span class="sxs-lookup"><span data-stu-id="b18c7-118">Relationships</span></span>
<span data-ttu-id="b18c7-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b18c7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b18c7-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b18c7-120">JSON Representation</span></span>
<span data-ttu-id="b18c7-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b18c7-121">Here is a JSON representation of the resource.</span></span>
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





