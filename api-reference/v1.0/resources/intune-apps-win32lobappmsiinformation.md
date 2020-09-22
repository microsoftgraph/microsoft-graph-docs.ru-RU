---
title: Тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a812789a8231731b171edea8e15f7f540266cbde
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080166"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="50e3e-103">Тип ресурса win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="50e3e-103">win32LobAppMsiInformation resource type</span></span>

<span data-ttu-id="50e3e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50e3e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50e3e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50e3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50e3e-106">Содержит свойства приложения MSI для приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="50e3e-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="50e3e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="50e3e-107">Properties</span></span>
|<span data-ttu-id="50e3e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="50e3e-108">Property</span></span>|<span data-ttu-id="50e3e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="50e3e-109">Type</span></span>|<span data-ttu-id="50e3e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="50e3e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50e3e-111">productCode</span><span class="sxs-lookup"><span data-stu-id="50e3e-111">productCode</span></span>|<span data-ttu-id="50e3e-112">String</span><span class="sxs-lookup"><span data-stu-id="50e3e-112">String</span></span>|<span data-ttu-id="50e3e-113">Код продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="50e3e-113">The MSI product code.</span></span>|
|<span data-ttu-id="50e3e-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="50e3e-114">productVersion</span></span>|<span data-ttu-id="50e3e-115">String</span><span class="sxs-lookup"><span data-stu-id="50e3e-115">String</span></span>|<span data-ttu-id="50e3e-116">Версия продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="50e3e-116">The MSI product version.</span></span>|
|<span data-ttu-id="50e3e-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="50e3e-117">upgradeCode</span></span>|<span data-ttu-id="50e3e-118">Строка</span><span class="sxs-lookup"><span data-stu-id="50e3e-118">String</span></span>|<span data-ttu-id="50e3e-119">Код обновления MSI.</span><span class="sxs-lookup"><span data-stu-id="50e3e-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="50e3e-120">рекуиресребут</span><span class="sxs-lookup"><span data-stu-id="50e3e-120">requiresReboot</span></span>|<span data-ttu-id="50e3e-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="50e3e-121">Boolean</span></span>|<span data-ttu-id="50e3e-122">Требует ли приложение MSI перезагрузку компьютера для завершения установки.</span><span class="sxs-lookup"><span data-stu-id="50e3e-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="50e3e-123">паккажетипе</span><span class="sxs-lookup"><span data-stu-id="50e3e-123">packageType</span></span>|[<span data-ttu-id="50e3e-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="50e3e-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="50e3e-125">Тип пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="50e3e-125">The MSI package type.</span></span> <span data-ttu-id="50e3e-126">Возможные значения: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="50e3e-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="50e3e-127">productName</span><span class="sxs-lookup"><span data-stu-id="50e3e-127">productName</span></span>|<span data-ttu-id="50e3e-128">String</span><span class="sxs-lookup"><span data-stu-id="50e3e-128">String</span></span>|<span data-ttu-id="50e3e-129">Имя продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="50e3e-129">The MSI product name.</span></span>|
|<span data-ttu-id="50e3e-130">publisher</span><span class="sxs-lookup"><span data-stu-id="50e3e-130">publisher</span></span>|<span data-ttu-id="50e3e-131">String</span><span class="sxs-lookup"><span data-stu-id="50e3e-131">String</span></span>|<span data-ttu-id="50e3e-132">Издатель MSI.</span><span class="sxs-lookup"><span data-stu-id="50e3e-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50e3e-133">Связи</span><span class="sxs-lookup"><span data-stu-id="50e3e-133">Relationships</span></span>
<span data-ttu-id="50e3e-134">Нет</span><span class="sxs-lookup"><span data-stu-id="50e3e-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50e3e-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50e3e-135">JSON Representation</span></span>
<span data-ttu-id="50e3e-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50e3e-136">Here is a JSON representation of the resource.</span></span>
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





