---
title: Тип ресурса win32LobAppMsiInformation
description: Содержит свойства приложения MSI для приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6fb872d970256a795c51570d68b3279fce43506f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274007"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="3397b-103">Тип ресурса win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="3397b-103">win32LobAppMsiInformation resource type</span></span>

<span data-ttu-id="3397b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3397b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3397b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3397b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3397b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3397b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3397b-107">Содержит свойства приложения MSI для приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="3397b-107">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="3397b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3397b-108">Properties</span></span>
|<span data-ttu-id="3397b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3397b-109">Property</span></span>|<span data-ttu-id="3397b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3397b-110">Type</span></span>|<span data-ttu-id="3397b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3397b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3397b-112">productCode</span><span class="sxs-lookup"><span data-stu-id="3397b-112">productCode</span></span>|<span data-ttu-id="3397b-113">String</span><span class="sxs-lookup"><span data-stu-id="3397b-113">String</span></span>|<span data-ttu-id="3397b-114">Код продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="3397b-114">The MSI product code.</span></span>|
|<span data-ttu-id="3397b-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="3397b-115">productVersion</span></span>|<span data-ttu-id="3397b-116">String</span><span class="sxs-lookup"><span data-stu-id="3397b-116">String</span></span>|<span data-ttu-id="3397b-117">Версия продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="3397b-117">The MSI product version.</span></span>|
|<span data-ttu-id="3397b-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="3397b-118">upgradeCode</span></span>|<span data-ttu-id="3397b-119">String</span><span class="sxs-lookup"><span data-stu-id="3397b-119">String</span></span>|<span data-ttu-id="3397b-120">Код обновления MSI.</span><span class="sxs-lookup"><span data-stu-id="3397b-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="3397b-121">рекуиресребут</span><span class="sxs-lookup"><span data-stu-id="3397b-121">requiresReboot</span></span>|<span data-ttu-id="3397b-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="3397b-122">Boolean</span></span>|<span data-ttu-id="3397b-123">Требует ли приложение MSI перезагрузку компьютера для завершения установки.</span><span class="sxs-lookup"><span data-stu-id="3397b-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="3397b-124">паккажетипе</span><span class="sxs-lookup"><span data-stu-id="3397b-124">packageType</span></span>|[<span data-ttu-id="3397b-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="3397b-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="3397b-126">Тип пакета MSI.</span><span class="sxs-lookup"><span data-stu-id="3397b-126">The MSI package type.</span></span> <span data-ttu-id="3397b-127">Возможные значения: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="3397b-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="3397b-128">productName</span><span class="sxs-lookup"><span data-stu-id="3397b-128">productName</span></span>|<span data-ttu-id="3397b-129">String</span><span class="sxs-lookup"><span data-stu-id="3397b-129">String</span></span>|<span data-ttu-id="3397b-130">Имя продукта MSI.</span><span class="sxs-lookup"><span data-stu-id="3397b-130">The MSI product name.</span></span>|
|<span data-ttu-id="3397b-131">publisher</span><span class="sxs-lookup"><span data-stu-id="3397b-131">publisher</span></span>|<span data-ttu-id="3397b-132">String</span><span class="sxs-lookup"><span data-stu-id="3397b-132">String</span></span>|<span data-ttu-id="3397b-133">Издатель MSI.</span><span class="sxs-lookup"><span data-stu-id="3397b-133">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3397b-134">Связи</span><span class="sxs-lookup"><span data-stu-id="3397b-134">Relationships</span></span>
<span data-ttu-id="3397b-135">Нет</span><span class="sxs-lookup"><span data-stu-id="3397b-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3397b-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3397b-136">JSON Representation</span></span>
<span data-ttu-id="3397b-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3397b-137">Here is a JSON representation of the resource.</span></span>
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




