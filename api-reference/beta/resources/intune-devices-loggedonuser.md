---
title: Тип ресурса loggedOnUser
description: Вход в систему пользователя
ms.openlocfilehash: 37df6b5343df515a76bc6b755889156cb86c4bf0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082607"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="ad28b-103">Тип ресурса loggedOnUser</span><span class="sxs-lookup"><span data-stu-id="ad28b-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="ad28b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad28b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad28b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad28b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad28b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ad28b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad28b-107">Вход в систему пользователя</span><span class="sxs-lookup"><span data-stu-id="ad28b-107">Logged On User</span></span>
## <a name="properties"></a><span data-ttu-id="ad28b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad28b-108">Properties</span></span>
|<span data-ttu-id="ad28b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad28b-109">Property</span></span>|<span data-ttu-id="ad28b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ad28b-110">Type</span></span>|<span data-ttu-id="ad28b-111">Description</span><span class="sxs-lookup"><span data-stu-id="ad28b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad28b-112">userId</span><span class="sxs-lookup"><span data-stu-id="ad28b-112">userId</span></span>|<span data-ttu-id="ad28b-113">String</span><span class="sxs-lookup"><span data-stu-id="ad28b-113">String</span></span>|<span data-ttu-id="ad28b-114">Идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="ad28b-114">User id</span></span>|
|<span data-ttu-id="ad28b-115">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="ad28b-115">lastLogOnDateTime</span></span>|<span data-ttu-id="ad28b-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad28b-116">DateTimeOffset</span></span>|<span data-ttu-id="ad28b-117">Дата и время, при входе пользователя в систему</span><span class="sxs-lookup"><span data-stu-id="ad28b-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad28b-118">Связи</span><span class="sxs-lookup"><span data-stu-id="ad28b-118">Relationships</span></span>
<span data-ttu-id="ad28b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ad28b-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ad28b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad28b-120">JSON Representation</span></span>
<span data-ttu-id="ad28b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad28b-121">Here is a JSON representation of the resource.</span></span>
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





