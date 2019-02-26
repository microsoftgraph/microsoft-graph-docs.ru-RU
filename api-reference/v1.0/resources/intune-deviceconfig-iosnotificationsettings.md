---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ce016579729353f69f2e7671ff67b5da0004536
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260384"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="8f3b5-103">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="8f3b5-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="8f3b5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f3b5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f3b5-105">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="8f3b5-105">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="8f3b5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f3b5-106">Properties</span></span>
|<span data-ttu-id="8f3b5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f3b5-107">Property</span></span>|<span data-ttu-id="8f3b5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8f3b5-108">Type</span></span>|<span data-ttu-id="8f3b5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8f3b5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f3b5-110">bundleID</span><span class="sxs-lookup"><span data-stu-id="8f3b5-110">bundleID</span></span>|<span data-ttu-id="8f3b5-111">String</span><span class="sxs-lookup"><span data-stu-id="8f3b5-111">String</span></span>|<span data-ttu-id="8f3b5-112">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="8f3b5-112">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="8f3b5-113">appName</span><span class="sxs-lookup"><span data-stu-id="8f3b5-113">appName</span></span>|<span data-ttu-id="8f3b5-114">String</span><span class="sxs-lookup"><span data-stu-id="8f3b5-114">String</span></span>|<span data-ttu-id="8f3b5-115">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="8f3b5-115">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="8f3b5-116">publisher</span><span class="sxs-lookup"><span data-stu-id="8f3b5-116">publisher</span></span>|<span data-ttu-id="8f3b5-117">String</span><span class="sxs-lookup"><span data-stu-id="8f3b5-117">String</span></span>|<span data-ttu-id="8f3b5-118">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="8f3b5-118">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="8f3b5-119">enabled</span><span class="sxs-lookup"><span data-stu-id="8f3b5-119">enabled</span></span>|<span data-ttu-id="8f3b5-120">Логический</span><span class="sxs-lookup"><span data-stu-id="8f3b5-120">Boolean</span></span>|<span data-ttu-id="8f3b5-121">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="8f3b5-121">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="8f3b5-122">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="8f3b5-122">showInNotificationCenter</span></span>|<span data-ttu-id="8f3b5-123">Логический</span><span class="sxs-lookup"><span data-stu-id="8f3b5-123">Boolean</span></span>|<span data-ttu-id="8f3b5-124">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="8f3b5-124">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="8f3b5-125">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="8f3b5-125">showOnLockScreen</span></span>|<span data-ttu-id="8f3b5-126">Логический</span><span class="sxs-lookup"><span data-stu-id="8f3b5-126">Boolean</span></span>|<span data-ttu-id="8f3b5-127">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="8f3b5-127">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="8f3b5-128">alertType</span><span class="sxs-lookup"><span data-stu-id="8f3b5-128">alertType</span></span>|[<span data-ttu-id="8f3b5-129">Иоснотификатионалерттипе</span><span class="sxs-lookup"><span data-stu-id="8f3b5-129">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="8f3b5-130">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="8f3b5-130">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="8f3b5-131">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="8f3b5-131">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="8f3b5-132">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="8f3b5-132">badgesEnabled</span></span>|<span data-ttu-id="8f3b5-133">Логический</span><span class="sxs-lookup"><span data-stu-id="8f3b5-133">Boolean</span></span>|<span data-ttu-id="8f3b5-134">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="8f3b5-134">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="8f3b5-135">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="8f3b5-135">soundsEnabled</span></span>|<span data-ttu-id="8f3b5-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f3b5-136">Boolean</span></span>|<span data-ttu-id="8f3b5-137">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="8f3b5-137">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f3b5-138">Связи</span><span class="sxs-lookup"><span data-stu-id="8f3b5-138">Relationships</span></span>
<span data-ttu-id="8f3b5-139">Нет</span><span class="sxs-lookup"><span data-stu-id="8f3b5-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f3b5-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f3b5-140">JSON Representation</span></span>
<span data-ttu-id="8f3b5-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f3b5-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```



