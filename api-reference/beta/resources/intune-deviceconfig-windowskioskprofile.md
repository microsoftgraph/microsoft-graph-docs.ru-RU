---
title: Тип ресурса windowsKioskProfile
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55d8c23d3bfae2baf9d632c33390b8aafb5e7ef8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420250"
---
# <a name="windowskioskprofile-resource-type"></a><span data-ttu-id="a383e-103">Тип ресурса windowsKioskProfile</span><span class="sxs-lookup"><span data-stu-id="a383e-103">windowsKioskProfile resource type</span></span>

> <span data-ttu-id="a383e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a383e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a383e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a383e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a383e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a383e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a383e-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a383e-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a383e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a383e-108">Properties</span></span>
|<span data-ttu-id="a383e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a383e-109">Property</span></span>|<span data-ttu-id="a383e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a383e-110">Type</span></span>|<span data-ttu-id="a383e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a383e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a383e-112">profileId</span><span class="sxs-lookup"><span data-stu-id="a383e-112">profileId</span></span>|<span data-ttu-id="a383e-113">String</span><span class="sxs-lookup"><span data-stu-id="a383e-113">String</span></span>|<span data-ttu-id="a383e-114">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a383e-114">Key of the entity.</span></span>|
|<span data-ttu-id="a383e-115">Имя_профиля</span><span class="sxs-lookup"><span data-stu-id="a383e-115">profileName</span></span>|<span data-ttu-id="a383e-116">String</span><span class="sxs-lookup"><span data-stu-id="a383e-116">String</span></span>|<span data-ttu-id="a383e-117">Это понятное имя, используемое для идентификации групп приложений, макет эти приложения в меню Пуск и пользователи, которым назначена эта конфигурация киоска.</span><span class="sxs-lookup"><span data-stu-id="a383e-117">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="a383e-118">appConfiguration</span><span class="sxs-lookup"><span data-stu-id="a383e-118">appConfiguration</span></span>|<span data-ttu-id="a383e-119">[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="a383e-119">[windowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)</span></span>|<span data-ttu-id="a383e-120">Настройка приложения, который будет использоваться для этой базовой конфигурации.</span><span class="sxs-lookup"><span data-stu-id="a383e-120">The App configuration that will be used for this kiosk configuration.</span></span>|
|<span data-ttu-id="a383e-121">userAccountsConfiguration</span><span class="sxs-lookup"><span data-stu-id="a383e-121">userAccountsConfiguration</span></span>|<span data-ttu-id="a383e-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a383e-122">[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md) collection</span></span>|<span data-ttu-id="a383e-123">Учетные записи пользователей, которые будут заблокированы для этой базовой конфигурации.</span><span class="sxs-lookup"><span data-stu-id="a383e-123">The user accounts that will be locked to this kiosk configuration.</span></span> <span data-ttu-id="a383e-124">Эта коллекция может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="a383e-124">This collection can contain a maximum of 100 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a383e-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="a383e-125">Relationships</span></span>
<span data-ttu-id="a383e-126">Нет</span><span class="sxs-lookup"><span data-stu-id="a383e-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a383e-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a383e-127">JSON Representation</span></span>
<span data-ttu-id="a383e-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a383e-128">Here is a JSON representation of the resource.</span></span>
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




