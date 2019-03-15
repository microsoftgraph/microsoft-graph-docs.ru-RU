---
title: Тип ресурса Виндовскиоскпрофиле
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63f00d8cdb8030a29baccc4a8f29e6c6e562c900
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571951"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="92d7f-103">Тип ресурса Виндовскиоскпрофиле</span><span class="sxs-lookup"><span data-stu-id="92d7f-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="92d7f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92d7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92d7f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92d7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92d7f-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="92d7f-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="92d7f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="92d7f-107">Properties</span></span>
|<span data-ttu-id="92d7f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="92d7f-108">Property</span></span>|<span data-ttu-id="92d7f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="92d7f-109">Type</span></span>|<span data-ttu-id="92d7f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="92d7f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92d7f-111">Профилеид</span><span class="sxs-lookup"><span data-stu-id="92d7f-111">profileId</span></span>|<span data-ttu-id="92d7f-112">String</span><span class="sxs-lookup"><span data-stu-id="92d7f-112">String</span></span>|<span data-ttu-id="92d7f-113">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="92d7f-113">Key of the entity.</span></span>|
|<span data-ttu-id="92d7f-114">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="92d7f-114">profileName</span></span>|<span data-ttu-id="92d7f-115">Строка</span><span class="sxs-lookup"><span data-stu-id="92d7f-115">String</span></span>|<span data-ttu-id="92d7f-116">Это понятное имя, используемое для идентификации группы приложений, макета этих приложений в меню "Пуск" и пользователей, которым назначена эта конфигурация киоска.</span><span class="sxs-lookup"><span data-stu-id="92d7f-116">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="92d7f-117">Аппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="92d7f-117">appConfiguration</span></span>|<span data-ttu-id="92d7f-118">[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="92d7f-118">[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>|<span data-ttu-id="92d7f-119">Конфигурация приложения, которая будет использоваться для этой конфигурации киоска.</span><span class="sxs-lookup"><span data-stu-id="92d7f-119">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="92d7f-120">Усераккаунтсконфигуратион</span><span class="sxs-lookup"><span data-stu-id="92d7f-120">userAccountsConfiguration</span></span>|<span data-ttu-id="92d7f-121">Коллекция [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="92d7f-121">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="92d7f-122">Учетные записи пользователей, которые будут заблокированы для этой конфигурации киоска.</span><span class="sxs-lookup"><span data-stu-id="92d7f-122">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="92d7f-123">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="92d7f-123">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92d7f-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="92d7f-124">Relationships</span></span>
<span data-ttu-id="92d7f-125">Нет</span><span class="sxs-lookup"><span data-stu-id="92d7f-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92d7f-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92d7f-126">JSON Representation</span></span>
<span data-ttu-id="92d7f-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92d7f-127">Here is a JSON representation of the resource.</span></span>
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
        "appType": "String",
        "autoLaunch": true,
        "appUserModelId": "String",
        "appId": "String",
        "containedAppId": "String"
      }
    ],
    "showTaskBar": true,
    "allowAccessToDownloadsFolder": true,
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




