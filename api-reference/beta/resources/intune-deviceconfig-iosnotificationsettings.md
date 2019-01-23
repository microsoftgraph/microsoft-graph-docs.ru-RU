---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7db0b6ba438522db0795f6897daba8b5c43258c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420502"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="dfb10-103">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="dfb10-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="dfb10-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dfb10-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dfb10-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfb10-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dfb10-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dfb10-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfb10-107">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="dfb10-107">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="dfb10-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfb10-108">Properties</span></span>
|<span data-ttu-id="dfb10-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfb10-109">Property</span></span>|<span data-ttu-id="dfb10-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dfb10-110">Type</span></span>|<span data-ttu-id="dfb10-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dfb10-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfb10-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="dfb10-112">bundleID</span></span>|<span data-ttu-id="dfb10-113">String</span><span class="sxs-lookup"><span data-stu-id="dfb10-113">String</span></span>|<span data-ttu-id="dfb10-114">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="dfb10-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="dfb10-115">appName</span><span class="sxs-lookup"><span data-stu-id="dfb10-115">appName</span></span>|<span data-ttu-id="dfb10-116">String</span><span class="sxs-lookup"><span data-stu-id="dfb10-116">String</span></span>|<span data-ttu-id="dfb10-117">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="dfb10-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="dfb10-118">publisher</span><span class="sxs-lookup"><span data-stu-id="dfb10-118">publisher</span></span>|<span data-ttu-id="dfb10-119">String</span><span class="sxs-lookup"><span data-stu-id="dfb10-119">String</span></span>|<span data-ttu-id="dfb10-120">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="dfb10-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="dfb10-121">enabled</span><span class="sxs-lookup"><span data-stu-id="dfb10-121">enabled</span></span>|<span data-ttu-id="dfb10-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb10-122">Boolean</span></span>|<span data-ttu-id="dfb10-123">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="dfb10-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="dfb10-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="dfb10-124">showInNotificationCenter</span></span>|<span data-ttu-id="dfb10-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb10-125">Boolean</span></span>|<span data-ttu-id="dfb10-126">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="dfb10-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="dfb10-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="dfb10-127">showOnLockScreen</span></span>|<span data-ttu-id="dfb10-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb10-128">Boolean</span></span>|<span data-ttu-id="dfb10-129">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="dfb10-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="dfb10-130">alertType</span><span class="sxs-lookup"><span data-stu-id="dfb10-130">alertType</span></span>|[<span data-ttu-id="dfb10-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="dfb10-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="dfb10-132">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="dfb10-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="dfb10-133">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="dfb10-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="dfb10-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="dfb10-134">badgesEnabled</span></span>|<span data-ttu-id="dfb10-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb10-135">Boolean</span></span>|<span data-ttu-id="dfb10-136">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="dfb10-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="dfb10-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="dfb10-137">soundsEnabled</span></span>|<span data-ttu-id="dfb10-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfb10-138">Boolean</span></span>|<span data-ttu-id="dfb10-139">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="dfb10-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfb10-140">Связи</span><span class="sxs-lookup"><span data-stu-id="dfb10-140">Relationships</span></span>
<span data-ttu-id="dfb10-141">Нет</span><span class="sxs-lookup"><span data-stu-id="dfb10-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfb10-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dfb10-142">JSON Representation</span></span>
<span data-ttu-id="dfb10-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfb10-143">Here is a JSON representation of the resource.</span></span>
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




