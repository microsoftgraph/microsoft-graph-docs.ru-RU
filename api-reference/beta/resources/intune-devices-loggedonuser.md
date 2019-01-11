---
title: Тип ресурса loggedOnUser
description: Вход в систему пользователя
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e832c6452b73a6fad39723675acb129d79c2b888
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859754"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="dca20-103">Тип ресурса loggedOnUser</span><span class="sxs-lookup"><span data-stu-id="dca20-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="dca20-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dca20-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dca20-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dca20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dca20-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dca20-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dca20-107">Вход в систему пользователя</span><span class="sxs-lookup"><span data-stu-id="dca20-107">Logged On User</span></span>
## <a name="properties"></a><span data-ttu-id="dca20-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dca20-108">Properties</span></span>
|<span data-ttu-id="dca20-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dca20-109">Property</span></span>|<span data-ttu-id="dca20-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dca20-110">Type</span></span>|<span data-ttu-id="dca20-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dca20-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dca20-112">userId</span><span class="sxs-lookup"><span data-stu-id="dca20-112">userId</span></span>|<span data-ttu-id="dca20-113">String</span><span class="sxs-lookup"><span data-stu-id="dca20-113">String</span></span>|<span data-ttu-id="dca20-114">Идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="dca20-114">User id</span></span>|
|<span data-ttu-id="dca20-115">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="dca20-115">lastLogOnDateTime</span></span>|<span data-ttu-id="dca20-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dca20-116">DateTimeOffset</span></span>|<span data-ttu-id="dca20-117">Дата и время, при входе пользователя в систему</span><span class="sxs-lookup"><span data-stu-id="dca20-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="dca20-118">Связи</span><span class="sxs-lookup"><span data-stu-id="dca20-118">Relationships</span></span>
<span data-ttu-id="dca20-119">Нет</span><span class="sxs-lookup"><span data-stu-id="dca20-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dca20-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dca20-120">JSON Representation</span></span>
<span data-ttu-id="dca20-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dca20-121">Here is a JSON representation of the resource.</span></span>
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





