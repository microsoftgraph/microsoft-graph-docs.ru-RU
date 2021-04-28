---
title: тип ресурса featureUpdateCatalogEntry
description: Метаданные для обновления Windows 10, которое можно утвердить для развертывания.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 64ad4c2506a2d8f90276e50e7fe5288e1af1d8db
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067543"
---
# <a name="featureupdatecatalogentry-resource-type"></a><span data-ttu-id="12521-103">тип ресурса featureUpdateCatalogEntry</span><span class="sxs-lookup"><span data-stu-id="12521-103">featureUpdateCatalogEntry resource type</span></span>

<span data-ttu-id="12521-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="12521-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12521-105">Метаданные для обновления Windows 10, которое можно утвердить для развертывания.</span><span class="sxs-lookup"><span data-stu-id="12521-105">Metadata for a Windows 10 feature update that you can approve for deployment.</span></span>

<span data-ttu-id="12521-106">Windows 10 обновления компонентов выпускаются раз в два года и содержат новые функции для Windows 10.</span><span class="sxs-lookup"><span data-stu-id="12521-106">Windows 10 feature updates are released bi-annually and contain new features for Windows 10.</span></span> <span data-ttu-id="12521-107">Установка этих обновлений увеличивает Windows 10 сборки и, как правило, приводит к новому жизненному циклу обслуживания и концу даты службы.</span><span class="sxs-lookup"><span data-stu-id="12521-107">Installing these updates increases the Windows 10 build number and typically results in a new servicing lifecycle and end of service date.</span></span> <span data-ttu-id="12521-108">Корпорация Майкрософт рекомендует организациям регулярно развертывать новые обновления функций в рамках Windows в качестве службы.</span><span class="sxs-lookup"><span data-stu-id="12521-108">Microsoft recommends organizations regularly deploy new feature updates as part of adopting Windows as a service.</span></span>

<span data-ttu-id="12521-109">Наследует от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="12521-109">Inherits from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>

## <a name="properties"></a><span data-ttu-id="12521-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="12521-110">Properties</span></span>
|<span data-ttu-id="12521-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="12521-111">Property</span></span>|<span data-ttu-id="12521-112">Тип</span><span class="sxs-lookup"><span data-stu-id="12521-112">Type</span></span>|<span data-ttu-id="12521-113">Описание</span><span class="sxs-lookup"><span data-stu-id="12521-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12521-114">deployableUntilDateTime</span><span class="sxs-lookup"><span data-stu-id="12521-114">deployableUntilDateTime</span></span>|<span data-ttu-id="12521-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12521-115">DateTimeOffset</span></span>|<span data-ttu-id="12521-116">Дата, в которую контент больше не доступен для развертывания с помощью службы.</span><span class="sxs-lookup"><span data-stu-id="12521-116">The date on which the content is no longer available for deployment using the service.</span></span> <span data-ttu-id="12521-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12521-117">Read-only.</span></span> <span data-ttu-id="12521-118">Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="12521-118">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="12521-119">displayName</span><span class="sxs-lookup"><span data-stu-id="12521-119">displayName</span></span>|<span data-ttu-id="12521-120">String</span><span class="sxs-lookup"><span data-stu-id="12521-120">String</span></span>|<span data-ttu-id="12521-121">Отображение имени контента.</span><span class="sxs-lookup"><span data-stu-id="12521-121">The display name of the content.</span></span> <span data-ttu-id="12521-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12521-122">Read-only.</span></span> <span data-ttu-id="12521-123">Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="12521-123">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="12521-124">id</span><span class="sxs-lookup"><span data-stu-id="12521-124">id</span></span>|<span data-ttu-id="12521-125">String</span><span class="sxs-lookup"><span data-stu-id="12521-125">String</span></span>|<span data-ttu-id="12521-126">Уникальный идентификатор для записи каталога.</span><span class="sxs-lookup"><span data-stu-id="12521-126">The unique identifier for the catalog entry.</span></span> <span data-ttu-id="12521-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12521-127">Read-only.</span></span> <span data-ttu-id="12521-128">Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="12521-128">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="12521-129">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="12521-129">releaseDateTime</span></span>|<span data-ttu-id="12521-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12521-130">DateTimeOffset</span></span>|<span data-ttu-id="12521-131">Дата выпуска контента.</span><span class="sxs-lookup"><span data-stu-id="12521-131">The release date for the content.</span></span> <span data-ttu-id="12521-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12521-132">Read-only.</span></span> <span data-ttu-id="12521-133">Унаследовано от [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span><span class="sxs-lookup"><span data-stu-id="12521-133">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="12521-134">version</span><span class="sxs-lookup"><span data-stu-id="12521-134">version</span></span>|<span data-ttu-id="12521-135">String</span><span class="sxs-lookup"><span data-stu-id="12521-135">String</span></span>|<span data-ttu-id="12521-136">Версия обновления функции.</span><span class="sxs-lookup"><span data-stu-id="12521-136">The version of the feature update.</span></span> <span data-ttu-id="12521-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12521-137">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12521-138">Связи</span><span class="sxs-lookup"><span data-stu-id="12521-138">Relationships</span></span>
<span data-ttu-id="12521-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="12521-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="12521-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="12521-140">JSON representation</span></span>
<span data-ttu-id="12521-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12521-141">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.featureUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)",
  "version": "String"
}
```

