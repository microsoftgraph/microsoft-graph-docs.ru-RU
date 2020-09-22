---
title: Тип ресурса Впптокенлиценсесуммари
description: Сводка по лицензии для определенного приложения в маркере.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7b206d4ca825f818390421dbce23ea618917336a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029374"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="8f4b3-103">Тип ресурса Впптокенлиценсесуммари</span><span class="sxs-lookup"><span data-stu-id="8f4b3-103">vppTokenLicenseSummary resource type</span></span>

<span data-ttu-id="8f4b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f4b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f4b3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f4b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f4b3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f4b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f4b3-107">Сводка по лицензии для определенного приложения в маркере.</span><span class="sxs-lookup"><span data-stu-id="8f4b3-107">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="8f4b3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f4b3-108">Properties</span></span>
|<span data-ttu-id="8f4b3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f4b3-109">Property</span></span>|<span data-ttu-id="8f4b3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8f4b3-110">Type</span></span>|<span data-ttu-id="8f4b3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8f4b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f4b3-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="8f4b3-112">vppTokenId</span></span>|<span data-ttu-id="8f4b3-113">String</span><span class="sxs-lookup"><span data-stu-id="8f4b3-113">String</span></span>|<span data-ttu-id="8f4b3-114">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="8f4b3-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="8f4b3-115">appleId</span><span class="sxs-lookup"><span data-stu-id="8f4b3-115">appleId</span></span>|<span data-ttu-id="8f4b3-116">String</span><span class="sxs-lookup"><span data-stu-id="8f4b3-116">String</span></span>|<span data-ttu-id="8f4b3-117">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="8f4b3-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="8f4b3-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="8f4b3-118">organizationName</span></span>|<span data-ttu-id="8f4b3-119">Строка</span><span class="sxs-lookup"><span data-stu-id="8f4b3-119">String</span></span>|<span data-ttu-id="8f4b3-120">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="8f4b3-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="8f4b3-121">аваилаблелиценсекаунт</span><span class="sxs-lookup"><span data-stu-id="8f4b3-121">availableLicenseCount</span></span>|<span data-ttu-id="8f4b3-122">Int32</span><span class="sxs-lookup"><span data-stu-id="8f4b3-122">Int32</span></span>|<span data-ttu-id="8f4b3-123">Число доступных лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="8f4b3-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="8f4b3-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="8f4b3-124">usedLicenseCount</span></span>|<span data-ttu-id="8f4b3-125">Int32</span><span class="sxs-lookup"><span data-stu-id="8f4b3-125">Int32</span></span>|<span data-ttu-id="8f4b3-126">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="8f4b3-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f4b3-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="8f4b3-127">Relationships</span></span>
<span data-ttu-id="8f4b3-128">Нет</span><span class="sxs-lookup"><span data-stu-id="8f4b3-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f4b3-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f4b3-129">JSON Representation</span></span>
<span data-ttu-id="8f4b3-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f4b3-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenLicenseSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenLicenseSummary",
  "vppTokenId": "String",
  "appleId": "String",
  "organizationName": "String",
  "availableLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```






