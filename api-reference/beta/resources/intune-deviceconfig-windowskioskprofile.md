---
title: Тип ресурса Виндовскиоскпрофиле
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c69c8d32be23dccc935d1de74b0a450850091722
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268218"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="85818-103">Тип ресурса Виндовскиоскпрофиле</span><span class="sxs-lookup"><span data-stu-id="85818-103">windowsKioskProfile resource type</span></span>

<span data-ttu-id="85818-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85818-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85818-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85818-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85818-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85818-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85818-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="85818-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="85818-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="85818-108">Properties</span></span>
|<span data-ttu-id="85818-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="85818-109">Property</span></span>|<span data-ttu-id="85818-110">Тип</span><span class="sxs-lookup"><span data-stu-id="85818-110">Type</span></span>|<span data-ttu-id="85818-111">Описание</span><span class="sxs-lookup"><span data-stu-id="85818-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85818-112">профилеид</span><span class="sxs-lookup"><span data-stu-id="85818-112">profileId</span></span>|<span data-ttu-id="85818-113">String</span><span class="sxs-lookup"><span data-stu-id="85818-113">String</span></span>|<span data-ttu-id="85818-114">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="85818-114">Key of the entity.</span></span>|
|<span data-ttu-id="85818-115">имя_профиля</span><span class="sxs-lookup"><span data-stu-id="85818-115">profileName</span></span>|<span data-ttu-id="85818-116">String</span><span class="sxs-lookup"><span data-stu-id="85818-116">String</span></span>|<span data-ttu-id="85818-117">Это понятное имя, используемое для идентификации группы приложений, макета этих приложений в меню "Пуск" и пользователей, которым назначена эта конфигурация киоска.</span><span class="sxs-lookup"><span data-stu-id="85818-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="85818-118">аппконфигуратион</span><span class="sxs-lookup"><span data-stu-id="85818-118">appConfiguration</span></span>|<span data-ttu-id="85818-119">[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="85818-119">[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>|<span data-ttu-id="85818-120">Конфигурация приложения, которая будет использоваться для этой конфигурации киоска.</span><span class="sxs-lookup"><span data-stu-id="85818-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="85818-121">усераккаунтсконфигуратион</span><span class="sxs-lookup"><span data-stu-id="85818-121">userAccountsConfiguration</span></span>|<span data-ttu-id="85818-122">Коллекция [виндовскиоскусер](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="85818-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="85818-123">Учетные записи пользователей, которые будут заблокированы для этой конфигурации киоска.</span><span class="sxs-lookup"><span data-stu-id="85818-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="85818-124">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="85818-124">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85818-125">Связи</span><span class="sxs-lookup"><span data-stu-id="85818-125">Relationships</span></span>
<span data-ttu-id="85818-126">Нет</span><span class="sxs-lookup"><span data-stu-id="85818-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85818-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85818-127">JSON Representation</span></span>
<span data-ttu-id="85818-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85818-128">Here is a JSON representation of the resource.</span></span>
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




