---
title: Тип ресурса eBookInstallSummary
description: Содержит свойства сводки по установке книги для устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a3d07dc2d1a1b7a117e001546cd5298765676bdd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986154"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="bc1f2-103">Тип ресурса eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="bc1f2-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="bc1f2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bc1f2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc1f2-105">Содержит свойства сводки по установке книги для устройства.</span><span class="sxs-lookup"><span data-stu-id="bc1f2-105">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="bc1f2-106">Методы</span><span class="sxs-lookup"><span data-stu-id="bc1f2-106">Methods</span></span>
|<span data-ttu-id="bc1f2-107">Метод</span><span class="sxs-lookup"><span data-stu-id="bc1f2-107">Method</span></span>|<span data-ttu-id="bc1f2-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bc1f2-108">Return Type</span></span>|<span data-ttu-id="bc1f2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bc1f2-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc1f2-110">Получение объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="bc1f2-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="bc1f2-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="bc1f2-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="bc1f2-112">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="bc1f2-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="bc1f2-113">Обновление объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="bc1f2-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="bc1f2-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="bc1f2-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="bc1f2-115">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="bc1f2-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc1f2-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc1f2-116">Properties</span></span>
|<span data-ttu-id="bc1f2-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc1f2-117">Property</span></span>|<span data-ttu-id="bc1f2-118">Тип</span><span class="sxs-lookup"><span data-stu-id="bc1f2-118">Type</span></span>|<span data-ttu-id="bc1f2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bc1f2-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc1f2-120">id</span><span class="sxs-lookup"><span data-stu-id="bc1f2-120">id</span></span>|<span data-ttu-id="bc1f2-121">String</span><span class="sxs-lookup"><span data-stu-id="bc1f2-121">String</span></span>|<span data-ttu-id="bc1f2-122">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bc1f2-122">Key of the entity.</span></span>|
|<span data-ttu-id="bc1f2-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bc1f2-123">installedDeviceCount</span></span>|<span data-ttu-id="bc1f2-124">Int32</span><span class="sxs-lookup"><span data-stu-id="bc1f2-124">Int32</span></span>|<span data-ttu-id="bc1f2-125">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="bc1f2-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="bc1f2-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bc1f2-126">failedDeviceCount</span></span>|<span data-ttu-id="bc1f2-127">Int32</span><span class="sxs-lookup"><span data-stu-id="bc1f2-127">Int32</span></span>|<span data-ttu-id="bc1f2-128">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="bc1f2-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="bc1f2-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bc1f2-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="bc1f2-130">Int32</span><span class="sxs-lookup"><span data-stu-id="bc1f2-130">Int32</span></span>|<span data-ttu-id="bc1f2-131">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="bc1f2-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="bc1f2-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="bc1f2-132">installedUserCount</span></span>|<span data-ttu-id="bc1f2-133">Int32</span><span class="sxs-lookup"><span data-stu-id="bc1f2-133">Int32</span></span>|<span data-ttu-id="bc1f2-134">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="bc1f2-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="bc1f2-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="bc1f2-135">failedUserCount</span></span>|<span data-ttu-id="bc1f2-136">Int32</span><span class="sxs-lookup"><span data-stu-id="bc1f2-136">Int32</span></span>|<span data-ttu-id="bc1f2-137">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="bc1f2-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="bc1f2-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="bc1f2-138">notInstalledUserCount</span></span>|<span data-ttu-id="bc1f2-139">Int32</span><span class="sxs-lookup"><span data-stu-id="bc1f2-139">Int32</span></span>|<span data-ttu-id="bc1f2-140">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="bc1f2-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc1f2-141">Связи</span><span class="sxs-lookup"><span data-stu-id="bc1f2-141">Relationships</span></span>
<span data-ttu-id="bc1f2-142">Нет</span><span class="sxs-lookup"><span data-stu-id="bc1f2-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bc1f2-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc1f2-143">JSON Representation</span></span>
<span data-ttu-id="bc1f2-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc1f2-144">Here is a JSON representation of the resource.</span></span>
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



