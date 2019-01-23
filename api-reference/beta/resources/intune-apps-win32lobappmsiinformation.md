---
title: Тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ba91c572286020a3e349527f325d22bf0be5d67
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399250"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="23f3e-103">Тип ресурса win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="23f3e-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="23f3e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="23f3e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="23f3e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23f3e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23f3e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23f3e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23f3e-107">Содержит свойства приложения MSI для приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="23f3e-107">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="23f3e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="23f3e-108">Properties</span></span>
|<span data-ttu-id="23f3e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="23f3e-109">Property</span></span>|<span data-ttu-id="23f3e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="23f3e-110">Type</span></span>|<span data-ttu-id="23f3e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="23f3e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23f3e-112">productCode</span><span class="sxs-lookup"><span data-stu-id="23f3e-112">productCode</span></span>|<span data-ttu-id="23f3e-113">String</span><span class="sxs-lookup"><span data-stu-id="23f3e-113">String</span></span>|<span data-ttu-id="23f3e-114">Код продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="23f3e-114">The MSI product code.</span></span>|
|<span data-ttu-id="23f3e-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="23f3e-115">productVersion</span></span>|<span data-ttu-id="23f3e-116">String</span><span class="sxs-lookup"><span data-stu-id="23f3e-116">String</span></span>|<span data-ttu-id="23f3e-117">Версия продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="23f3e-117">The MSI product version.</span></span>|
|<span data-ttu-id="23f3e-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="23f3e-118">upgradeCode</span></span>|<span data-ttu-id="23f3e-119">String</span><span class="sxs-lookup"><span data-stu-id="23f3e-119">String</span></span>|<span data-ttu-id="23f3e-120">Код обновления MSI.</span><span class="sxs-lookup"><span data-stu-id="23f3e-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="23f3e-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="23f3e-121">requiresReboot</span></span>|<span data-ttu-id="23f3e-122">Логический</span><span class="sxs-lookup"><span data-stu-id="23f3e-122">Boolean</span></span>|<span data-ttu-id="23f3e-123">Требуется ли приложение MSI для завершения установки перезагрузить компьютер.</span><span class="sxs-lookup"><span data-stu-id="23f3e-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="23f3e-124">Тип корпуса</span><span class="sxs-lookup"><span data-stu-id="23f3e-124">packageType</span></span>|[<span data-ttu-id="23f3e-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="23f3e-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="23f3e-126">Тип пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="23f3e-126">The MSI package type.</span></span> <span data-ttu-id="23f3e-127">Возможные значения: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="23f3e-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23f3e-128">Связи</span><span class="sxs-lookup"><span data-stu-id="23f3e-128">Relationships</span></span>
<span data-ttu-id="23f3e-129">Нет</span><span class="sxs-lookup"><span data-stu-id="23f3e-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23f3e-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23f3e-130">JSON Representation</span></span>
<span data-ttu-id="23f3e-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23f3e-131">Here is a JSON representation of the resource.</span></span>
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
  "packageType": "String"
}
```




