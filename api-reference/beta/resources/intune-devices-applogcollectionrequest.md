---
title: тип ресурса appLogCollectionRequest
description: Объект AppLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 44284785c3dacbed31d6b88960af23b50b0d48f2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133439"
---
# <a name="applogcollectionrequest-resource-type"></a><span data-ttu-id="1d567-103">тип ресурса appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="1d567-103">appLogCollectionRequest resource type</span></span>

<span data-ttu-id="1d567-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d567-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d567-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d567-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d567-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d567-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d567-107">Объект AppLogCollectionRequest.</span><span class="sxs-lookup"><span data-stu-id="1d567-107">AppLogCollectionRequest Entity.</span></span>

## <a name="methods"></a><span data-ttu-id="1d567-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1d567-108">Methods</span></span>
|<span data-ttu-id="1d567-109">Метод</span><span class="sxs-lookup"><span data-stu-id="1d567-109">Method</span></span>|<span data-ttu-id="1d567-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1d567-110">Return Type</span></span>|<span data-ttu-id="1d567-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1d567-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1d567-112">Get appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="1d567-112">Get appLogCollectionRequest</span></span>](../api/intune-devices-applogcollectionrequest-get.md)|[<span data-ttu-id="1d567-113">appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="1d567-113">appLogCollectionRequest</span></span>](../resources/intune-devices-applogcollectionrequest.md)|<span data-ttu-id="1d567-114">Чтение свойств и связей объекта [appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)</span><span class="sxs-lookup"><span data-stu-id="1d567-114">Read properties and relationships of the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>|
|[<span data-ttu-id="1d567-115">Создание appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="1d567-115">Create appLogCollectionRequest</span></span>](../api/intune-devices-applogcollectionrequest-create.md)|[<span data-ttu-id="1d567-116">appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="1d567-116">appLogCollectionRequest</span></span>](../resources/intune-devices-applogcollectionrequest.md)|<span data-ttu-id="1d567-117">Создайте новый [объект appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)</span><span class="sxs-lookup"><span data-stu-id="1d567-117">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>|
|[<span data-ttu-id="1d567-118">Действие createDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="1d567-118">createDownloadUrl action</span></span>](../api/intune-devices-applogcollectionrequest-createdownloadurl.md)|[<span data-ttu-id="1d567-119">appLogCollectionDownloadDetails</span><span class="sxs-lookup"><span data-stu-id="1d567-119">appLogCollectionDownloadDetails</span></span>](../resources/intune-devices-applogcollectiondownloaddetails.md)|<span data-ttu-id="1d567-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1d567-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1d567-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d567-121">Properties</span></span>
|<span data-ttu-id="1d567-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d567-122">Property</span></span>|<span data-ttu-id="1d567-123">Тип</span><span class="sxs-lookup"><span data-stu-id="1d567-123">Type</span></span>|<span data-ttu-id="1d567-124">Описание</span><span class="sxs-lookup"><span data-stu-id="1d567-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d567-125">id</span><span class="sxs-lookup"><span data-stu-id="1d567-125">id</span></span>|<span data-ttu-id="1d567-126">Строка</span><span class="sxs-lookup"><span data-stu-id="1d567-126">String</span></span>|<span data-ttu-id="1d567-127">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="1d567-127">The unique Identifier.</span></span> <span data-ttu-id="1d567-128">Это userId_DeviceId_AppId id.</span><span class="sxs-lookup"><span data-stu-id="1d567-128">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="1d567-129">status</span><span class="sxs-lookup"><span data-stu-id="1d567-129">status</span></span>|[<span data-ttu-id="1d567-130">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="1d567-130">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="1d567-131">Состояние загрузки журнала.</span><span class="sxs-lookup"><span data-stu-id="1d567-131">Log upload status.</span></span> <span data-ttu-id="1d567-132">Возможные значения: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="1d567-132">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="1d567-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="1d567-133">errorMessage</span></span>|<span data-ttu-id="1d567-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1d567-134">String</span></span>|<span data-ttu-id="1d567-135">Сообщение об ошибке, если таково сообщение во время процесса загрузки</span><span class="sxs-lookup"><span data-stu-id="1d567-135">Error message if any during the upload process</span></span>|
|<span data-ttu-id="1d567-136">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="1d567-136">customLogFolders</span></span>|<span data-ttu-id="1d567-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1d567-137">String collection</span></span>|<span data-ttu-id="1d567-138">Список папок журнала.</span><span class="sxs-lookup"><span data-stu-id="1d567-138">List of log folders.</span></span> |
|<span data-ttu-id="1d567-139">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d567-139">completedDateTime</span></span>|<span data-ttu-id="1d567-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d567-140">DateTimeOffset</span></span>|<span data-ttu-id="1d567-141">Время, в течение которого запрос журнала загрузки достиг состояния терминала</span><span class="sxs-lookup"><span data-stu-id="1d567-141">Time at which the upload log request reached a terminal state</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d567-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="1d567-142">Relationships</span></span>
<span data-ttu-id="1d567-143">Нет</span><span class="sxs-lookup"><span data-stu-id="1d567-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d567-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d567-144">JSON Representation</span></span>
<span data-ttu-id="1d567-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d567-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appLogCollectionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "String (identifier)",
  "status": "String",
  "errorMessage": "String",
  "customLogFolders": [
    "String"
  ],
  "completedDateTime": "String (timestamp)"
}
```




