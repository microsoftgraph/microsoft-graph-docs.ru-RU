---
title: Тип ресурса Девицеманажементтраублешутинжеррордетаилс
description: Объект, содержащий подробные сведения об ошибке и ее исправлении.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a50c749e6c6c6ddd59705bbea34f0bbd2488f9a4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939786"
---
# <a name="devicemanagementtroubleshootingerrordetails-resource-type"></a><span data-ttu-id="bd4ff-103">Тип ресурса Девицеманажементтраублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="bd4ff-103">deviceManagementTroubleshootingErrorDetails resource type</span></span>

> <span data-ttu-id="bd4ff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd4ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd4ff-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd4ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd4ff-106">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="bd4ff-106">Object containing detailed information about the error and its remediation.</span></span>

## <a name="properties"></a><span data-ttu-id="bd4ff-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd4ff-107">Properties</span></span>
|<span data-ttu-id="bd4ff-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd4ff-108">Property</span></span>|<span data-ttu-id="bd4ff-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bd4ff-109">Type</span></span>|<span data-ttu-id="bd4ff-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bd4ff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd4ff-111">контекст</span><span class="sxs-lookup"><span data-stu-id="bd4ff-111">context</span></span>|<span data-ttu-id="bd4ff-112">String</span><span class="sxs-lookup"><span data-stu-id="bd4ff-112">String</span></span>|<span data-ttu-id="bd4ff-113">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="bd4ff-113">Not yet documented</span></span>|
|<span data-ttu-id="bd4ff-114">Failure</span><span class="sxs-lookup"><span data-stu-id="bd4ff-114">failure</span></span>|<span data-ttu-id="bd4ff-115">String</span><span class="sxs-lookup"><span data-stu-id="bd4ff-115">String</span></span>|<span data-ttu-id="bd4ff-116">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="bd4ff-116">Not yet documented</span></span>|
|<span data-ttu-id="bd4ff-117">Фаилуредетаилс</span><span class="sxs-lookup"><span data-stu-id="bd4ff-117">failureDetails</span></span>|<span data-ttu-id="bd4ff-118">Строка</span><span class="sxs-lookup"><span data-stu-id="bd4ff-118">String</span></span>|<span data-ttu-id="bd4ff-119">Подробное описание того, что пошло не так.</span><span class="sxs-lookup"><span data-stu-id="bd4ff-119">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="bd4ff-120">исправления</span><span class="sxs-lookup"><span data-stu-id="bd4ff-120">remediation</span></span>|<span data-ttu-id="bd4ff-121">Строка</span><span class="sxs-lookup"><span data-stu-id="bd4ff-121">String</span></span>|<span data-ttu-id="bd4ff-122">Подробное описание этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="bd4ff-122">The detailed description of how to remediate this issue.</span></span>|
|<span data-ttu-id="bd4ff-123">resources</span><span class="sxs-lookup"><span data-stu-id="bd4ff-123">resources</span></span>|<span data-ttu-id="bd4ff-124">Коллекция [девицеманажементтраублешутинжеррорресаурце](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md)</span><span class="sxs-lookup"><span data-stu-id="bd4ff-124">[deviceManagementTroubleshootingErrorResource](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource.md) collection</span></span>|<span data-ttu-id="bd4ff-125">Ссылки на полезную документацию об этой ошибке.</span><span class="sxs-lookup"><span data-stu-id="bd4ff-125">Links to helpful documentation about this failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd4ff-126">Связи</span><span class="sxs-lookup"><span data-stu-id="bd4ff-126">Relationships</span></span>
<span data-ttu-id="bd4ff-127">Нет</span><span class="sxs-lookup"><span data-stu-id="bd4ff-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd4ff-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd4ff-128">JSON Representation</span></span>
<span data-ttu-id="bd4ff-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd4ff-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorDetails",
  "context": "String",
  "failure": "String",
  "failureDetails": "String",
  "remediation": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
      "text": "String",
      "link": "String"
    }
  ]
}
```




