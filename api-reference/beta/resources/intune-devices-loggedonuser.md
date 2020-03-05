---
title: Тип ресурса Логжедонусер
description: Вошедший в систему пользователь
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 37c0ffd9b5359f4f876ba3278e4f95ea7272e670
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524993"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="421f6-103">Тип ресурса Логжедонусер</span><span class="sxs-lookup"><span data-stu-id="421f6-103">loggedOnUser resource type</span></span>

<span data-ttu-id="421f6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="421f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="421f6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="421f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="421f6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="421f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="421f6-107">Вошедший в систему пользователь</span><span class="sxs-lookup"><span data-stu-id="421f6-107">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="421f6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="421f6-108">Properties</span></span>
|<span data-ttu-id="421f6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="421f6-109">Property</span></span>|<span data-ttu-id="421f6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="421f6-110">Type</span></span>|<span data-ttu-id="421f6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="421f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="421f6-112">userId</span><span class="sxs-lookup"><span data-stu-id="421f6-112">userId</span></span>|<span data-ttu-id="421f6-113">String</span><span class="sxs-lookup"><span data-stu-id="421f6-113">String</span></span>|<span data-ttu-id="421f6-114">Идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="421f6-114">User id</span></span>|
|<span data-ttu-id="421f6-115">ластлогондатетиме</span><span class="sxs-lookup"><span data-stu-id="421f6-115">lastLogOnDateTime</span></span>|<span data-ttu-id="421f6-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="421f6-116">DateTimeOffset</span></span>|<span data-ttu-id="421f6-117">Дата и время, когда пользователь входит в систему</span><span class="sxs-lookup"><span data-stu-id="421f6-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="421f6-118">Связи</span><span class="sxs-lookup"><span data-stu-id="421f6-118">Relationships</span></span>
<span data-ttu-id="421f6-119">Нет</span><span class="sxs-lookup"><span data-stu-id="421f6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="421f6-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="421f6-120">JSON Representation</span></span>
<span data-ttu-id="421f6-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="421f6-121">Here is a JSON representation of the resource.</span></span>
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



