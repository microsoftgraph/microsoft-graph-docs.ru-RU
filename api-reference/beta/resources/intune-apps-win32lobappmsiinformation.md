---
title: Тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f80e41eec3b2e6b494d076029a5408267da65595
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732659"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="c4e42-103">Тип ресурса win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="c4e42-103">win32LobAppMsiInformation resource type</span></span>

<span data-ttu-id="c4e42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4e42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4e42-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4e42-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4e42-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4e42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4e42-107">Содержит свойства приложения MSI для приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="c4e42-107">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="c4e42-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4e42-108">Properties</span></span>
|<span data-ttu-id="c4e42-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4e42-109">Property</span></span>|<span data-ttu-id="c4e42-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c4e42-110">Type</span></span>|<span data-ttu-id="c4e42-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c4e42-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4e42-112">productCode</span><span class="sxs-lookup"><span data-stu-id="c4e42-112">productCode</span></span>|<span data-ttu-id="c4e42-113">String</span><span class="sxs-lookup"><span data-stu-id="c4e42-113">String</span></span>|<span data-ttu-id="c4e42-114">Код продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="c4e42-114">The MSI product code.</span></span>|
|<span data-ttu-id="c4e42-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="c4e42-115">productVersion</span></span>|<span data-ttu-id="c4e42-116">String</span><span class="sxs-lookup"><span data-stu-id="c4e42-116">String</span></span>|<span data-ttu-id="c4e42-117">Версия продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="c4e42-117">The MSI product version.</span></span>|
|<span data-ttu-id="c4e42-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="c4e42-118">upgradeCode</span></span>|<span data-ttu-id="c4e42-119">Строка</span><span class="sxs-lookup"><span data-stu-id="c4e42-119">String</span></span>|<span data-ttu-id="c4e42-120">Код обновления MSI.</span><span class="sxs-lookup"><span data-stu-id="c4e42-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="c4e42-121">рекуиресребут</span><span class="sxs-lookup"><span data-stu-id="c4e42-121">requiresReboot</span></span>|<span data-ttu-id="c4e42-122">Логический</span><span class="sxs-lookup"><span data-stu-id="c4e42-122">Boolean</span></span>|<span data-ttu-id="c4e42-123">Требует ли приложение MSI перезагрузку компьютера для завершения установки.</span><span class="sxs-lookup"><span data-stu-id="c4e42-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="c4e42-124">паккажетипе</span><span class="sxs-lookup"><span data-stu-id="c4e42-124">packageType</span></span>|[<span data-ttu-id="c4e42-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="c4e42-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="c4e42-126">Тип пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="c4e42-126">The MSI package type.</span></span> <span data-ttu-id="c4e42-127">Возможные значения: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="c4e42-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="c4e42-128">productName</span><span class="sxs-lookup"><span data-stu-id="c4e42-128">productName</span></span>|<span data-ttu-id="c4e42-129">String</span><span class="sxs-lookup"><span data-stu-id="c4e42-129">String</span></span>|<span data-ttu-id="c4e42-130">Имя продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="c4e42-130">The MSI product name.</span></span>|
|<span data-ttu-id="c4e42-131">publisher</span><span class="sxs-lookup"><span data-stu-id="c4e42-131">publisher</span></span>|<span data-ttu-id="c4e42-132">String</span><span class="sxs-lookup"><span data-stu-id="c4e42-132">String</span></span>|<span data-ttu-id="c4e42-133">Издатель MSI.</span><span class="sxs-lookup"><span data-stu-id="c4e42-133">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4e42-134">Связи</span><span class="sxs-lookup"><span data-stu-id="c4e42-134">Relationships</span></span>
<span data-ttu-id="c4e42-135">Нет</span><span class="sxs-lookup"><span data-stu-id="c4e42-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4e42-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4e42-136">JSON Representation</span></span>
<span data-ttu-id="c4e42-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4e42-137">Here is a JSON representation of the resource.</span></span>
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





