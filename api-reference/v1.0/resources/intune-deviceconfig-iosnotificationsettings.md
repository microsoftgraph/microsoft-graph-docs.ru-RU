---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 438b1cf075aa1e1cedafc8340b33186965691424
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760031"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="4dc49-103">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="4dc49-103">iosNotificationSettings resource type</span></span>

<span data-ttu-id="4dc49-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dc49-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4dc49-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4dc49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dc49-106">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="4dc49-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="4dc49-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4dc49-107">Properties</span></span>
|<span data-ttu-id="4dc49-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4dc49-108">Property</span></span>|<span data-ttu-id="4dc49-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4dc49-109">Type</span></span>|<span data-ttu-id="4dc49-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4dc49-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dc49-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="4dc49-111">bundleID</span></span>|<span data-ttu-id="4dc49-112">String</span><span class="sxs-lookup"><span data-stu-id="4dc49-112">String</span></span>|<span data-ttu-id="4dc49-113">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="4dc49-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="4dc49-114">appName</span><span class="sxs-lookup"><span data-stu-id="4dc49-114">appName</span></span>|<span data-ttu-id="4dc49-115">String</span><span class="sxs-lookup"><span data-stu-id="4dc49-115">String</span></span>|<span data-ttu-id="4dc49-116">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="4dc49-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="4dc49-117">publisher</span><span class="sxs-lookup"><span data-stu-id="4dc49-117">publisher</span></span>|<span data-ttu-id="4dc49-118">String</span><span class="sxs-lookup"><span data-stu-id="4dc49-118">String</span></span>|<span data-ttu-id="4dc49-119">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="4dc49-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="4dc49-120">enabled</span><span class="sxs-lookup"><span data-stu-id="4dc49-120">enabled</span></span>|<span data-ttu-id="4dc49-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dc49-121">Boolean</span></span>|<span data-ttu-id="4dc49-122">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="4dc49-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="4dc49-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="4dc49-123">showInNotificationCenter</span></span>|<span data-ttu-id="4dc49-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dc49-124">Boolean</span></span>|<span data-ttu-id="4dc49-125">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="4dc49-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="4dc49-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="4dc49-126">showOnLockScreen</span></span>|<span data-ttu-id="4dc49-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dc49-127">Boolean</span></span>|<span data-ttu-id="4dc49-128">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="4dc49-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="4dc49-129">alertType</span><span class="sxs-lookup"><span data-stu-id="4dc49-129">alertType</span></span>|[<span data-ttu-id="4dc49-130">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="4dc49-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="4dc49-131">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="4dc49-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="4dc49-132">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="4dc49-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="4dc49-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="4dc49-133">badgesEnabled</span></span>|<span data-ttu-id="4dc49-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dc49-134">Boolean</span></span>|<span data-ttu-id="4dc49-135">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="4dc49-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="4dc49-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="4dc49-136">soundsEnabled</span></span>|<span data-ttu-id="4dc49-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="4dc49-137">Boolean</span></span>|<span data-ttu-id="4dc49-138">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="4dc49-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dc49-139">Связи</span><span class="sxs-lookup"><span data-stu-id="4dc49-139">Relationships</span></span>
<span data-ttu-id="4dc49-140">Нет</span><span class="sxs-lookup"><span data-stu-id="4dc49-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4dc49-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4dc49-141">JSON Representation</span></span>
<span data-ttu-id="4dc49-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4dc49-142">Here is a JSON representation of the resource.</span></span>
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




