---
title: Тип ресурса userAppInstallStatus
description: Содержит свойства для состояние установки для пользователя.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f4d848a4fe4cd742df8a83184d539d7ff27290b0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885206"
---
# <a name="userappinstallstatus-resource-type"></a><span data-ttu-id="b6123-103">Тип ресурса userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="b6123-103">userAppInstallStatus resource type</span></span>

> <span data-ttu-id="b6123-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b6123-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6123-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6123-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6123-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b6123-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6123-107">Содержит свойства для состояние установки для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b6123-107">Contains properties for the installation status for a user.</span></span>
## <a name="methods"></a><span data-ttu-id="b6123-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b6123-108">Methods</span></span>
|<span data-ttu-id="b6123-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b6123-109">Method</span></span>|<span data-ttu-id="b6123-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b6123-110">Return Type</span></span>|<span data-ttu-id="b6123-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b6123-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b6123-112">Список userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="b6123-112">List userAppInstallStatuses</span></span>](../api/intune-apps-userappinstallstatus-list.md)|<span data-ttu-id="b6123-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b6123-113">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="b6123-114">Свойства списка и связей объектов [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="b6123-114">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>|
|[<span data-ttu-id="b6123-115">Получение userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="b6123-115">Get userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-get.md)|[<span data-ttu-id="b6123-116">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="b6123-116">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="b6123-117">Чтение свойства и связи объекта [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="b6123-117">Read properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="b6123-118">Создание userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="b6123-118">Create userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-create.md)|[<span data-ttu-id="b6123-119">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="b6123-119">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="b6123-120">Создание нового объекта [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="b6123-120">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|
|[<span data-ttu-id="b6123-121">Удаление userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="b6123-121">Delete userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-delete.md)|<span data-ttu-id="b6123-122">Нет</span><span class="sxs-lookup"><span data-stu-id="b6123-122">None</span></span>|<span data-ttu-id="b6123-123">Удаляет [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span><span class="sxs-lookup"><span data-stu-id="b6123-123">Deletes a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>|
|[<span data-ttu-id="b6123-124">Обновление userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="b6123-124">Update userAppInstallStatus</span></span>](../api/intune-apps-userappinstallstatus-update.md)|[<span data-ttu-id="b6123-125">userAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="b6123-125">userAppInstallStatus</span></span>](../resources/intune-apps-userappinstallstatus.md)|<span data-ttu-id="b6123-126">Обновление свойства объекта [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="b6123-126">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b6123-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6123-127">Properties</span></span>
|<span data-ttu-id="b6123-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6123-128">Property</span></span>|<span data-ttu-id="b6123-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b6123-129">Type</span></span>|<span data-ttu-id="b6123-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b6123-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6123-131">id</span><span class="sxs-lookup"><span data-stu-id="b6123-131">id</span></span>|<span data-ttu-id="b6123-132">Строка</span><span class="sxs-lookup"><span data-stu-id="b6123-132">String</span></span>|<span data-ttu-id="b6123-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b6123-133">Key of the entity.</span></span>|
|<span data-ttu-id="b6123-134">userName</span><span class="sxs-lookup"><span data-stu-id="b6123-134">userName</span></span>|<span data-ttu-id="b6123-135">String</span><span class="sxs-lookup"><span data-stu-id="b6123-135">String</span></span>|<span data-ttu-id="b6123-136">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="b6123-136">User name.</span></span>|
|<span data-ttu-id="b6123-137">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b6123-137">userPrincipalName</span></span>|<span data-ttu-id="b6123-138">Строка</span><span class="sxs-lookup"><span data-stu-id="b6123-138">String</span></span>|<span data-ttu-id="b6123-139">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="b6123-139">User Principal Name.</span></span>|
|<span data-ttu-id="b6123-140">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b6123-140">installedDeviceCount</span></span>|<span data-ttu-id="b6123-141">Int32</span><span class="sxs-lookup"><span data-stu-id="b6123-141">Int32</span></span>|<span data-ttu-id="b6123-142">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="b6123-142">Installed Device Count.</span></span>|
|<span data-ttu-id="b6123-143">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b6123-143">failedDeviceCount</span></span>|<span data-ttu-id="b6123-144">Int32</span><span class="sxs-lookup"><span data-stu-id="b6123-144">Int32</span></span>|<span data-ttu-id="b6123-145">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="b6123-145">Failed Device Count.</span></span>|
|<span data-ttu-id="b6123-146">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b6123-146">notInstalledDeviceCount</span></span>|<span data-ttu-id="b6123-147">Int32</span><span class="sxs-lookup"><span data-stu-id="b6123-147">Int32</span></span>|<span data-ttu-id="b6123-148">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="b6123-148">Not installed device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6123-149">Связи</span><span class="sxs-lookup"><span data-stu-id="b6123-149">Relationships</span></span>
|<span data-ttu-id="b6123-150">Связь</span><span class="sxs-lookup"><span data-stu-id="b6123-150">Relationship</span></span>|<span data-ttu-id="b6123-151">Тип</span><span class="sxs-lookup"><span data-stu-id="b6123-151">Type</span></span>|<span data-ttu-id="b6123-152">Описание</span><span class="sxs-lookup"><span data-stu-id="b6123-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6123-153">приложение</span><span class="sxs-lookup"><span data-stu-id="b6123-153">app</span></span>|<span data-ttu-id="b6123-154">[mobileApp](../resources/intune-apps-mobileapp.md);</span><span class="sxs-lookup"><span data-stu-id="b6123-154">[mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|<span data-ttu-id="b6123-155">Навигационная ссылка для мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="b6123-155">The navigation link to the mobile app.</span></span>|
|<span data-ttu-id="b6123-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="b6123-156">deviceStatuses</span></span>|<span data-ttu-id="b6123-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b6123-157">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="b6123-158">Состояние установки приложений на устройствах.</span><span class="sxs-lookup"><span data-stu-id="b6123-158">The install state of the app on devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6123-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6123-159">JSON Representation</span></span>
<span data-ttu-id="b6123-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6123-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "String (identifier)",
  "userName": "String",
  "userPrincipalName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```





