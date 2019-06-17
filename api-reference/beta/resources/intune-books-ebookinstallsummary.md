---
title: Тип ресурса eBookInstallSummary
description: Содержит свойства сводки по установке книги для устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 574ce848e827093f6693a1a7f6a4ebe860833495
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964362"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="6a334-103">Тип ресурса eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6a334-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="6a334-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a334-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a334-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a334-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a334-106">Содержит свойства сводки по установке книги для устройства.</span><span class="sxs-lookup"><span data-stu-id="6a334-106">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="6a334-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6a334-107">Methods</span></span>
|<span data-ttu-id="6a334-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6a334-108">Method</span></span>|<span data-ttu-id="6a334-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6a334-109">Return Type</span></span>|<span data-ttu-id="6a334-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6a334-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6a334-111">Получение объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6a334-111">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="6a334-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6a334-112">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="6a334-113">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="6a334-113">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="6a334-114">Обновление объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6a334-114">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="6a334-115">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="6a334-115">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="6a334-116">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="6a334-116">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a334-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a334-117">Properties</span></span>
|<span data-ttu-id="6a334-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a334-118">Property</span></span>|<span data-ttu-id="6a334-119">Тип</span><span class="sxs-lookup"><span data-stu-id="6a334-119">Type</span></span>|<span data-ttu-id="6a334-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6a334-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a334-121">id</span><span class="sxs-lookup"><span data-stu-id="6a334-121">id</span></span>|<span data-ttu-id="6a334-122">String</span><span class="sxs-lookup"><span data-stu-id="6a334-122">String</span></span>|<span data-ttu-id="6a334-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6a334-123">Key of the entity.</span></span>|
|<span data-ttu-id="6a334-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6a334-124">installedDeviceCount</span></span>|<span data-ttu-id="6a334-125">Int32</span><span class="sxs-lookup"><span data-stu-id="6a334-125">Int32</span></span>|<span data-ttu-id="6a334-126">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="6a334-126">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="6a334-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6a334-127">failedDeviceCount</span></span>|<span data-ttu-id="6a334-128">Int32</span><span class="sxs-lookup"><span data-stu-id="6a334-128">Int32</span></span>|<span data-ttu-id="6a334-129">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="6a334-129">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="6a334-130">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="6a334-130">notInstalledDeviceCount</span></span>|<span data-ttu-id="6a334-131">Int32</span><span class="sxs-lookup"><span data-stu-id="6a334-131">Int32</span></span>|<span data-ttu-id="6a334-132">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="6a334-132">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="6a334-133">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="6a334-133">installedUserCount</span></span>|<span data-ttu-id="6a334-134">Int32</span><span class="sxs-lookup"><span data-stu-id="6a334-134">Int32</span></span>|<span data-ttu-id="6a334-135">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="6a334-135">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="6a334-136">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="6a334-136">failedUserCount</span></span>|<span data-ttu-id="6a334-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6a334-137">Int32</span></span>|<span data-ttu-id="6a334-138">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="6a334-138">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="6a334-139">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="6a334-139">notInstalledUserCount</span></span>|<span data-ttu-id="6a334-140">Int32</span><span class="sxs-lookup"><span data-stu-id="6a334-140">Int32</span></span>|<span data-ttu-id="6a334-141">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="6a334-141">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a334-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="6a334-142">Relationships</span></span>
<span data-ttu-id="6a334-143">Нет</span><span class="sxs-lookup"><span data-stu-id="6a334-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a334-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a334-144">JSON Representation</span></span>
<span data-ttu-id="6a334-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a334-145">Here is a JSON representation of the resource.</span></span>
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





