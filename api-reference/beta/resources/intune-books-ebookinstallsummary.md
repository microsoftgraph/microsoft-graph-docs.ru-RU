---
title: Тип ресурса eBookInstallSummary
description: Содержит свойства сводки по установке книги для устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4e8952012624a038f497fea3c6b81ad364448a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415343"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="b5987-103">Тип ресурса eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b5987-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="b5987-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b5987-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b5987-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5987-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5987-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5987-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5987-107">Содержит свойства сводки по установке книги для устройства.</span><span class="sxs-lookup"><span data-stu-id="b5987-107">Contains properties for the installation summary of a book for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="b5987-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b5987-108">Methods</span></span>
|<span data-ttu-id="b5987-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b5987-109">Method</span></span>|<span data-ttu-id="b5987-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b5987-110">Return Type</span></span>|<span data-ttu-id="b5987-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b5987-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b5987-112">Получение объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b5987-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="b5987-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b5987-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="b5987-114">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b5987-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="b5987-115">Обновление объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b5987-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="b5987-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="b5987-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="b5987-117">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="b5987-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b5987-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5987-118">Properties</span></span>
|<span data-ttu-id="b5987-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5987-119">Property</span></span>|<span data-ttu-id="b5987-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b5987-120">Type</span></span>|<span data-ttu-id="b5987-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b5987-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5987-122">id</span><span class="sxs-lookup"><span data-stu-id="b5987-122">id</span></span>|<span data-ttu-id="b5987-123">String</span><span class="sxs-lookup"><span data-stu-id="b5987-123">String</span></span>|<span data-ttu-id="b5987-124">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b5987-124">Key of the entity.</span></span>|
|<span data-ttu-id="b5987-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b5987-125">installedDeviceCount</span></span>|<span data-ttu-id="b5987-126">Int32</span><span class="sxs-lookup"><span data-stu-id="b5987-126">Int32</span></span>|<span data-ttu-id="b5987-127">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="b5987-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="b5987-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b5987-128">failedDeviceCount</span></span>|<span data-ttu-id="b5987-129">Int32</span><span class="sxs-lookup"><span data-stu-id="b5987-129">Int32</span></span>|<span data-ttu-id="b5987-130">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="b5987-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="b5987-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b5987-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="b5987-132">Int32</span><span class="sxs-lookup"><span data-stu-id="b5987-132">Int32</span></span>|<span data-ttu-id="b5987-133">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="b5987-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="b5987-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="b5987-134">installedUserCount</span></span>|<span data-ttu-id="b5987-135">Int32</span><span class="sxs-lookup"><span data-stu-id="b5987-135">Int32</span></span>|<span data-ttu-id="b5987-136">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="b5987-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="b5987-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="b5987-137">failedUserCount</span></span>|<span data-ttu-id="b5987-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b5987-138">Int32</span></span>|<span data-ttu-id="b5987-139">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="b5987-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="b5987-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="b5987-140">notInstalledUserCount</span></span>|<span data-ttu-id="b5987-141">Int32</span><span class="sxs-lookup"><span data-stu-id="b5987-141">Int32</span></span>|<span data-ttu-id="b5987-142">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="b5987-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5987-143">Связи</span><span class="sxs-lookup"><span data-stu-id="b5987-143">Relationships</span></span>
<span data-ttu-id="b5987-144">Нет</span><span class="sxs-lookup"><span data-stu-id="b5987-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5987-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5987-145">JSON Representation</span></span>
<span data-ttu-id="b5987-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5987-146">Here is a JSON representation of the resource.</span></span>
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




