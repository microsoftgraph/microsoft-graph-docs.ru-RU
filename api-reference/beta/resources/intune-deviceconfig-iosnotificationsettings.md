---
title: Тип ресурса iosNotificationSettings
description: Элемент, описывающий параметры уведомлений.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a14233ef8f74aa0aeeb7e21be3fc819aec985a4d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440250"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="98aff-103">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="98aff-103">iosNotificationSettings resource type</span></span>

<span data-ttu-id="98aff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98aff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98aff-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98aff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98aff-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98aff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98aff-107">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="98aff-107">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="98aff-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="98aff-108">Properties</span></span>
|<span data-ttu-id="98aff-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="98aff-109">Property</span></span>|<span data-ttu-id="98aff-110">Тип</span><span class="sxs-lookup"><span data-stu-id="98aff-110">Type</span></span>|<span data-ttu-id="98aff-111">Описание</span><span class="sxs-lookup"><span data-stu-id="98aff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98aff-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="98aff-112">bundleID</span></span>|<span data-ttu-id="98aff-113">String</span><span class="sxs-lookup"><span data-stu-id="98aff-113">String</span></span>|<span data-ttu-id="98aff-114">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="98aff-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="98aff-115">appName</span><span class="sxs-lookup"><span data-stu-id="98aff-115">appName</span></span>|<span data-ttu-id="98aff-116">String</span><span class="sxs-lookup"><span data-stu-id="98aff-116">String</span></span>|<span data-ttu-id="98aff-117">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="98aff-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="98aff-118">publisher</span><span class="sxs-lookup"><span data-stu-id="98aff-118">publisher</span></span>|<span data-ttu-id="98aff-119">String</span><span class="sxs-lookup"><span data-stu-id="98aff-119">String</span></span>|<span data-ttu-id="98aff-120">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="98aff-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="98aff-121">enabled</span><span class="sxs-lookup"><span data-stu-id="98aff-121">enabled</span></span>|<span data-ttu-id="98aff-122">Логическое</span><span class="sxs-lookup"><span data-stu-id="98aff-122">Boolean</span></span>|<span data-ttu-id="98aff-123">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="98aff-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="98aff-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="98aff-124">showInNotificationCenter</span></span>|<span data-ttu-id="98aff-125">Логическое</span><span class="sxs-lookup"><span data-stu-id="98aff-125">Boolean</span></span>|<span data-ttu-id="98aff-126">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="98aff-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="98aff-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="98aff-127">showOnLockScreen</span></span>|<span data-ttu-id="98aff-128">Логическое</span><span class="sxs-lookup"><span data-stu-id="98aff-128">Boolean</span></span>|<span data-ttu-id="98aff-129">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="98aff-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="98aff-130">alertType</span><span class="sxs-lookup"><span data-stu-id="98aff-130">alertType</span></span>|[<span data-ttu-id="98aff-131">иоснотификатионалерттипе</span><span class="sxs-lookup"><span data-stu-id="98aff-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="98aff-132">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="98aff-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="98aff-133">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="98aff-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="98aff-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="98aff-134">badgesEnabled</span></span>|<span data-ttu-id="98aff-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="98aff-135">Boolean</span></span>|<span data-ttu-id="98aff-136">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="98aff-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="98aff-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="98aff-137">soundsEnabled</span></span>|<span data-ttu-id="98aff-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="98aff-138">Boolean</span></span>|<span data-ttu-id="98aff-139">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="98aff-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98aff-140">Связи</span><span class="sxs-lookup"><span data-stu-id="98aff-140">Relationships</span></span>
<span data-ttu-id="98aff-141">Нет</span><span class="sxs-lookup"><span data-stu-id="98aff-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98aff-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98aff-142">JSON Representation</span></span>
<span data-ttu-id="98aff-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98aff-143">Here is a JSON representation of the resource.</span></span>
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



