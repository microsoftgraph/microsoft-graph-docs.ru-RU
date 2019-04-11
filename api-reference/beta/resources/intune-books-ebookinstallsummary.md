---
title: Тип ресурса eBookInstallSummary
description: Содержит свойства сводки по установке книги для устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4eec97cd82224af5e74577a8d9ed9f378534263a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804398"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="53251-103">Тип ресурса eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="53251-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="53251-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53251-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53251-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53251-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53251-106">Содержит свойства сводки по установке книги для устройства.</span><span class="sxs-lookup"><span data-stu-id="53251-106">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="53251-107">Методы</span><span class="sxs-lookup"><span data-stu-id="53251-107">Methods</span></span>
|<span data-ttu-id="53251-108">Метод</span><span class="sxs-lookup"><span data-stu-id="53251-108">Method</span></span>|<span data-ttu-id="53251-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="53251-109">Return Type</span></span>|<span data-ttu-id="53251-110">Описание</span><span class="sxs-lookup"><span data-stu-id="53251-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="53251-111">Get eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="53251-111">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="53251-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="53251-112">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="53251-113">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="53251-113">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="53251-114">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="53251-114">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="53251-115">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="53251-115">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="53251-116">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="53251-116">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="53251-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="53251-117">Properties</span></span>
|<span data-ttu-id="53251-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="53251-118">Property</span></span>|<span data-ttu-id="53251-119">Тип</span><span class="sxs-lookup"><span data-stu-id="53251-119">Type</span></span>|<span data-ttu-id="53251-120">Описание</span><span class="sxs-lookup"><span data-stu-id="53251-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53251-121">id</span><span class="sxs-lookup"><span data-stu-id="53251-121">id</span></span>|<span data-ttu-id="53251-122">String</span><span class="sxs-lookup"><span data-stu-id="53251-122">String</span></span>|<span data-ttu-id="53251-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="53251-123">Key of the entity.</span></span>|
|<span data-ttu-id="53251-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53251-124">installedDeviceCount</span></span>|<span data-ttu-id="53251-125">Int32</span><span class="sxs-lookup"><span data-stu-id="53251-125">Int32</span></span>|<span data-ttu-id="53251-126">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="53251-126">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="53251-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53251-127">failedDeviceCount</span></span>|<span data-ttu-id="53251-128">Int32</span><span class="sxs-lookup"><span data-stu-id="53251-128">Int32</span></span>|<span data-ttu-id="53251-129">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="53251-129">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="53251-130">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="53251-130">notInstalledDeviceCount</span></span>|<span data-ttu-id="53251-131">Int32</span><span class="sxs-lookup"><span data-stu-id="53251-131">Int32</span></span>|<span data-ttu-id="53251-132">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="53251-132">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="53251-133">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="53251-133">installedUserCount</span></span>|<span data-ttu-id="53251-134">Int32</span><span class="sxs-lookup"><span data-stu-id="53251-134">Int32</span></span>|<span data-ttu-id="53251-135">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="53251-135">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="53251-136">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="53251-136">failedUserCount</span></span>|<span data-ttu-id="53251-137">Int32</span><span class="sxs-lookup"><span data-stu-id="53251-137">Int32</span></span>|<span data-ttu-id="53251-138">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="53251-138">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="53251-139">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="53251-139">notInstalledUserCount</span></span>|<span data-ttu-id="53251-140">Int32</span><span class="sxs-lookup"><span data-stu-id="53251-140">Int32</span></span>|<span data-ttu-id="53251-141">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="53251-141">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53251-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="53251-142">Relationships</span></span>
<span data-ttu-id="53251-143">Нет</span><span class="sxs-lookup"><span data-stu-id="53251-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53251-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53251-144">JSON Representation</span></span>
<span data-ttu-id="53251-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53251-145">Here is a JSON representation of the resource.</span></span>
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





