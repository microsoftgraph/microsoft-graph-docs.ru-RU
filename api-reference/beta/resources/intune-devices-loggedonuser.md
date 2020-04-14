---
title: Тип ресурса Логжедонусер
description: Вошедший в систему пользователь
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e8f1547669a2bb14c5ae84920c1eb6bef2dfbeb1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470523"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="eaf04-103">Тип ресурса Логжедонусер</span><span class="sxs-lookup"><span data-stu-id="eaf04-103">loggedOnUser resource type</span></span>

<span data-ttu-id="eaf04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaf04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eaf04-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaf04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eaf04-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eaf04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eaf04-107">Вошедший в систему пользователь</span><span class="sxs-lookup"><span data-stu-id="eaf04-107">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="eaf04-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eaf04-108">Properties</span></span>
|<span data-ttu-id="eaf04-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eaf04-109">Property</span></span>|<span data-ttu-id="eaf04-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eaf04-110">Type</span></span>|<span data-ttu-id="eaf04-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eaf04-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaf04-112">userId</span><span class="sxs-lookup"><span data-stu-id="eaf04-112">userId</span></span>|<span data-ttu-id="eaf04-113">String</span><span class="sxs-lookup"><span data-stu-id="eaf04-113">String</span></span>|<span data-ttu-id="eaf04-114">Идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="eaf04-114">User id</span></span>|
|<span data-ttu-id="eaf04-115">ластлогондатетиме</span><span class="sxs-lookup"><span data-stu-id="eaf04-115">lastLogOnDateTime</span></span>|<span data-ttu-id="eaf04-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaf04-116">DateTimeOffset</span></span>|<span data-ttu-id="eaf04-117">Дата и время, когда пользователь входит в систему</span><span class="sxs-lookup"><span data-stu-id="eaf04-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="eaf04-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="eaf04-118">Relationships</span></span>
<span data-ttu-id="eaf04-119">Нет</span><span class="sxs-lookup"><span data-stu-id="eaf04-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eaf04-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eaf04-120">JSON Representation</span></span>
<span data-ttu-id="eaf04-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eaf04-121">Here is a JSON representation of the resource.</span></span>
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



