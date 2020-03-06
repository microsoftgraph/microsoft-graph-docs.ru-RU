---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 309bc8ce2211f4b2abfb1e72a01c857b9221ae4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530658"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="71291-103">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="71291-103">iosNotificationSettings resource type</span></span>

<span data-ttu-id="71291-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71291-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71291-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71291-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71291-106">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="71291-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="71291-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="71291-107">Properties</span></span>
|<span data-ttu-id="71291-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="71291-108">Property</span></span>|<span data-ttu-id="71291-109">Тип</span><span class="sxs-lookup"><span data-stu-id="71291-109">Type</span></span>|<span data-ttu-id="71291-110">Описание</span><span class="sxs-lookup"><span data-stu-id="71291-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71291-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="71291-111">bundleID</span></span>|<span data-ttu-id="71291-112">Строка</span><span class="sxs-lookup"><span data-stu-id="71291-112">String</span></span>|<span data-ttu-id="71291-113">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="71291-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="71291-114">appName</span><span class="sxs-lookup"><span data-stu-id="71291-114">appName</span></span>|<span data-ttu-id="71291-115">String</span><span class="sxs-lookup"><span data-stu-id="71291-115">String</span></span>|<span data-ttu-id="71291-116">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="71291-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="71291-117">publisher</span><span class="sxs-lookup"><span data-stu-id="71291-117">publisher</span></span>|<span data-ttu-id="71291-118">String</span><span class="sxs-lookup"><span data-stu-id="71291-118">String</span></span>|<span data-ttu-id="71291-119">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="71291-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="71291-120">enabled</span><span class="sxs-lookup"><span data-stu-id="71291-120">enabled</span></span>|<span data-ttu-id="71291-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="71291-121">Boolean</span></span>|<span data-ttu-id="71291-122">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="71291-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="71291-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="71291-123">showInNotificationCenter</span></span>|<span data-ttu-id="71291-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="71291-124">Boolean</span></span>|<span data-ttu-id="71291-125">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="71291-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="71291-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="71291-126">showOnLockScreen</span></span>|<span data-ttu-id="71291-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="71291-127">Boolean</span></span>|<span data-ttu-id="71291-128">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="71291-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="71291-129">alertType</span><span class="sxs-lookup"><span data-stu-id="71291-129">alertType</span></span>|[<span data-ttu-id="71291-130">иоснотификатионалерттипе</span><span class="sxs-lookup"><span data-stu-id="71291-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="71291-131">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="71291-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="71291-132">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="71291-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="71291-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="71291-133">badgesEnabled</span></span>|<span data-ttu-id="71291-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="71291-134">Boolean</span></span>|<span data-ttu-id="71291-135">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="71291-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="71291-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="71291-136">soundsEnabled</span></span>|<span data-ttu-id="71291-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="71291-137">Boolean</span></span>|<span data-ttu-id="71291-138">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="71291-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71291-139">Связи</span><span class="sxs-lookup"><span data-stu-id="71291-139">Relationships</span></span>
<span data-ttu-id="71291-140">Нет</span><span class="sxs-lookup"><span data-stu-id="71291-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71291-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71291-141">JSON Representation</span></span>
<span data-ttu-id="71291-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71291-142">Here is a JSON representation of the resource.</span></span>
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




