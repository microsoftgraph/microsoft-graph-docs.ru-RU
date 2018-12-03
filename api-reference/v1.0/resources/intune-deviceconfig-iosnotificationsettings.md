---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
ms.openlocfilehash: 40f23c228bf10cfb7f273efbe343c1ff773ac280
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027504"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="6350d-103">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="6350d-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="6350d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6350d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6350d-105">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="6350d-105">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="6350d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6350d-106">Properties</span></span>
|<span data-ttu-id="6350d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6350d-107">Property</span></span>|<span data-ttu-id="6350d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6350d-108">Type</span></span>|<span data-ttu-id="6350d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6350d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6350d-110">bundleID</span><span class="sxs-lookup"><span data-stu-id="6350d-110">bundleID</span></span>|<span data-ttu-id="6350d-111">String</span><span class="sxs-lookup"><span data-stu-id="6350d-111">String</span></span>|<span data-ttu-id="6350d-112">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="6350d-112">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="6350d-113">appName</span><span class="sxs-lookup"><span data-stu-id="6350d-113">appName</span></span>|<span data-ttu-id="6350d-114">String</span><span class="sxs-lookup"><span data-stu-id="6350d-114">String</span></span>|<span data-ttu-id="6350d-115">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="6350d-115">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="6350d-116">publisher</span><span class="sxs-lookup"><span data-stu-id="6350d-116">publisher</span></span>|<span data-ttu-id="6350d-117">String</span><span class="sxs-lookup"><span data-stu-id="6350d-117">String</span></span>|<span data-ttu-id="6350d-118">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="6350d-118">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="6350d-119">enabled</span><span class="sxs-lookup"><span data-stu-id="6350d-119">enabled</span></span>|<span data-ttu-id="6350d-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="6350d-120">Boolean</span></span>|<span data-ttu-id="6350d-121">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="6350d-121">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="6350d-122">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="6350d-122">showInNotificationCenter</span></span>|<span data-ttu-id="6350d-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="6350d-123">Boolean</span></span>|<span data-ttu-id="6350d-124">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="6350d-124">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="6350d-125">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="6350d-125">showOnLockScreen</span></span>|<span data-ttu-id="6350d-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="6350d-126">Boolean</span></span>|<span data-ttu-id="6350d-127">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="6350d-127">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="6350d-128">alertType</span><span class="sxs-lookup"><span data-stu-id="6350d-128">alertType</span></span>|[<span data-ttu-id="6350d-129">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="6350d-129">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="6350d-130">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="6350d-130">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="6350d-131">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="6350d-131">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="6350d-132">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="6350d-132">badgesEnabled</span></span>|<span data-ttu-id="6350d-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="6350d-133">Boolean</span></span>|<span data-ttu-id="6350d-134">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="6350d-134">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="6350d-135">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="6350d-135">soundsEnabled</span></span>|<span data-ttu-id="6350d-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="6350d-136">Boolean</span></span>|<span data-ttu-id="6350d-137">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="6350d-137">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6350d-138">Связи</span><span class="sxs-lookup"><span data-stu-id="6350d-138">Relationships</span></span>
<span data-ttu-id="6350d-139">Нет</span><span class="sxs-lookup"><span data-stu-id="6350d-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6350d-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6350d-140">JSON Representation</span></span>
<span data-ttu-id="6350d-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6350d-141">Here is a JSON representation of the resource.</span></span>
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



