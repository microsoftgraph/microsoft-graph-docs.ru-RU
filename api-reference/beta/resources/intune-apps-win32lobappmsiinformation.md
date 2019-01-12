---
title: Тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 04972e9e7fa909c220fe55ca6337be3ac44138ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967877"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="addac-103">Тип ресурса win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="addac-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="addac-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="addac-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="addac-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="addac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="addac-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="addac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="addac-107">Содержит свойства приложения MSI для приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="addac-107">Contains MSI app properties for a Win32 App.</span></span>
## <a name="properties"></a><span data-ttu-id="addac-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="addac-108">Properties</span></span>
|<span data-ttu-id="addac-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="addac-109">Property</span></span>|<span data-ttu-id="addac-110">Тип</span><span class="sxs-lookup"><span data-stu-id="addac-110">Type</span></span>|<span data-ttu-id="addac-111">Описание</span><span class="sxs-lookup"><span data-stu-id="addac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="addac-112">productCode</span><span class="sxs-lookup"><span data-stu-id="addac-112">productCode</span></span>|<span data-ttu-id="addac-113">String</span><span class="sxs-lookup"><span data-stu-id="addac-113">String</span></span>|<span data-ttu-id="addac-114">Код продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="addac-114">The MSI product code.</span></span>|
|<span data-ttu-id="addac-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="addac-115">productVersion</span></span>|<span data-ttu-id="addac-116">String</span><span class="sxs-lookup"><span data-stu-id="addac-116">String</span></span>|<span data-ttu-id="addac-117">Версия продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="addac-117">The MSI product version.</span></span>|
|<span data-ttu-id="addac-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="addac-118">upgradeCode</span></span>|<span data-ttu-id="addac-119">Строка</span><span class="sxs-lookup"><span data-stu-id="addac-119">String</span></span>|<span data-ttu-id="addac-120">Код обновления MSI.</span><span class="sxs-lookup"><span data-stu-id="addac-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="addac-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="addac-121">requiresReboot</span></span>|<span data-ttu-id="addac-122">Логический</span><span class="sxs-lookup"><span data-stu-id="addac-122">Boolean</span></span>|<span data-ttu-id="addac-123">Требуется ли приложение MSI для завершения установки перезагрузить компьютер.</span><span class="sxs-lookup"><span data-stu-id="addac-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="addac-124">Тип корпуса</span><span class="sxs-lookup"><span data-stu-id="addac-124">packageType</span></span>|[<span data-ttu-id="addac-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="addac-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="addac-126">Тип пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="addac-126">The MSI package type.</span></span> <span data-ttu-id="addac-127">Возможные значения: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="addac-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="addac-128">Связи</span><span class="sxs-lookup"><span data-stu-id="addac-128">Relationships</span></span>
<span data-ttu-id="addac-129">Нет</span><span class="sxs-lookup"><span data-stu-id="addac-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="addac-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="addac-130">JSON Representation</span></span>
<span data-ttu-id="addac-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="addac-131">Here is a JSON representation of the resource.</span></span>
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





