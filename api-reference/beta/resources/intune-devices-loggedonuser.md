---
title: Тип ресурса Логжедонусер
description: Вошедший в систему пользователь
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 994946d9dcd7abf3f2f57df652321a61dd71dd47
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208949"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="ee7b1-103">Тип ресурса Логжедонусер</span><span class="sxs-lookup"><span data-stu-id="ee7b1-103">loggedOnUser resource type</span></span>

<span data-ttu-id="ee7b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee7b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee7b1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee7b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee7b1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee7b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee7b1-107">Вошедший в систему пользователь</span><span class="sxs-lookup"><span data-stu-id="ee7b1-107">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="ee7b1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee7b1-108">Properties</span></span>
|<span data-ttu-id="ee7b1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee7b1-109">Property</span></span>|<span data-ttu-id="ee7b1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ee7b1-110">Type</span></span>|<span data-ttu-id="ee7b1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ee7b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee7b1-112">userId</span><span class="sxs-lookup"><span data-stu-id="ee7b1-112">userId</span></span>|<span data-ttu-id="ee7b1-113">String</span><span class="sxs-lookup"><span data-stu-id="ee7b1-113">String</span></span>|<span data-ttu-id="ee7b1-114">Идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="ee7b1-114">User id</span></span>|
|<span data-ttu-id="ee7b1-115">ластлогондатетиме</span><span class="sxs-lookup"><span data-stu-id="ee7b1-115">lastLogOnDateTime</span></span>|<span data-ttu-id="ee7b1-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee7b1-116">DateTimeOffset</span></span>|<span data-ttu-id="ee7b1-117">Дата и время, когда пользователь входит в систему</span><span class="sxs-lookup"><span data-stu-id="ee7b1-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee7b1-118">Связи</span><span class="sxs-lookup"><span data-stu-id="ee7b1-118">Relationships</span></span>
<span data-ttu-id="ee7b1-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ee7b1-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee7b1-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee7b1-120">JSON Representation</span></span>
<span data-ttu-id="ee7b1-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee7b1-121">Here is a JSON representation of the resource.</span></span>
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




