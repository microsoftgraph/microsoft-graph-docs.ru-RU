---
title: Тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd612a5593ef151d4f324f3058c793ce7cd29bf0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949635"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="76680-103">Тип ресурса win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="76680-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="76680-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76680-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76680-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76680-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76680-106">Содержит свойства приложения MSI для приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="76680-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="76680-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="76680-107">Properties</span></span>
|<span data-ttu-id="76680-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="76680-108">Property</span></span>|<span data-ttu-id="76680-109">Тип</span><span class="sxs-lookup"><span data-stu-id="76680-109">Type</span></span>|<span data-ttu-id="76680-110">Описание</span><span class="sxs-lookup"><span data-stu-id="76680-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76680-111">productCode</span><span class="sxs-lookup"><span data-stu-id="76680-111">productCode</span></span>|<span data-ttu-id="76680-112">Строка</span><span class="sxs-lookup"><span data-stu-id="76680-112">String</span></span>|<span data-ttu-id="76680-113">Код продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="76680-113">The MSI product code.</span></span>|
|<span data-ttu-id="76680-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="76680-114">productVersion</span></span>|<span data-ttu-id="76680-115">Строка</span><span class="sxs-lookup"><span data-stu-id="76680-115">String</span></span>|<span data-ttu-id="76680-116">Версия продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="76680-116">The MSI product version.</span></span>|
|<span data-ttu-id="76680-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="76680-117">upgradeCode</span></span>|<span data-ttu-id="76680-118">Строка</span><span class="sxs-lookup"><span data-stu-id="76680-118">String</span></span>|<span data-ttu-id="76680-119">Код обновления MSI.</span><span class="sxs-lookup"><span data-stu-id="76680-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="76680-120">Рекуиресребут</span><span class="sxs-lookup"><span data-stu-id="76680-120">requiresReboot</span></span>|<span data-ttu-id="76680-121">Логический</span><span class="sxs-lookup"><span data-stu-id="76680-121">Boolean</span></span>|<span data-ttu-id="76680-122">Требует ли приложение MSI перезагрузку компьютера для завершения установки.</span><span class="sxs-lookup"><span data-stu-id="76680-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="76680-123">Паккажетипе</span><span class="sxs-lookup"><span data-stu-id="76680-123">packageType</span></span>|[<span data-ttu-id="76680-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="76680-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="76680-125">Тип пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="76680-125">The MSI package type.</span></span> <span data-ttu-id="76680-126">Возможные значения: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="76680-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="76680-127">productName</span><span class="sxs-lookup"><span data-stu-id="76680-127">productName</span></span>|<span data-ttu-id="76680-128">String</span><span class="sxs-lookup"><span data-stu-id="76680-128">String</span></span>|<span data-ttu-id="76680-129">Имя продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="76680-129">The MSI product name.</span></span>|
|<span data-ttu-id="76680-130">publisher</span><span class="sxs-lookup"><span data-stu-id="76680-130">publisher</span></span>|<span data-ttu-id="76680-131">Строка</span><span class="sxs-lookup"><span data-stu-id="76680-131">String</span></span>|<span data-ttu-id="76680-132">Издатель MSI.</span><span class="sxs-lookup"><span data-stu-id="76680-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76680-133">Связи</span><span class="sxs-lookup"><span data-stu-id="76680-133">Relationships</span></span>
<span data-ttu-id="76680-134">Нет</span><span class="sxs-lookup"><span data-stu-id="76680-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76680-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76680-135">JSON Representation</span></span>
<span data-ttu-id="76680-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76680-136">Here is a JSON representation of the resource.</span></span>
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




