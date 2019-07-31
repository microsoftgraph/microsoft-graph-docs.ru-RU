---
title: Тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d993306cdd5f6c69d373669ed83fab6f986497df
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971657"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="d7c95-103">Тип ресурса win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="d7c95-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="d7c95-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7c95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7c95-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7c95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7c95-106">Содержит свойства приложения MSI для приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="d7c95-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="d7c95-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7c95-107">Properties</span></span>
|<span data-ttu-id="d7c95-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7c95-108">Property</span></span>|<span data-ttu-id="d7c95-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d7c95-109">Type</span></span>|<span data-ttu-id="d7c95-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d7c95-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7c95-111">productCode</span><span class="sxs-lookup"><span data-stu-id="d7c95-111">productCode</span></span>|<span data-ttu-id="d7c95-112">String</span><span class="sxs-lookup"><span data-stu-id="d7c95-112">String</span></span>|<span data-ttu-id="d7c95-113">Код продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="d7c95-113">The MSI product code.</span></span>|
|<span data-ttu-id="d7c95-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="d7c95-114">productVersion</span></span>|<span data-ttu-id="d7c95-115">String</span><span class="sxs-lookup"><span data-stu-id="d7c95-115">String</span></span>|<span data-ttu-id="d7c95-116">Версия продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="d7c95-116">The MSI product version.</span></span>|
|<span data-ttu-id="d7c95-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="d7c95-117">upgradeCode</span></span>|<span data-ttu-id="d7c95-118">String</span><span class="sxs-lookup"><span data-stu-id="d7c95-118">String</span></span>|<span data-ttu-id="d7c95-119">Код обновления MSI.</span><span class="sxs-lookup"><span data-stu-id="d7c95-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="d7c95-120">Рекуиресребут</span><span class="sxs-lookup"><span data-stu-id="d7c95-120">requiresReboot</span></span>|<span data-ttu-id="d7c95-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7c95-121">Boolean</span></span>|<span data-ttu-id="d7c95-122">Требует ли приложение MSI перезагрузку компьютера для завершения установки.</span><span class="sxs-lookup"><span data-stu-id="d7c95-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="d7c95-123">Паккажетипе</span><span class="sxs-lookup"><span data-stu-id="d7c95-123">packageType</span></span>|[<span data-ttu-id="d7c95-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="d7c95-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="d7c95-125">Тип пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="d7c95-125">The MSI package type.</span></span> <span data-ttu-id="d7c95-126">Возможные значения: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="d7c95-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="d7c95-127">productName</span><span class="sxs-lookup"><span data-stu-id="d7c95-127">productName</span></span>|<span data-ttu-id="d7c95-128">String</span><span class="sxs-lookup"><span data-stu-id="d7c95-128">String</span></span>|<span data-ttu-id="d7c95-129">Имя продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="d7c95-129">The MSI product name.</span></span>|
|<span data-ttu-id="d7c95-130">publisher</span><span class="sxs-lookup"><span data-stu-id="d7c95-130">publisher</span></span>|<span data-ttu-id="d7c95-131">String</span><span class="sxs-lookup"><span data-stu-id="d7c95-131">String</span></span>|<span data-ttu-id="d7c95-132">Издатель MSI.</span><span class="sxs-lookup"><span data-stu-id="d7c95-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7c95-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="d7c95-133">Relationships</span></span>
<span data-ttu-id="d7c95-134">Нет</span><span class="sxs-lookup"><span data-stu-id="d7c95-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7c95-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7c95-135">JSON Representation</span></span>
<span data-ttu-id="d7c95-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7c95-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppMsiInformation",
  "productCode": "String",
  "productVersion": "String",
  "upgradeCode": "String",
  "requiresReboot": true,
  "packageType": "String",
  "productName": "String",
  "publisher": "String"
}
```





