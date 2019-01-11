---
title: Тип ресурса windowsKioskProfile
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c082b5fb9421af36bbc742051989492a5a3b19d0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807653"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="c5761-103">Тип ресурса windowsKioskProfile</span><span class="sxs-lookup"><span data-stu-id="c5761-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="c5761-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5761-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5761-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5761-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5761-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c5761-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5761-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c5761-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c5761-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5761-108">Properties</span></span>
|<span data-ttu-id="c5761-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5761-109">Property</span></span>|<span data-ttu-id="c5761-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c5761-110">Type</span></span>|<span data-ttu-id="c5761-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c5761-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5761-112">profileId</span><span class="sxs-lookup"><span data-stu-id="c5761-112">profileId</span></span>|<span data-ttu-id="c5761-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c5761-113">String</span></span>|<span data-ttu-id="c5761-114">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c5761-114">Key of the entity.</span></span>|
|<span data-ttu-id="c5761-115">Имя_профиля</span><span class="sxs-lookup"><span data-stu-id="c5761-115">profileName</span></span>|<span data-ttu-id="c5761-116">Строка</span><span class="sxs-lookup"><span data-stu-id="c5761-116">String</span></span>|<span data-ttu-id="c5761-117">Это понятное имя, используемое для идентификации групп приложений, макет эти приложения в меню Пуск и пользователи, которым назначена эта конфигурация киоска.</span><span class="sxs-lookup"><span data-stu-id="c5761-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="c5761-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5761-118">appConfiguration</span></span>|<span data-ttu-id="c5761-119">[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="c5761-119">[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>|<span data-ttu-id="c5761-120">Настройка приложения, который будет использоваться для этой базовой конфигурации.</span><span class="sxs-lookup"><span data-stu-id="c5761-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="c5761-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5761-121">userAccountsConfiguration</span></span>|<span data-ttu-id="c5761-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="c5761-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="c5761-123">Учетные записи пользователей, которые будут заблокированы для этой базовой конфигурации.</span><span class="sxs-lookup"><span data-stu-id="c5761-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="c5761-124">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c5761-124">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5761-125">Связи</span><span class="sxs-lookup"><span data-stu-id="c5761-125">Relationships</span></span>
<span data-ttu-id="c5761-126">Нет</span><span class="sxs-lookup"><span data-stu-id="c5761-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c5761-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5761-127">JSON Representation</span></span>
<span data-ttu-id="c5761-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5761-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskProfile",
  "profileId": "String",
  "profileName": "String",
  "appConfiguration": {
    "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
    "apps": [
      {
        "@odata.type": "microsoft.graph.windowsKioskUWPApp",
        "startLayoutTileSize": "String",
        "name": "String",
        "appUserModelId": "String",
        "appId": "String",
        "containedAppId": "String"
      }
    ],
    "showTaskBar": true,
    "disallowDesktopApps": true,
    "startMenuLayoutXml": "binary"
  },
  "userAccountsConfiguration": [
    {
      "@odata.type": "microsoft.graph.windowsKioskVisitor"
    }
  ]
}
```





