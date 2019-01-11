---
title: Тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e43b3dc9e46ed193b7547a7ce85863253445d30c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846517"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="c63a2-103">Тип ресурса win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="c63a2-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="c63a2-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c63a2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c63a2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c63a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c63a2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c63a2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c63a2-107">Содержит свойства приложения MSI для приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="c63a2-107">Contains MSI app properties for a Win32 App.</span></span>
## <a name="properties"></a><span data-ttu-id="c63a2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c63a2-108">Properties</span></span>
|<span data-ttu-id="c63a2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c63a2-109">Property</span></span>|<span data-ttu-id="c63a2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c63a2-110">Type</span></span>|<span data-ttu-id="c63a2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c63a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c63a2-112">productCode</span><span class="sxs-lookup"><span data-stu-id="c63a2-112">productCode</span></span>|<span data-ttu-id="c63a2-113">String</span><span class="sxs-lookup"><span data-stu-id="c63a2-113">String</span></span>|<span data-ttu-id="c63a2-114">Код продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="c63a2-114">The MSI product code.</span></span>|
|<span data-ttu-id="c63a2-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="c63a2-115">productVersion</span></span>|<span data-ttu-id="c63a2-116">String</span><span class="sxs-lookup"><span data-stu-id="c63a2-116">String</span></span>|<span data-ttu-id="c63a2-117">Версия продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="c63a2-117">The MSI product version.</span></span>|
|<span data-ttu-id="c63a2-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="c63a2-118">upgradeCode</span></span>|<span data-ttu-id="c63a2-119">Строка</span><span class="sxs-lookup"><span data-stu-id="c63a2-119">String</span></span>|<span data-ttu-id="c63a2-120">Код обновления MSI.</span><span class="sxs-lookup"><span data-stu-id="c63a2-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="c63a2-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="c63a2-121">requiresReboot</span></span>|<span data-ttu-id="c63a2-122">Логический</span><span class="sxs-lookup"><span data-stu-id="c63a2-122">Boolean</span></span>|<span data-ttu-id="c63a2-123">Требуется ли приложение MSI для завершения установки перезагрузить компьютер.</span><span class="sxs-lookup"><span data-stu-id="c63a2-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="c63a2-124">Тип корпуса</span><span class="sxs-lookup"><span data-stu-id="c63a2-124">packageType</span></span>|[<span data-ttu-id="c63a2-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="c63a2-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="c63a2-126">Тип пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="c63a2-126">The MSI package type.</span></span> <span data-ttu-id="c63a2-127">Возможные значения: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="c63a2-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c63a2-128">Связи</span><span class="sxs-lookup"><span data-stu-id="c63a2-128">Relationships</span></span>
<span data-ttu-id="c63a2-129">Нет</span><span class="sxs-lookup"><span data-stu-id="c63a2-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c63a2-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c63a2-130">JSON Representation</span></span>
<span data-ttu-id="c63a2-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c63a2-131">Here is a JSON representation of the resource.</span></span>
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





