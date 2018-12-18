---
title: Тип ресурса windowsKioskLocalUser
description: Класс, используемый для идентификации локальная учетная запись для базовой конфигурации
author: tfitzmac
ms.openlocfilehash: 5ac98147172fd08fc9914a7d9302e3b074ca3246
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310824"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="24169-103">Тип ресурса windowsKioskLocalUser</span><span class="sxs-lookup"><span data-stu-id="24169-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="24169-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="24169-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24169-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24169-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24169-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="24169-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24169-107">Класс, используемый для идентификации локальная учетная запись для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="24169-107">The class used to identify a local account for the kiosk configuration</span></span>

<span data-ttu-id="24169-108">Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="24169-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="24169-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="24169-109">Properties</span></span>
|<span data-ttu-id="24169-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="24169-110">Property</span></span>|<span data-ttu-id="24169-111">Тип</span><span class="sxs-lookup"><span data-stu-id="24169-111">Type</span></span>|<span data-ttu-id="24169-112">Описание</span><span class="sxs-lookup"><span data-stu-id="24169-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24169-113">userName</span><span class="sxs-lookup"><span data-stu-id="24169-113">userName</span></span>|<span data-ttu-id="24169-114">String</span><span class="sxs-lookup"><span data-stu-id="24169-114">String</span></span>|<span data-ttu-id="24169-115">Локальный пользователь, который будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="24169-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="24169-116">Связи</span><span class="sxs-lookup"><span data-stu-id="24169-116">Relationships</span></span>
<span data-ttu-id="24169-117">Нет</span><span class="sxs-lookup"><span data-stu-id="24169-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="24169-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24169-118">JSON Representation</span></span>
<span data-ttu-id="24169-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24169-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```





