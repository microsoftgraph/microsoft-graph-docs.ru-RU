---
title: Тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 151b0d756258b3c1b5911ab8719c3f72a6e7b263
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422968"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="05434-103">Тип ресурса win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="05434-103">win32LobAppMsiInformation resource type</span></span>

<span data-ttu-id="05434-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05434-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05434-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05434-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05434-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05434-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05434-107">Содержит свойства приложения MSI для приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="05434-107">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="05434-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="05434-108">Properties</span></span>
|<span data-ttu-id="05434-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="05434-109">Property</span></span>|<span data-ttu-id="05434-110">Тип</span><span class="sxs-lookup"><span data-stu-id="05434-110">Type</span></span>|<span data-ttu-id="05434-111">Описание</span><span class="sxs-lookup"><span data-stu-id="05434-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05434-112">productCode</span><span class="sxs-lookup"><span data-stu-id="05434-112">productCode</span></span>|<span data-ttu-id="05434-113">String</span><span class="sxs-lookup"><span data-stu-id="05434-113">String</span></span>|<span data-ttu-id="05434-114">Код продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="05434-114">The MSI product code.</span></span>|
|<span data-ttu-id="05434-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="05434-115">productVersion</span></span>|<span data-ttu-id="05434-116">String</span><span class="sxs-lookup"><span data-stu-id="05434-116">String</span></span>|<span data-ttu-id="05434-117">Версия продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="05434-117">The MSI product version.</span></span>|
|<span data-ttu-id="05434-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="05434-118">upgradeCode</span></span>|<span data-ttu-id="05434-119">String</span><span class="sxs-lookup"><span data-stu-id="05434-119">String</span></span>|<span data-ttu-id="05434-120">Код обновления MSI.</span><span class="sxs-lookup"><span data-stu-id="05434-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="05434-121">рекуиресребут</span><span class="sxs-lookup"><span data-stu-id="05434-121">requiresReboot</span></span>|<span data-ttu-id="05434-122">Логическое</span><span class="sxs-lookup"><span data-stu-id="05434-122">Boolean</span></span>|<span data-ttu-id="05434-123">Требует ли приложение MSI перезагрузку компьютера для завершения установки.</span><span class="sxs-lookup"><span data-stu-id="05434-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="05434-124">паккажетипе</span><span class="sxs-lookup"><span data-stu-id="05434-124">packageType</span></span>|[<span data-ttu-id="05434-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="05434-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="05434-126">Тип пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="05434-126">The MSI package type.</span></span> <span data-ttu-id="05434-127">Возможные значения: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="05434-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="05434-128">productName</span><span class="sxs-lookup"><span data-stu-id="05434-128">productName</span></span>|<span data-ttu-id="05434-129">String</span><span class="sxs-lookup"><span data-stu-id="05434-129">String</span></span>|<span data-ttu-id="05434-130">Имя продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="05434-130">The MSI product name.</span></span>|
|<span data-ttu-id="05434-131">publisher</span><span class="sxs-lookup"><span data-stu-id="05434-131">publisher</span></span>|<span data-ttu-id="05434-132">String</span><span class="sxs-lookup"><span data-stu-id="05434-132">String</span></span>|<span data-ttu-id="05434-133">Издатель MSI.</span><span class="sxs-lookup"><span data-stu-id="05434-133">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05434-134">Связи</span><span class="sxs-lookup"><span data-stu-id="05434-134">Relationships</span></span>
<span data-ttu-id="05434-135">Нет</span><span class="sxs-lookup"><span data-stu-id="05434-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05434-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05434-136">JSON Representation</span></span>
<span data-ttu-id="05434-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05434-137">Here is a JSON representation of the resource.</span></span>
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



