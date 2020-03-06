---
title: Тип ресурса eBookInstallSummary
description: Содержит свойства сводки по установке книги для устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8338d2376540d8600d574e56ac38c95d0c6b9626
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531023"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="ed86a-103">Тип ресурса eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ed86a-103">eBookInstallSummary resource type</span></span>

<span data-ttu-id="ed86a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed86a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed86a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed86a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed86a-106">Содержит свойства сводки по установке книги для устройства.</span><span class="sxs-lookup"><span data-stu-id="ed86a-106">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="ed86a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ed86a-107">Methods</span></span>
|<span data-ttu-id="ed86a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ed86a-108">Method</span></span>|<span data-ttu-id="ed86a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ed86a-109">Return Type</span></span>|<span data-ttu-id="ed86a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ed86a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ed86a-111">Получение объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ed86a-111">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="ed86a-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ed86a-112">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="ed86a-113">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ed86a-113">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="ed86a-114">Обновление объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ed86a-114">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="ed86a-115">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ed86a-115">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="ed86a-116">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ed86a-116">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed86a-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed86a-117">Properties</span></span>
|<span data-ttu-id="ed86a-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed86a-118">Property</span></span>|<span data-ttu-id="ed86a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ed86a-119">Type</span></span>|<span data-ttu-id="ed86a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ed86a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed86a-121">id</span><span class="sxs-lookup"><span data-stu-id="ed86a-121">id</span></span>|<span data-ttu-id="ed86a-122">Строка</span><span class="sxs-lookup"><span data-stu-id="ed86a-122">String</span></span>|<span data-ttu-id="ed86a-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ed86a-123">Key of the entity.</span></span>|
|<span data-ttu-id="ed86a-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed86a-124">installedDeviceCount</span></span>|<span data-ttu-id="ed86a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ed86a-125">Int32</span></span>|<span data-ttu-id="ed86a-126">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="ed86a-126">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="ed86a-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed86a-127">failedDeviceCount</span></span>|<span data-ttu-id="ed86a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="ed86a-128">Int32</span></span>|<span data-ttu-id="ed86a-129">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="ed86a-129">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="ed86a-130">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed86a-130">notInstalledDeviceCount</span></span>|<span data-ttu-id="ed86a-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ed86a-131">Int32</span></span>|<span data-ttu-id="ed86a-132">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="ed86a-132">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="ed86a-133">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="ed86a-133">installedUserCount</span></span>|<span data-ttu-id="ed86a-134">Int32</span><span class="sxs-lookup"><span data-stu-id="ed86a-134">Int32</span></span>|<span data-ttu-id="ed86a-135">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="ed86a-135">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="ed86a-136">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="ed86a-136">failedUserCount</span></span>|<span data-ttu-id="ed86a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ed86a-137">Int32</span></span>|<span data-ttu-id="ed86a-138">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="ed86a-138">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="ed86a-139">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="ed86a-139">notInstalledUserCount</span></span>|<span data-ttu-id="ed86a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ed86a-140">Int32</span></span>|<span data-ttu-id="ed86a-141">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="ed86a-141">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed86a-142">Связи</span><span class="sxs-lookup"><span data-stu-id="ed86a-142">Relationships</span></span>
<span data-ttu-id="ed86a-143">Нет</span><span class="sxs-lookup"><span data-stu-id="ed86a-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed86a-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed86a-144">JSON Representation</span></span>
<span data-ttu-id="ed86a-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed86a-145">Here is a JSON representation of the resource.</span></span>
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




