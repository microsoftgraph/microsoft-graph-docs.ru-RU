---
title: Тип ресурса eBookInstallSummary
description: Содержит свойства сводки по установке книги для устройства.
author: tfitzmac
ms.openlocfilehash: 631ebbcc704072051f5c9a954040de4cc94a2c48
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307814"
---
# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="69bf1-103">Тип ресурса eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="69bf1-103">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="69bf1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="69bf1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69bf1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69bf1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69bf1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="69bf1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69bf1-107">Содержит свойства сводки по установке книги для устройства.</span><span class="sxs-lookup"><span data-stu-id="69bf1-107">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="69bf1-108">Методы</span><span class="sxs-lookup"><span data-stu-id="69bf1-108">Methods</span></span>
|<span data-ttu-id="69bf1-109">Метод</span><span class="sxs-lookup"><span data-stu-id="69bf1-109">Method</span></span>|<span data-ttu-id="69bf1-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="69bf1-110">Return Type</span></span>|<span data-ttu-id="69bf1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="69bf1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="69bf1-112">Получение объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="69bf1-112">Get eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-get.md)|[<span data-ttu-id="69bf1-113">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="69bf1-113">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="69bf1-114">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="69bf1-114">Read properties and relationships of the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="69bf1-115">Обновление объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="69bf1-115">Update eBookInstallSummary</span></span>](../api/intune-books-ebookinstallsummary-update.md)|[<span data-ttu-id="69bf1-116">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="69bf1-116">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="69bf1-117">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="69bf1-117">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="69bf1-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="69bf1-118">Properties</span></span>
|<span data-ttu-id="69bf1-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="69bf1-119">Property</span></span>|<span data-ttu-id="69bf1-120">Тип</span><span class="sxs-lookup"><span data-stu-id="69bf1-120">Type</span></span>|<span data-ttu-id="69bf1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="69bf1-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69bf1-122">id</span><span class="sxs-lookup"><span data-stu-id="69bf1-122">id</span></span>|<span data-ttu-id="69bf1-123">Строка</span><span class="sxs-lookup"><span data-stu-id="69bf1-123">String</span></span>|<span data-ttu-id="69bf1-124">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="69bf1-124">Key of the entity.</span></span>|
|<span data-ttu-id="69bf1-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69bf1-125">installedDeviceCount</span></span>|<span data-ttu-id="69bf1-126">Int32</span><span class="sxs-lookup"><span data-stu-id="69bf1-126">Int32</span></span>|<span data-ttu-id="69bf1-127">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="69bf1-127">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="69bf1-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69bf1-128">failedDeviceCount</span></span>|<span data-ttu-id="69bf1-129">Int32</span><span class="sxs-lookup"><span data-stu-id="69bf1-129">Int32</span></span>|<span data-ttu-id="69bf1-130">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="69bf1-130">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="69bf1-131">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="69bf1-131">notInstalledDeviceCount</span></span>|<span data-ttu-id="69bf1-132">Int32</span><span class="sxs-lookup"><span data-stu-id="69bf1-132">Int32</span></span>|<span data-ttu-id="69bf1-133">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="69bf1-133">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="69bf1-134">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="69bf1-134">installedUserCount</span></span>|<span data-ttu-id="69bf1-135">Int32</span><span class="sxs-lookup"><span data-stu-id="69bf1-135">Int32</span></span>|<span data-ttu-id="69bf1-136">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="69bf1-136">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="69bf1-137">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="69bf1-137">failedUserCount</span></span>|<span data-ttu-id="69bf1-138">Int32</span><span class="sxs-lookup"><span data-stu-id="69bf1-138">Int32</span></span>|<span data-ttu-id="69bf1-139">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="69bf1-139">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="69bf1-140">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="69bf1-140">notInstalledUserCount</span></span>|<span data-ttu-id="69bf1-141">Int32</span><span class="sxs-lookup"><span data-stu-id="69bf1-141">Int32</span></span>|<span data-ttu-id="69bf1-142">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="69bf1-142">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69bf1-143">Связи</span><span class="sxs-lookup"><span data-stu-id="69bf1-143">Relationships</span></span>
<span data-ttu-id="69bf1-144">Нет</span><span class="sxs-lookup"><span data-stu-id="69bf1-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="69bf1-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69bf1-145">JSON Representation</span></span>
<span data-ttu-id="69bf1-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69bf1-146">Here is a JSON representation of the resource.</span></span>
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





