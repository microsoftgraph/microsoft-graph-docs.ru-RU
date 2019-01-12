---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 242a15d4b636cf73f0e9a9f29a3f53ce17f2fd00
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972980"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="234ab-103">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="234ab-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="234ab-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="234ab-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="234ab-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="234ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="234ab-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="234ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="234ab-107">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="234ab-107">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="234ab-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="234ab-108">Properties</span></span>
|<span data-ttu-id="234ab-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="234ab-109">Property</span></span>|<span data-ttu-id="234ab-110">Тип</span><span class="sxs-lookup"><span data-stu-id="234ab-110">Type</span></span>|<span data-ttu-id="234ab-111">Описание</span><span class="sxs-lookup"><span data-stu-id="234ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="234ab-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="234ab-112">bundleID</span></span>|<span data-ttu-id="234ab-113">String</span><span class="sxs-lookup"><span data-stu-id="234ab-113">String</span></span>|<span data-ttu-id="234ab-114">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="234ab-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="234ab-115">appName</span><span class="sxs-lookup"><span data-stu-id="234ab-115">appName</span></span>|<span data-ttu-id="234ab-116">String</span><span class="sxs-lookup"><span data-stu-id="234ab-116">String</span></span>|<span data-ttu-id="234ab-117">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="234ab-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="234ab-118">publisher</span><span class="sxs-lookup"><span data-stu-id="234ab-118">publisher</span></span>|<span data-ttu-id="234ab-119">String</span><span class="sxs-lookup"><span data-stu-id="234ab-119">String</span></span>|<span data-ttu-id="234ab-120">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="234ab-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="234ab-121">enabled</span><span class="sxs-lookup"><span data-stu-id="234ab-121">enabled</span></span>|<span data-ttu-id="234ab-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="234ab-122">Boolean</span></span>|<span data-ttu-id="234ab-123">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="234ab-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="234ab-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="234ab-124">showInNotificationCenter</span></span>|<span data-ttu-id="234ab-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="234ab-125">Boolean</span></span>|<span data-ttu-id="234ab-126">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="234ab-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="234ab-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="234ab-127">showOnLockScreen</span></span>|<span data-ttu-id="234ab-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="234ab-128">Boolean</span></span>|<span data-ttu-id="234ab-129">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="234ab-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="234ab-130">alertType</span><span class="sxs-lookup"><span data-stu-id="234ab-130">alertType</span></span>|[<span data-ttu-id="234ab-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="234ab-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="234ab-132">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="234ab-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="234ab-133">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="234ab-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="234ab-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="234ab-134">badgesEnabled</span></span>|<span data-ttu-id="234ab-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="234ab-135">Boolean</span></span>|<span data-ttu-id="234ab-136">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="234ab-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="234ab-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="234ab-137">soundsEnabled</span></span>|<span data-ttu-id="234ab-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="234ab-138">Boolean</span></span>|<span data-ttu-id="234ab-139">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="234ab-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="234ab-140">Связи</span><span class="sxs-lookup"><span data-stu-id="234ab-140">Relationships</span></span>
<span data-ttu-id="234ab-141">Нет</span><span class="sxs-lookup"><span data-stu-id="234ab-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="234ab-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="234ab-142">JSON Representation</span></span>
<span data-ttu-id="234ab-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="234ab-143">Here is a JSON representation of the resource.</span></span>
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





