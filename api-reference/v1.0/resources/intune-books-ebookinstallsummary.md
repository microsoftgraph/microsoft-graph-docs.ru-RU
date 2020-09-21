---
title: Тип ресурса eBookInstallSummary
description: Содержит свойства сводки по установке книги для устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5f39a7327ecd8d5c87636d2194eb7ef35cb8cff2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965661"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="26f9a-103">Тип ресурса eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="26f9a-103">eBookInstallSummary resource type</span></span>

<span data-ttu-id="26f9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26f9a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26f9a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26f9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26f9a-106">Содержит свойства сводки по установке книги для устройства.</span><span class="sxs-lookup"><span data-stu-id="26f9a-106">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="26f9a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="26f9a-107">Methods</span></span>
|<span data-ttu-id="26f9a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="26f9a-108">Method</span></span>|<span data-ttu-id="26f9a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="26f9a-109">Return Type</span></span>|<span data-ttu-id="26f9a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="26f9a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="26f9a-111">Получение объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="26f9a-111">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="26f9a-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="26f9a-112">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="26f9a-113">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="26f9a-113">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="26f9a-114">Обновление объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="26f9a-114">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="26f9a-115">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="26f9a-115">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="26f9a-116">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="26f9a-116">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="26f9a-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="26f9a-117">Properties</span></span>
|<span data-ttu-id="26f9a-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="26f9a-118">Property</span></span>|<span data-ttu-id="26f9a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="26f9a-119">Type</span></span>|<span data-ttu-id="26f9a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="26f9a-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26f9a-121">id</span><span class="sxs-lookup"><span data-stu-id="26f9a-121">id</span></span>|<span data-ttu-id="26f9a-122">String</span><span class="sxs-lookup"><span data-stu-id="26f9a-122">String</span></span>|<span data-ttu-id="26f9a-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="26f9a-123">Key of the entity.</span></span>|
|<span data-ttu-id="26f9a-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26f9a-124">installedDeviceCount</span></span>|<span data-ttu-id="26f9a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="26f9a-125">Int32</span></span>|<span data-ttu-id="26f9a-126">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="26f9a-126">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="26f9a-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26f9a-127">failedDeviceCount</span></span>|<span data-ttu-id="26f9a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="26f9a-128">Int32</span></span>|<span data-ttu-id="26f9a-129">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="26f9a-129">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="26f9a-130">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="26f9a-130">notInstalledDeviceCount</span></span>|<span data-ttu-id="26f9a-131">Int32</span><span class="sxs-lookup"><span data-stu-id="26f9a-131">Int32</span></span>|<span data-ttu-id="26f9a-132">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="26f9a-132">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="26f9a-133">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="26f9a-133">installedUserCount</span></span>|<span data-ttu-id="26f9a-134">Int32</span><span class="sxs-lookup"><span data-stu-id="26f9a-134">Int32</span></span>|<span data-ttu-id="26f9a-135">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="26f9a-135">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="26f9a-136">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="26f9a-136">failedUserCount</span></span>|<span data-ttu-id="26f9a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="26f9a-137">Int32</span></span>|<span data-ttu-id="26f9a-138">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="26f9a-138">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="26f9a-139">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="26f9a-139">notInstalledUserCount</span></span>|<span data-ttu-id="26f9a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="26f9a-140">Int32</span></span>|<span data-ttu-id="26f9a-141">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="26f9a-141">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26f9a-142">Связи</span><span class="sxs-lookup"><span data-stu-id="26f9a-142">Relationships</span></span>
<span data-ttu-id="26f9a-143">Нет</span><span class="sxs-lookup"><span data-stu-id="26f9a-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26f9a-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26f9a-144">JSON Representation</span></span>
<span data-ttu-id="26f9a-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26f9a-145">Here is a JSON representation of the resource.</span></span>
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









