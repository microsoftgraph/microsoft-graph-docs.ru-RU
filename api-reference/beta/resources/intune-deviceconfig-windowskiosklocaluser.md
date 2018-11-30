---
title: Тип ресурса windowsKioskLocalUser
description: Класс, используемый для идентификации локальная учетная запись для базовой конфигурации
ms.openlocfilehash: 1b5b8837f4f93005dabf839a7fc20e3b05b1fbf9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076394"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="56777-103">Тип ресурса windowsKioskLocalUser</span><span class="sxs-lookup"><span data-stu-id="56777-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="56777-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="56777-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56777-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56777-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56777-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="56777-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56777-107">Класс, используемый для идентификации локальная учетная запись для базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="56777-107">The class used to identify a local account for the kiosk configuration</span></span>

<span data-ttu-id="56777-108">Наследуется от [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="56777-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="56777-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="56777-109">Properties</span></span>
|<span data-ttu-id="56777-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="56777-110">Property</span></span>|<span data-ttu-id="56777-111">Тип</span><span class="sxs-lookup"><span data-stu-id="56777-111">Type</span></span>|<span data-ttu-id="56777-112">Description</span><span class="sxs-lookup"><span data-stu-id="56777-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56777-113">userName</span><span class="sxs-lookup"><span data-stu-id="56777-113">userName</span></span>|<span data-ttu-id="56777-114">String</span><span class="sxs-lookup"><span data-stu-id="56777-114">String</span></span>|<span data-ttu-id="56777-115">Локальный пользователь, который будет заблокирована этой базовой конфигурации</span><span class="sxs-lookup"><span data-stu-id="56777-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="56777-116">Связи</span><span class="sxs-lookup"><span data-stu-id="56777-116">Relationships</span></span>
<span data-ttu-id="56777-117">Нет</span><span class="sxs-lookup"><span data-stu-id="56777-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="56777-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56777-118">JSON Representation</span></span>
<span data-ttu-id="56777-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56777-119">Here is a JSON representation of the resource.</span></span>
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





