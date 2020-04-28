---
title: Тип ресурса eBookInstallSummary
description: Содержит свойства сводки по установке книги для устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b305d2814abf04725cd1a42acf05b90f96f0dd8b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472088"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="7df9a-103">Тип ресурса eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7df9a-103">eBookInstallSummary resource type</span></span>

<span data-ttu-id="7df9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7df9a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7df9a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7df9a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7df9a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7df9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7df9a-107">Содержит свойства сводки по установке книги для устройства.</span><span class="sxs-lookup"><span data-stu-id="7df9a-107">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="7df9a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="7df9a-108">Methods</span></span>
|<span data-ttu-id="7df9a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="7df9a-109">Method</span></span>|<span data-ttu-id="7df9a-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7df9a-110">Return Type</span></span>|<span data-ttu-id="7df9a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7df9a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7df9a-112">Получение объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7df9a-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="7df9a-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7df9a-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="7df9a-114">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="7df9a-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="7df9a-115">Обновление объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7df9a-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="7df9a-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7df9a-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="7df9a-117">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="7df9a-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7df9a-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="7df9a-118">Properties</span></span>
|<span data-ttu-id="7df9a-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="7df9a-119">Property</span></span>|<span data-ttu-id="7df9a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7df9a-120">Type</span></span>|<span data-ttu-id="7df9a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7df9a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7df9a-122">id</span><span class="sxs-lookup"><span data-stu-id="7df9a-122">id</span></span>|<span data-ttu-id="7df9a-123">String</span><span class="sxs-lookup"><span data-stu-id="7df9a-123">String</span></span>|<span data-ttu-id="7df9a-124">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7df9a-124">Key of the entity.</span></span>|
|<span data-ttu-id="7df9a-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7df9a-125">installedDeviceCount</span></span>|<span data-ttu-id="7df9a-126">Int32</span><span class="sxs-lookup"><span data-stu-id="7df9a-126">Int32</span></span>|<span data-ttu-id="7df9a-127">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="7df9a-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="7df9a-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7df9a-128">failedDeviceCount</span></span>|<span data-ttu-id="7df9a-129">Int32</span><span class="sxs-lookup"><span data-stu-id="7df9a-129">Int32</span></span>|<span data-ttu-id="7df9a-130">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="7df9a-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="7df9a-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7df9a-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="7df9a-132">Int32</span><span class="sxs-lookup"><span data-stu-id="7df9a-132">Int32</span></span>|<span data-ttu-id="7df9a-133">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="7df9a-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="7df9a-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="7df9a-134">installedUserCount</span></span>|<span data-ttu-id="7df9a-135">Int32</span><span class="sxs-lookup"><span data-stu-id="7df9a-135">Int32</span></span>|<span data-ttu-id="7df9a-136">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="7df9a-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="7df9a-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="7df9a-137">failedUserCount</span></span>|<span data-ttu-id="7df9a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7df9a-138">Int32</span></span>|<span data-ttu-id="7df9a-139">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="7df9a-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="7df9a-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="7df9a-140">notInstalledUserCount</span></span>|<span data-ttu-id="7df9a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="7df9a-141">Int32</span></span>|<span data-ttu-id="7df9a-142">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="7df9a-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7df9a-143">Связи</span><span class="sxs-lookup"><span data-stu-id="7df9a-143">Relationships</span></span>
<span data-ttu-id="7df9a-144">Нет</span><span class="sxs-lookup"><span data-stu-id="7df9a-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7df9a-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7df9a-145">JSON Representation</span></span>
<span data-ttu-id="7df9a-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7df9a-146">Here is a JSON representation of the resource.</span></span>
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



