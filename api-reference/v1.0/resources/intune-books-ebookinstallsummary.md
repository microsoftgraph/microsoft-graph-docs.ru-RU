---
title: Тип ресурса eBookInstallSummary
description: Содержит свойства сводки по установке книги для устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e5068e7c84797898e33b13fc503f11aaf7ad081b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468783"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="f44f4-103">Тип ресурса eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f44f4-103">eBookInstallSummary resource type</span></span>

<span data-ttu-id="f44f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f44f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f44f4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f44f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f44f4-106">Содержит свойства сводки по установке книги для устройства.</span><span class="sxs-lookup"><span data-stu-id="f44f4-106">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="f44f4-107">Методы</span><span class="sxs-lookup"><span data-stu-id="f44f4-107">Methods</span></span>
|<span data-ttu-id="f44f4-108">Метод</span><span class="sxs-lookup"><span data-stu-id="f44f4-108">Method</span></span>|<span data-ttu-id="f44f4-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f44f4-109">Return Type</span></span>|<span data-ttu-id="f44f4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f44f4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f44f4-111">Получение объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f44f4-111">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="f44f4-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f44f4-112">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="f44f4-113">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f44f4-113">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="f44f4-114">Обновление объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f44f4-114">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="f44f4-115">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f44f4-115">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="f44f4-116">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="f44f4-116">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f44f4-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="f44f4-117">Properties</span></span>
|<span data-ttu-id="f44f4-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="f44f4-118">Property</span></span>|<span data-ttu-id="f44f4-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f44f4-119">Type</span></span>|<span data-ttu-id="f44f4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f44f4-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f44f4-121">id</span><span class="sxs-lookup"><span data-stu-id="f44f4-121">id</span></span>|<span data-ttu-id="f44f4-122">String</span><span class="sxs-lookup"><span data-stu-id="f44f4-122">String</span></span>|<span data-ttu-id="f44f4-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f44f4-123">Key of the entity.</span></span>|
|<span data-ttu-id="f44f4-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f44f4-124">installedDeviceCount</span></span>|<span data-ttu-id="f44f4-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f44f4-125">Int32</span></span>|<span data-ttu-id="f44f4-126">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="f44f4-126">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="f44f4-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f44f4-127">failedDeviceCount</span></span>|<span data-ttu-id="f44f4-128">Int32</span><span class="sxs-lookup"><span data-stu-id="f44f4-128">Int32</span></span>|<span data-ttu-id="f44f4-129">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="f44f4-129">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="f44f4-130">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f44f4-130">notInstalledDeviceCount</span></span>|<span data-ttu-id="f44f4-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f44f4-131">Int32</span></span>|<span data-ttu-id="f44f4-132">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="f44f4-132">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="f44f4-133">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="f44f4-133">installedUserCount</span></span>|<span data-ttu-id="f44f4-134">Int32</span><span class="sxs-lookup"><span data-stu-id="f44f4-134">Int32</span></span>|<span data-ttu-id="f44f4-135">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="f44f4-135">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="f44f4-136">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="f44f4-136">failedUserCount</span></span>|<span data-ttu-id="f44f4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f44f4-137">Int32</span></span>|<span data-ttu-id="f44f4-138">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="f44f4-138">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="f44f4-139">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="f44f4-139">notInstalledUserCount</span></span>|<span data-ttu-id="f44f4-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f44f4-140">Int32</span></span>|<span data-ttu-id="f44f4-141">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="f44f4-141">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f44f4-142">Связи</span><span class="sxs-lookup"><span data-stu-id="f44f4-142">Relationships</span></span>
<span data-ttu-id="f44f4-143">Нет</span><span class="sxs-lookup"><span data-stu-id="f44f4-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f44f4-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f44f4-144">JSON Representation</span></span>
<span data-ttu-id="f44f4-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f44f4-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```







