---
title: Тип ресурса Впптокенлиценсесуммари
description: Сводка по лицензии для определенного приложения в маркере.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2aa3da365f9c03d2d4b4ce5beace75e4a1b4f1bd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940164"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="0c0e9-103">Тип ресурса Впптокенлиценсесуммари</span><span class="sxs-lookup"><span data-stu-id="0c0e9-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="0c0e9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c0e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c0e9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c0e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c0e9-106">Сводка по лицензии для определенного приложения в маркере.</span><span class="sxs-lookup"><span data-stu-id="0c0e9-106">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="0c0e9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c0e9-107">Properties</span></span>
|<span data-ttu-id="0c0e9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c0e9-108">Property</span></span>|<span data-ttu-id="0c0e9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0c0e9-109">Type</span></span>|<span data-ttu-id="0c0e9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0c0e9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c0e9-111">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="0c0e9-111">vppTokenId</span></span>|<span data-ttu-id="0c0e9-112">Строка</span><span class="sxs-lookup"><span data-stu-id="0c0e9-112">String</span></span>|<span data-ttu-id="0c0e9-113">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="0c0e9-113">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="0c0e9-114">appleId</span><span class="sxs-lookup"><span data-stu-id="0c0e9-114">appleId</span></span>|<span data-ttu-id="0c0e9-115">String</span><span class="sxs-lookup"><span data-stu-id="0c0e9-115">String</span></span>|<span data-ttu-id="0c0e9-116">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="0c0e9-116">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="0c0e9-117">organizationName</span><span class="sxs-lookup"><span data-stu-id="0c0e9-117">organizationName</span></span>|<span data-ttu-id="0c0e9-118">Строка</span><span class="sxs-lookup"><span data-stu-id="0c0e9-118">String</span></span>|<span data-ttu-id="0c0e9-119">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="0c0e9-119">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="0c0e9-120">Аваилаблелиценсекаунт</span><span class="sxs-lookup"><span data-stu-id="0c0e9-120">availableLicenseCount</span></span>|<span data-ttu-id="0c0e9-121">Int32</span><span class="sxs-lookup"><span data-stu-id="0c0e9-121">Int32</span></span>|<span data-ttu-id="0c0e9-122">Число доступных лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="0c0e9-122">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="0c0e9-123">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="0c0e9-123">usedLicenseCount</span></span>|<span data-ttu-id="0c0e9-124">Int32</span><span class="sxs-lookup"><span data-stu-id="0c0e9-124">Int32</span></span>|<span data-ttu-id="0c0e9-125">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="0c0e9-125">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c0e9-126">Связи</span><span class="sxs-lookup"><span data-stu-id="0c0e9-126">Relationships</span></span>
<span data-ttu-id="0c0e9-127">Нет</span><span class="sxs-lookup"><span data-stu-id="0c0e9-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c0e9-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c0e9-128">JSON Representation</span></span>
<span data-ttu-id="0c0e9-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c0e9-129">Here is a JSON representation of the resource.</span></span>
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




