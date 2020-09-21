---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bfe71a68abd7ca55da6bb92654d8af0750a1ef22
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003719"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="7d04e-103">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="7d04e-103">iosNotificationSettings resource type</span></span>

<span data-ttu-id="7d04e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d04e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d04e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d04e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d04e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d04e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d04e-107">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="7d04e-107">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="7d04e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d04e-108">Properties</span></span>
|<span data-ttu-id="7d04e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d04e-109">Property</span></span>|<span data-ttu-id="7d04e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7d04e-110">Type</span></span>|<span data-ttu-id="7d04e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7d04e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d04e-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="7d04e-112">bundleID</span></span>|<span data-ttu-id="7d04e-113">String</span><span class="sxs-lookup"><span data-stu-id="7d04e-113">String</span></span>|<span data-ttu-id="7d04e-114">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="7d04e-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="7d04e-115">appName</span><span class="sxs-lookup"><span data-stu-id="7d04e-115">appName</span></span>|<span data-ttu-id="7d04e-116">String</span><span class="sxs-lookup"><span data-stu-id="7d04e-116">String</span></span>|<span data-ttu-id="7d04e-117">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="7d04e-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="7d04e-118">publisher</span><span class="sxs-lookup"><span data-stu-id="7d04e-118">publisher</span></span>|<span data-ttu-id="7d04e-119">String</span><span class="sxs-lookup"><span data-stu-id="7d04e-119">String</span></span>|<span data-ttu-id="7d04e-120">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="7d04e-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="7d04e-121">enabled</span><span class="sxs-lookup"><span data-stu-id="7d04e-121">enabled</span></span>|<span data-ttu-id="7d04e-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d04e-122">Boolean</span></span>|<span data-ttu-id="7d04e-123">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="7d04e-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="7d04e-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="7d04e-124">showInNotificationCenter</span></span>|<span data-ttu-id="7d04e-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d04e-125">Boolean</span></span>|<span data-ttu-id="7d04e-126">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="7d04e-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="7d04e-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="7d04e-127">showOnLockScreen</span></span>|<span data-ttu-id="7d04e-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d04e-128">Boolean</span></span>|<span data-ttu-id="7d04e-129">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="7d04e-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="7d04e-130">alertType</span><span class="sxs-lookup"><span data-stu-id="7d04e-130">alertType</span></span>|[<span data-ttu-id="7d04e-131">иоснотификатионалерттипе</span><span class="sxs-lookup"><span data-stu-id="7d04e-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="7d04e-132">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="7d04e-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="7d04e-133">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="7d04e-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="7d04e-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="7d04e-134">badgesEnabled</span></span>|<span data-ttu-id="7d04e-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d04e-135">Boolean</span></span>|<span data-ttu-id="7d04e-136">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="7d04e-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="7d04e-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="7d04e-137">soundsEnabled</span></span>|<span data-ttu-id="7d04e-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d04e-138">Boolean</span></span>|<span data-ttu-id="7d04e-139">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="7d04e-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d04e-140">Связи</span><span class="sxs-lookup"><span data-stu-id="7d04e-140">Relationships</span></span>
<span data-ttu-id="7d04e-141">Нет</span><span class="sxs-lookup"><span data-stu-id="7d04e-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d04e-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d04e-142">JSON Representation</span></span>
<span data-ttu-id="7d04e-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d04e-143">Here is a JSON representation of the resource.</span></span>
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






