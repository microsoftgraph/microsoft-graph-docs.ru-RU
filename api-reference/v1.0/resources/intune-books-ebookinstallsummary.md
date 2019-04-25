---
title: Тип ресурса eBookInstallSummary
description: Содержит свойства сводки по установке книги для устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17075183e0541669923a69c140d228cb1cbd4a2e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523919"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="ed708-103">Тип ресурса eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ed708-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="ed708-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed708-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed708-105">Содержит свойства сводки по установке книги для устройства.</span><span class="sxs-lookup"><span data-stu-id="ed708-105">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="ed708-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ed708-106">Methods</span></span>
|<span data-ttu-id="ed708-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ed708-107">Method</span></span>|<span data-ttu-id="ed708-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ed708-108">Return Type</span></span>|<span data-ttu-id="ed708-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ed708-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ed708-110">Получение объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ed708-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="ed708-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ed708-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="ed708-112">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ed708-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="ed708-113">Обновление объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ed708-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="ed708-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="ed708-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="ed708-115">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="ed708-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed708-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed708-116">Properties</span></span>
|<span data-ttu-id="ed708-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed708-117">Property</span></span>|<span data-ttu-id="ed708-118">Тип</span><span class="sxs-lookup"><span data-stu-id="ed708-118">Type</span></span>|<span data-ttu-id="ed708-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ed708-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed708-120">id</span><span class="sxs-lookup"><span data-stu-id="ed708-120">id</span></span>|<span data-ttu-id="ed708-121">String</span><span class="sxs-lookup"><span data-stu-id="ed708-121">String</span></span>|<span data-ttu-id="ed708-122">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ed708-122">Key of the entity.</span></span>|
|<span data-ttu-id="ed708-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed708-123">installedDeviceCount</span></span>|<span data-ttu-id="ed708-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ed708-124">Int32</span></span>|<span data-ttu-id="ed708-125">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="ed708-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="ed708-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed708-126">failedDeviceCount</span></span>|<span data-ttu-id="ed708-127">Int32</span><span class="sxs-lookup"><span data-stu-id="ed708-127">Int32</span></span>|<span data-ttu-id="ed708-128">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="ed708-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="ed708-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ed708-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="ed708-130">Int32</span><span class="sxs-lookup"><span data-stu-id="ed708-130">Int32</span></span>|<span data-ttu-id="ed708-131">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="ed708-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="ed708-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="ed708-132">installedUserCount</span></span>|<span data-ttu-id="ed708-133">Int32</span><span class="sxs-lookup"><span data-stu-id="ed708-133">Int32</span></span>|<span data-ttu-id="ed708-134">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="ed708-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="ed708-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="ed708-135">failedUserCount</span></span>|<span data-ttu-id="ed708-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ed708-136">Int32</span></span>|<span data-ttu-id="ed708-137">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="ed708-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="ed708-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="ed708-138">notInstalledUserCount</span></span>|<span data-ttu-id="ed708-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ed708-139">Int32</span></span>|<span data-ttu-id="ed708-140">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="ed708-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed708-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="ed708-141">Relationships</span></span>
<span data-ttu-id="ed708-142">Нет</span><span class="sxs-lookup"><span data-stu-id="ed708-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed708-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed708-143">JSON Representation</span></span>
<span data-ttu-id="ed708-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed708-144">Here is a JSON representation of the resource.</span></span>
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



