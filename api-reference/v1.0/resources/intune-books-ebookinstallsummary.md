---
title: Тип ресурса eBookInstallSummary
description: Содержит свойства сводки по установке книги для устройства.
ms.openlocfilehash: 59754a8b925f573e44abd9ae1f674ab3f08f51c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027851"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="184db-103">Тип ресурса eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="184db-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="184db-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="184db-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="184db-105">Содержит свойства сводки по установке книги для устройства.</span><span class="sxs-lookup"><span data-stu-id="184db-105">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="184db-106">Методы</span><span class="sxs-lookup"><span data-stu-id="184db-106">Methods</span></span>
|<span data-ttu-id="184db-107">Метод</span><span class="sxs-lookup"><span data-stu-id="184db-107">Method</span></span>|<span data-ttu-id="184db-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="184db-108">Return Type</span></span>|<span data-ttu-id="184db-109">Описание</span><span class="sxs-lookup"><span data-stu-id="184db-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="184db-110">Получение объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="184db-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="184db-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="184db-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="184db-112">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="184db-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="184db-113">Обновление объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="184db-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="184db-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="184db-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="184db-115">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="184db-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="184db-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="184db-116">Properties</span></span>
|<span data-ttu-id="184db-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="184db-117">Property</span></span>|<span data-ttu-id="184db-118">Тип</span><span class="sxs-lookup"><span data-stu-id="184db-118">Type</span></span>|<span data-ttu-id="184db-119">Описание</span><span class="sxs-lookup"><span data-stu-id="184db-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="184db-120">id</span><span class="sxs-lookup"><span data-stu-id="184db-120">id</span></span>|<span data-ttu-id="184db-121">String</span><span class="sxs-lookup"><span data-stu-id="184db-121">String</span></span>|<span data-ttu-id="184db-122">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="184db-122">Key of the entity.</span></span>|
|<span data-ttu-id="184db-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="184db-123">installedDeviceCount</span></span>|<span data-ttu-id="184db-124">Int32</span><span class="sxs-lookup"><span data-stu-id="184db-124">Int32</span></span>|<span data-ttu-id="184db-125">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="184db-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="184db-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="184db-126">failedDeviceCount</span></span>|<span data-ttu-id="184db-127">Int32</span><span class="sxs-lookup"><span data-stu-id="184db-127">Int32</span></span>|<span data-ttu-id="184db-128">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="184db-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="184db-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="184db-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="184db-130">Int32</span><span class="sxs-lookup"><span data-stu-id="184db-130">Int32</span></span>|<span data-ttu-id="184db-131">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="184db-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="184db-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="184db-132">installedUserCount</span></span>|<span data-ttu-id="184db-133">Int32</span><span class="sxs-lookup"><span data-stu-id="184db-133">Int32</span></span>|<span data-ttu-id="184db-134">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="184db-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="184db-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="184db-135">failedUserCount</span></span>|<span data-ttu-id="184db-136">Int32</span><span class="sxs-lookup"><span data-stu-id="184db-136">Int32</span></span>|<span data-ttu-id="184db-137">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="184db-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="184db-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="184db-138">notInstalledUserCount</span></span>|<span data-ttu-id="184db-139">Int32</span><span class="sxs-lookup"><span data-stu-id="184db-139">Int32</span></span>|<span data-ttu-id="184db-140">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="184db-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="184db-141">Связи</span><span class="sxs-lookup"><span data-stu-id="184db-141">Relationships</span></span>
<span data-ttu-id="184db-142">Нет</span><span class="sxs-lookup"><span data-stu-id="184db-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="184db-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="184db-143">JSON Representation</span></span>
<span data-ttu-id="184db-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="184db-144">Here is a JSON representation of the resource.</span></span>
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



