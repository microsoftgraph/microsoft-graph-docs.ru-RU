---
title: Тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 92ff70c8b1bbf63ce6fd81321282a0f61f4accc3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490695"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="2b7c7-103">Тип ресурса win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="2b7c7-103">win32LobAppMsiInformation resource type</span></span>

<span data-ttu-id="2b7c7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2b7c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b7c7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b7c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b7c7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b7c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b7c7-107">Содержит свойства приложения MSI для приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="2b7c7-107">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="2b7c7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b7c7-108">Properties</span></span>
|<span data-ttu-id="2b7c7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b7c7-109">Property</span></span>|<span data-ttu-id="2b7c7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2b7c7-110">Type</span></span>|<span data-ttu-id="2b7c7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2b7c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b7c7-112">productCode</span><span class="sxs-lookup"><span data-stu-id="2b7c7-112">productCode</span></span>|<span data-ttu-id="2b7c7-113">String</span><span class="sxs-lookup"><span data-stu-id="2b7c7-113">String</span></span>|<span data-ttu-id="2b7c7-114">Код продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="2b7c7-114">The MSI product code.</span></span>|
|<span data-ttu-id="2b7c7-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="2b7c7-115">productVersion</span></span>|<span data-ttu-id="2b7c7-116">String</span><span class="sxs-lookup"><span data-stu-id="2b7c7-116">String</span></span>|<span data-ttu-id="2b7c7-117">Версия продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="2b7c7-117">The MSI product version.</span></span>|
|<span data-ttu-id="2b7c7-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="2b7c7-118">upgradeCode</span></span>|<span data-ttu-id="2b7c7-119">String</span><span class="sxs-lookup"><span data-stu-id="2b7c7-119">String</span></span>|<span data-ttu-id="2b7c7-120">Код обновления MSI.</span><span class="sxs-lookup"><span data-stu-id="2b7c7-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="2b7c7-121">рекуиресребут</span><span class="sxs-lookup"><span data-stu-id="2b7c7-121">requiresReboot</span></span>|<span data-ttu-id="2b7c7-122">Логический</span><span class="sxs-lookup"><span data-stu-id="2b7c7-122">Boolean</span></span>|<span data-ttu-id="2b7c7-123">Требует ли приложение MSI перезагрузку компьютера для завершения установки.</span><span class="sxs-lookup"><span data-stu-id="2b7c7-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="2b7c7-124">паккажетипе</span><span class="sxs-lookup"><span data-stu-id="2b7c7-124">packageType</span></span>|[<span data-ttu-id="2b7c7-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="2b7c7-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="2b7c7-126">Тип пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="2b7c7-126">The MSI package type.</span></span> <span data-ttu-id="2b7c7-127">Возможные значения: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="2b7c7-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="2b7c7-128">productName</span><span class="sxs-lookup"><span data-stu-id="2b7c7-128">productName</span></span>|<span data-ttu-id="2b7c7-129">String</span><span class="sxs-lookup"><span data-stu-id="2b7c7-129">String</span></span>|<span data-ttu-id="2b7c7-130">Имя продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="2b7c7-130">The MSI product name.</span></span>|
|<span data-ttu-id="2b7c7-131">publisher</span><span class="sxs-lookup"><span data-stu-id="2b7c7-131">publisher</span></span>|<span data-ttu-id="2b7c7-132">String</span><span class="sxs-lookup"><span data-stu-id="2b7c7-132">String</span></span>|<span data-ttu-id="2b7c7-133">Издатель MSI.</span><span class="sxs-lookup"><span data-stu-id="2b7c7-133">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b7c7-134">Связи</span><span class="sxs-lookup"><span data-stu-id="2b7c7-134">Relationships</span></span>
<span data-ttu-id="2b7c7-135">Нет</span><span class="sxs-lookup"><span data-stu-id="2b7c7-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b7c7-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b7c7-136">JSON Representation</span></span>
<span data-ttu-id="2b7c7-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b7c7-137">Here is a JSON representation of the resource.</span></span>
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



