---
title: Тип ресурса eBookInstallSummary
description: Содержит свойства сводки по установке книги для устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a68033930abb413ab7c2640381120b86c9873359
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355962"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="00476-103">Тип ресурса eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="00476-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="00476-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00476-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00476-105">Содержит свойства сводки по установке книги для устройства.</span><span class="sxs-lookup"><span data-stu-id="00476-105">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="00476-106">Методы</span><span class="sxs-lookup"><span data-stu-id="00476-106">Methods</span></span>
|<span data-ttu-id="00476-107">Метод</span><span class="sxs-lookup"><span data-stu-id="00476-107">Method</span></span>|<span data-ttu-id="00476-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="00476-108">Return Type</span></span>|<span data-ttu-id="00476-109">Описание</span><span class="sxs-lookup"><span data-stu-id="00476-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="00476-110">Получение объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="00476-110">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="00476-111">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="00476-111">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="00476-112">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="00476-112">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="00476-113">Обновление объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="00476-113">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="00476-114">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="00476-114">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="00476-115">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="00476-115">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="00476-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="00476-116">Properties</span></span>
|<span data-ttu-id="00476-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="00476-117">Property</span></span>|<span data-ttu-id="00476-118">Тип</span><span class="sxs-lookup"><span data-stu-id="00476-118">Type</span></span>|<span data-ttu-id="00476-119">Описание</span><span class="sxs-lookup"><span data-stu-id="00476-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00476-120">id</span><span class="sxs-lookup"><span data-stu-id="00476-120">id</span></span>|<span data-ttu-id="00476-121">String</span><span class="sxs-lookup"><span data-stu-id="00476-121">String</span></span>|<span data-ttu-id="00476-122">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="00476-122">Key of the entity.</span></span>|
|<span data-ttu-id="00476-123">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="00476-123">installedDeviceCount</span></span>|<span data-ttu-id="00476-124">Int32</span><span class="sxs-lookup"><span data-stu-id="00476-124">Int32</span></span>|<span data-ttu-id="00476-125">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="00476-125">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="00476-126">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="00476-126">failedDeviceCount</span></span>|<span data-ttu-id="00476-127">Int32</span><span class="sxs-lookup"><span data-stu-id="00476-127">Int32</span></span>|<span data-ttu-id="00476-128">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="00476-128">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="00476-129">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="00476-129">notInstalledDeviceCount</span></span>|<span data-ttu-id="00476-130">Int32</span><span class="sxs-lookup"><span data-stu-id="00476-130">Int32</span></span>|<span data-ttu-id="00476-131">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="00476-131">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="00476-132">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="00476-132">installedUserCount</span></span>|<span data-ttu-id="00476-133">Int32</span><span class="sxs-lookup"><span data-stu-id="00476-133">Int32</span></span>|<span data-ttu-id="00476-134">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="00476-134">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="00476-135">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="00476-135">failedUserCount</span></span>|<span data-ttu-id="00476-136">Int32</span><span class="sxs-lookup"><span data-stu-id="00476-136">Int32</span></span>|<span data-ttu-id="00476-137">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="00476-137">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="00476-138">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="00476-138">notInstalledUserCount</span></span>|<span data-ttu-id="00476-139">Int32</span><span class="sxs-lookup"><span data-stu-id="00476-139">Int32</span></span>|<span data-ttu-id="00476-140">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="00476-140">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00476-141">Связи</span><span class="sxs-lookup"><span data-stu-id="00476-141">Relationships</span></span>
<span data-ttu-id="00476-142">Нет</span><span class="sxs-lookup"><span data-stu-id="00476-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00476-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00476-143">JSON Representation</span></span>
<span data-ttu-id="00476-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00476-144">Here is a JSON representation of the resource.</span></span>
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




