---
title: Тип ресурса Виндовскиоскпрофиле
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b48f3957a5f43f7dc3a42cf52056403096bbb15
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995408"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="8e97a-103">Тип ресурса Виндовскиоскпрофиле</span><span class="sxs-lookup"><span data-stu-id="8e97a-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="8e97a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e97a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e97a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e97a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e97a-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8e97a-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8e97a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e97a-107">Properties</span></span>
|<span data-ttu-id="8e97a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e97a-108">Property</span></span>|<span data-ttu-id="8e97a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8e97a-109">Type</span></span>|<span data-ttu-id="8e97a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8e97a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e97a-111">Профилеид</span><span class="sxs-lookup"><span data-stu-id="8e97a-111">profileId</span></span>|<span data-ttu-id="8e97a-112">String</span><span class="sxs-lookup"><span data-stu-id="8e97a-112">String</span></span>|<span data-ttu-id="8e97a-113">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8e97a-113">Key of the entity.</span></span>|
|<span data-ttu-id="8e97a-114">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="8e97a-114">profileName</span></span>|<span data-ttu-id="8e97a-115">String</span><span class="sxs-lookup"><span data-stu-id="8e97a-115">String</span></span>|<span data-ttu-id="8e97a-116">Это понятное имя, используемое для идентификации группы приложений, макета этих приложений в меню "Пуск" и пользователей, которым назначена эта конфигурация киоска.</span><span class="sxs-lookup"><span data-stu-id="8e97a-116">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="8e97a-117">Аппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8e97a-117">appConfiguration</span></span>|<span data-ttu-id="8e97a-118">[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="8e97a-118">[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>|<span data-ttu-id="8e97a-119">Конфигурация приложения, которая будет использоваться для этой конфигурации киоска.</span><span class="sxs-lookup"><span data-stu-id="8e97a-119">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="8e97a-120">Усераккаунтсконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8e97a-120">userAccountsConfiguration</span></span>|<span data-ttu-id="8e97a-121">Коллекция [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="8e97a-121">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="8e97a-122">Учетные записи пользователей, которые будут заблокированы для этой конфигурации киоска.</span><span class="sxs-lookup"><span data-stu-id="8e97a-122">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="8e97a-123">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="8e97a-123">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e97a-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="8e97a-124">Relationships</span></span>
<span data-ttu-id="8e97a-125">Нет</span><span class="sxs-lookup"><span data-stu-id="8e97a-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e97a-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e97a-126">JSON Representation</span></span>
<span data-ttu-id="8e97a-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e97a-127">Here is a JSON representation of the resource.</span></span>
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





