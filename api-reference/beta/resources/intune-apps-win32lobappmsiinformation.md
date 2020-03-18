---
title: Тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd710b166bd1171ed17a2deef7648e580d578301
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797642"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="ac10d-103">Тип ресурса win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="ac10d-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="ac10d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac10d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac10d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ac10d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac10d-106">Содержит свойства приложения MSI для приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="ac10d-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="ac10d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac10d-107">Properties</span></span>
|<span data-ttu-id="ac10d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac10d-108">Property</span></span>|<span data-ttu-id="ac10d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ac10d-109">Type</span></span>|<span data-ttu-id="ac10d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ac10d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac10d-111">productCode</span><span class="sxs-lookup"><span data-stu-id="ac10d-111">productCode</span></span>|<span data-ttu-id="ac10d-112">String</span><span class="sxs-lookup"><span data-stu-id="ac10d-112">String</span></span>|<span data-ttu-id="ac10d-113">Код продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="ac10d-113">The MSI product code.</span></span>|
|<span data-ttu-id="ac10d-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="ac10d-114">productVersion</span></span>|<span data-ttu-id="ac10d-115">String</span><span class="sxs-lookup"><span data-stu-id="ac10d-115">String</span></span>|<span data-ttu-id="ac10d-116">Версия продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="ac10d-116">The MSI product version.</span></span>|
|<span data-ttu-id="ac10d-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="ac10d-117">upgradeCode</span></span>|<span data-ttu-id="ac10d-118">String</span><span class="sxs-lookup"><span data-stu-id="ac10d-118">String</span></span>|<span data-ttu-id="ac10d-119">Код обновления MSI.</span><span class="sxs-lookup"><span data-stu-id="ac10d-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="ac10d-120">рекуиресребут</span><span class="sxs-lookup"><span data-stu-id="ac10d-120">requiresReboot</span></span>|<span data-ttu-id="ac10d-121">Логический</span><span class="sxs-lookup"><span data-stu-id="ac10d-121">Boolean</span></span>|<span data-ttu-id="ac10d-122">Требует ли приложение MSI перезагрузку компьютера для завершения установки.</span><span class="sxs-lookup"><span data-stu-id="ac10d-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="ac10d-123">паккажетипе</span><span class="sxs-lookup"><span data-stu-id="ac10d-123">packageType</span></span>|[<span data-ttu-id="ac10d-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="ac10d-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="ac10d-125">Тип пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="ac10d-125">The MSI package type.</span></span> <span data-ttu-id="ac10d-126">Возможные значения: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="ac10d-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="ac10d-127">productName</span><span class="sxs-lookup"><span data-stu-id="ac10d-127">productName</span></span>|<span data-ttu-id="ac10d-128">String</span><span class="sxs-lookup"><span data-stu-id="ac10d-128">String</span></span>|<span data-ttu-id="ac10d-129">Имя продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="ac10d-129">The MSI product name.</span></span>|
|<span data-ttu-id="ac10d-130">publisher</span><span class="sxs-lookup"><span data-stu-id="ac10d-130">publisher</span></span>|<span data-ttu-id="ac10d-131">String</span><span class="sxs-lookup"><span data-stu-id="ac10d-131">String</span></span>|<span data-ttu-id="ac10d-132">Издатель MSI.</span><span class="sxs-lookup"><span data-stu-id="ac10d-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac10d-133">Связи</span><span class="sxs-lookup"><span data-stu-id="ac10d-133">Relationships</span></span>
<span data-ttu-id="ac10d-134">Нет</span><span class="sxs-lookup"><span data-stu-id="ac10d-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac10d-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac10d-135">JSON Representation</span></span>
<span data-ttu-id="ac10d-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac10d-136">Here is a JSON representation of the resource.</span></span>
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



