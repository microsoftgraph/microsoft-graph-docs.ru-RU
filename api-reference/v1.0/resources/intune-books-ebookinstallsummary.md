---
title: Тип ресурса eBookInstallSummary
description: Содержит свойства сводки по установке книги для устройства.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b33f319106c39e11931726fcebcc8d5aa8d6ba46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825783"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="73851-103">Тип ресурса eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="73851-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="73851-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="73851-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73851-105">Содержит свойства сводки по установке книги для устройства.</span><span class="sxs-lookup"><span data-stu-id="73851-105">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="73851-106">Методы</span><span class="sxs-lookup"><span data-stu-id="73851-106">Methods</span></span>
|<span data-ttu-id="73851-107">Метод</span><span class="sxs-lookup"><span data-stu-id="73851-107">Method</span></span>|<span data-ttu-id="73851-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="73851-108">Return Type</span></span>|<span data-ttu-id="73851-109">Описание</span><span class="sxs-lookup"><span data-stu-id="73851-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="73851-110">Получение объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="73851-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="73851-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="73851-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="73851-112">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="73851-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="73851-113">Обновление объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="73851-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="73851-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="73851-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="73851-115">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="73851-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="73851-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="73851-116">Properties</span></span>
|<span data-ttu-id="73851-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="73851-117">Property</span></span>|<span data-ttu-id="73851-118">Тип</span><span class="sxs-lookup"><span data-stu-id="73851-118">Type</span></span>|<span data-ttu-id="73851-119">Описание</span><span class="sxs-lookup"><span data-stu-id="73851-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73851-120">id</span><span class="sxs-lookup"><span data-stu-id="73851-120">id</span></span>|<span data-ttu-id="73851-121">Строка</span><span class="sxs-lookup"><span data-stu-id="73851-121">String</span></span>|<span data-ttu-id="73851-122">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="73851-122">Key of the entity.</span></span>|
|<span data-ttu-id="73851-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="73851-123">installedDeviceCount</span></span>|<span data-ttu-id="73851-124">Int32</span><span class="sxs-lookup"><span data-stu-id="73851-124">Int32</span></span>|<span data-ttu-id="73851-125">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="73851-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="73851-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="73851-126">failedDeviceCount</span></span>|<span data-ttu-id="73851-127">Int32</span><span class="sxs-lookup"><span data-stu-id="73851-127">Int32</span></span>|<span data-ttu-id="73851-128">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="73851-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="73851-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="73851-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="73851-130">Int32</span><span class="sxs-lookup"><span data-stu-id="73851-130">Int32</span></span>|<span data-ttu-id="73851-131">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="73851-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="73851-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="73851-132">installedUserCount</span></span>|<span data-ttu-id="73851-133">Int32</span><span class="sxs-lookup"><span data-stu-id="73851-133">Int32</span></span>|<span data-ttu-id="73851-134">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="73851-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="73851-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="73851-135">failedUserCount</span></span>|<span data-ttu-id="73851-136">Int32</span><span class="sxs-lookup"><span data-stu-id="73851-136">Int32</span></span>|<span data-ttu-id="73851-137">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="73851-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="73851-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="73851-138">notInstalledUserCount</span></span>|<span data-ttu-id="73851-139">Int32</span><span class="sxs-lookup"><span data-stu-id="73851-139">Int32</span></span>|<span data-ttu-id="73851-140">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="73851-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73851-141">Связи</span><span class="sxs-lookup"><span data-stu-id="73851-141">Relationships</span></span>
<span data-ttu-id="73851-142">Нет</span><span class="sxs-lookup"><span data-stu-id="73851-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="73851-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="73851-143">JSON Representation</span></span>
<span data-ttu-id="73851-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73851-144">Here is a JSON representation of the resource.</span></span>
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



