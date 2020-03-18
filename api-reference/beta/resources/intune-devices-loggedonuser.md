---
title: Тип ресурса Логжедонусер
description: Вошедший в систему пользователь
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cab517ec064cea375efd8effaca9d31159e64bcd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783993"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="6cc76-103">Тип ресурса Логжедонусер</span><span class="sxs-lookup"><span data-stu-id="6cc76-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="6cc76-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cc76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cc76-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6cc76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cc76-106">Вошедший в систему пользователь</span><span class="sxs-lookup"><span data-stu-id="6cc76-106">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="6cc76-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6cc76-107">Properties</span></span>
|<span data-ttu-id="6cc76-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cc76-108">Property</span></span>|<span data-ttu-id="6cc76-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6cc76-109">Type</span></span>|<span data-ttu-id="6cc76-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6cc76-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cc76-111">userId</span><span class="sxs-lookup"><span data-stu-id="6cc76-111">userId</span></span>|<span data-ttu-id="6cc76-112">String</span><span class="sxs-lookup"><span data-stu-id="6cc76-112">String</span></span>|<span data-ttu-id="6cc76-113">Идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="6cc76-113">User id</span></span>|
|<span data-ttu-id="6cc76-114">ластлогондатетиме</span><span class="sxs-lookup"><span data-stu-id="6cc76-114">lastLogOnDateTime</span></span>|<span data-ttu-id="6cc76-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cc76-115">DateTimeOffset</span></span>|<span data-ttu-id="6cc76-116">Дата и время, когда пользователь входит в систему</span><span class="sxs-lookup"><span data-stu-id="6cc76-116">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="6cc76-117">Связи</span><span class="sxs-lookup"><span data-stu-id="6cc76-117">Relationships</span></span>
<span data-ttu-id="6cc76-118">Нет</span><span class="sxs-lookup"><span data-stu-id="6cc76-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6cc76-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6cc76-119">JSON Representation</span></span>
<span data-ttu-id="6cc76-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6cc76-120">Here is a JSON representation of the resource.</span></span>
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



