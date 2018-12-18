---
title: Тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
author: tfitzmac
ms.openlocfilehash: 1753df68ab1f4b0e1649c16a4a7fa0ad49941bf9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326140"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="7d999-103">Тип ресурса win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="7d999-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="7d999-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7d999-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d999-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d999-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d999-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7d999-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d999-107">Содержит свойства приложения MSI для приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="7d999-107">Contains MSI app properties for a Win32 App.</span></span>
## <a name="properties"></a><span data-ttu-id="7d999-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7d999-108">Properties</span></span>
|<span data-ttu-id="7d999-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d999-109">Property</span></span>|<span data-ttu-id="7d999-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7d999-110">Type</span></span>|<span data-ttu-id="7d999-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7d999-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d999-112">productCode</span><span class="sxs-lookup"><span data-stu-id="7d999-112">productCode</span></span>|<span data-ttu-id="7d999-113">String</span><span class="sxs-lookup"><span data-stu-id="7d999-113">String</span></span>|<span data-ttu-id="7d999-114">Код продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="7d999-114">The MSI product code.</span></span>|
|<span data-ttu-id="7d999-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="7d999-115">productVersion</span></span>|<span data-ttu-id="7d999-116">String</span><span class="sxs-lookup"><span data-stu-id="7d999-116">String</span></span>|<span data-ttu-id="7d999-117">Версия продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="7d999-117">The MSI product version.</span></span>|
|<span data-ttu-id="7d999-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="7d999-118">upgradeCode</span></span>|<span data-ttu-id="7d999-119">String.</span><span class="sxs-lookup"><span data-stu-id="7d999-119">String</span></span>|<span data-ttu-id="7d999-120">Код обновления MSI.</span><span class="sxs-lookup"><span data-stu-id="7d999-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="7d999-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="7d999-121">requiresReboot</span></span>|<span data-ttu-id="7d999-122">Boolean.</span><span class="sxs-lookup"><span data-stu-id="7d999-122">Boolean</span></span>|<span data-ttu-id="7d999-123">Требуется ли приложение MSI для завершения установки перезагрузить компьютер.</span><span class="sxs-lookup"><span data-stu-id="7d999-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="7d999-124">Тип корпуса</span><span class="sxs-lookup"><span data-stu-id="7d999-124">packageType</span></span>|[<span data-ttu-id="7d999-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="7d999-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="7d999-126">Тип пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="7d999-126">The MSI package type.</span></span> <span data-ttu-id="7d999-127">Возможные значения: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="7d999-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d999-128">Связи</span><span class="sxs-lookup"><span data-stu-id="7d999-128">Relationships</span></span>
<span data-ttu-id="7d999-129">Нет</span><span class="sxs-lookup"><span data-stu-id="7d999-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7d999-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7d999-130">JSON Representation</span></span>
<span data-ttu-id="7d999-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d999-131">Here is a JSON representation of the resource.</span></span>
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





