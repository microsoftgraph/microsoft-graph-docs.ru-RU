---
title: тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f9c610711f58a9d1929d0e708e127e2b337396f8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752198"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="51ece-103">тип ресурса win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="51ece-103">win32LobAppMsiInformation resource type</span></span>

<span data-ttu-id="51ece-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51ece-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51ece-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51ece-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51ece-106">Содержит свойства приложения MSI для приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="51ece-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="51ece-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="51ece-107">Properties</span></span>
|<span data-ttu-id="51ece-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="51ece-108">Property</span></span>|<span data-ttu-id="51ece-109">Тип</span><span class="sxs-lookup"><span data-stu-id="51ece-109">Type</span></span>|<span data-ttu-id="51ece-110">Описание</span><span class="sxs-lookup"><span data-stu-id="51ece-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51ece-111">productCode</span><span class="sxs-lookup"><span data-stu-id="51ece-111">productCode</span></span>|<span data-ttu-id="51ece-112">String</span><span class="sxs-lookup"><span data-stu-id="51ece-112">String</span></span>|<span data-ttu-id="51ece-113">Код продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="51ece-113">The MSI product code.</span></span>|
|<span data-ttu-id="51ece-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="51ece-114">productVersion</span></span>|<span data-ttu-id="51ece-115">String</span><span class="sxs-lookup"><span data-stu-id="51ece-115">String</span></span>|<span data-ttu-id="51ece-116">Версия продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="51ece-116">The MSI product version.</span></span>|
|<span data-ttu-id="51ece-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="51ece-117">upgradeCode</span></span>|<span data-ttu-id="51ece-118">String</span><span class="sxs-lookup"><span data-stu-id="51ece-118">String</span></span>|<span data-ttu-id="51ece-119">Код обновления MSI.</span><span class="sxs-lookup"><span data-stu-id="51ece-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="51ece-120">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="51ece-120">requiresReboot</span></span>|<span data-ttu-id="51ece-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="51ece-121">Boolean</span></span>|<span data-ttu-id="51ece-122">Требуется ли приложению MSI перезагрузить машину для завершения установки.</span><span class="sxs-lookup"><span data-stu-id="51ece-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="51ece-123">packageType</span><span class="sxs-lookup"><span data-stu-id="51ece-123">packageType</span></span>|[<span data-ttu-id="51ece-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="51ece-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="51ece-125">Тип пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="51ece-125">The MSI package type.</span></span> <span data-ttu-id="51ece-126">Возможные значения: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="51ece-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="51ece-127">productName</span><span class="sxs-lookup"><span data-stu-id="51ece-127">productName</span></span>|<span data-ttu-id="51ece-128">String</span><span class="sxs-lookup"><span data-stu-id="51ece-128">String</span></span>|<span data-ttu-id="51ece-129">Имя продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="51ece-129">The MSI product name.</span></span>|
|<span data-ttu-id="51ece-130">publisher</span><span class="sxs-lookup"><span data-stu-id="51ece-130">publisher</span></span>|<span data-ttu-id="51ece-131">String</span><span class="sxs-lookup"><span data-stu-id="51ece-131">String</span></span>|<span data-ttu-id="51ece-132">Издатель MSI.</span><span class="sxs-lookup"><span data-stu-id="51ece-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51ece-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="51ece-133">Relationships</span></span>
<span data-ttu-id="51ece-134">Нет</span><span class="sxs-lookup"><span data-stu-id="51ece-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51ece-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51ece-135">JSON Representation</span></span>
<span data-ttu-id="51ece-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51ece-136">Here is a JSON representation of the resource.</span></span>
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




