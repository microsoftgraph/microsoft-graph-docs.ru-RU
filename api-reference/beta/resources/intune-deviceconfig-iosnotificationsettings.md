---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
author: tfitzmac
ms.openlocfilehash: c24e0719e634d2939f88280431538b41fb0a1b5f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359194"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="accdd-103">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="accdd-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="accdd-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="accdd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="accdd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="accdd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="accdd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="accdd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="accdd-107">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="accdd-107">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="accdd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="accdd-108">Properties</span></span>
|<span data-ttu-id="accdd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="accdd-109">Property</span></span>|<span data-ttu-id="accdd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="accdd-110">Type</span></span>|<span data-ttu-id="accdd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="accdd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="accdd-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="accdd-112">bundleID</span></span>|<span data-ttu-id="accdd-113">String</span><span class="sxs-lookup"><span data-stu-id="accdd-113">String</span></span>|<span data-ttu-id="accdd-114">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="accdd-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="accdd-115">appName</span><span class="sxs-lookup"><span data-stu-id="accdd-115">appName</span></span>|<span data-ttu-id="accdd-116">String</span><span class="sxs-lookup"><span data-stu-id="accdd-116">String</span></span>|<span data-ttu-id="accdd-117">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="accdd-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="accdd-118">publisher</span><span class="sxs-lookup"><span data-stu-id="accdd-118">publisher</span></span>|<span data-ttu-id="accdd-119">String</span><span class="sxs-lookup"><span data-stu-id="accdd-119">String</span></span>|<span data-ttu-id="accdd-120">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="accdd-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="accdd-121">enabled</span><span class="sxs-lookup"><span data-stu-id="accdd-121">enabled</span></span>|<span data-ttu-id="accdd-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="accdd-122">Boolean</span></span>|<span data-ttu-id="accdd-123">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="accdd-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="accdd-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="accdd-124">showInNotificationCenter</span></span>|<span data-ttu-id="accdd-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="accdd-125">Boolean</span></span>|<span data-ttu-id="accdd-126">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="accdd-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="accdd-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="accdd-127">showOnLockScreen</span></span>|<span data-ttu-id="accdd-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="accdd-128">Boolean</span></span>|<span data-ttu-id="accdd-129">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="accdd-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="accdd-130">alertType</span><span class="sxs-lookup"><span data-stu-id="accdd-130">alertType</span></span>|[<span data-ttu-id="accdd-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="accdd-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="accdd-132">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="accdd-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="accdd-133">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="accdd-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="accdd-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="accdd-134">badgesEnabled</span></span>|<span data-ttu-id="accdd-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="accdd-135">Boolean</span></span>|<span data-ttu-id="accdd-136">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="accdd-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="accdd-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="accdd-137">soundsEnabled</span></span>|<span data-ttu-id="accdd-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="accdd-138">Boolean</span></span>|<span data-ttu-id="accdd-139">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="accdd-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="accdd-140">Связи</span><span class="sxs-lookup"><span data-stu-id="accdd-140">Relationships</span></span>
<span data-ttu-id="accdd-141">Нет</span><span class="sxs-lookup"><span data-stu-id="accdd-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="accdd-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="accdd-142">JSON Representation</span></span>
<span data-ttu-id="accdd-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="accdd-143">Here is a JSON representation of the resource.</span></span>
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





