---
title: Тип ресурса Впптокенлиценсесуммари
description: Сводка по лицензии для определенного приложения в маркере.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 47d56f27ac08d1b4ca657973cf6e5ae0690ba498
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527702"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="1259e-103">Тип ресурса Впптокенлиценсесуммари</span><span class="sxs-lookup"><span data-stu-id="1259e-103">vppTokenLicenseSummary resource type</span></span>

<span data-ttu-id="1259e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1259e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1259e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1259e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1259e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1259e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1259e-107">Сводка по лицензии для определенного приложения в маркере.</span><span class="sxs-lookup"><span data-stu-id="1259e-107">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="1259e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1259e-108">Properties</span></span>
|<span data-ttu-id="1259e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1259e-109">Property</span></span>|<span data-ttu-id="1259e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1259e-110">Type</span></span>|<span data-ttu-id="1259e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1259e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1259e-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="1259e-112">vppTokenId</span></span>|<span data-ttu-id="1259e-113">String</span><span class="sxs-lookup"><span data-stu-id="1259e-113">String</span></span>|<span data-ttu-id="1259e-114">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="1259e-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="1259e-115">appleId</span><span class="sxs-lookup"><span data-stu-id="1259e-115">appleId</span></span>|<span data-ttu-id="1259e-116">String</span><span class="sxs-lookup"><span data-stu-id="1259e-116">String</span></span>|<span data-ttu-id="1259e-117">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="1259e-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="1259e-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="1259e-118">organizationName</span></span>|<span data-ttu-id="1259e-119">String</span><span class="sxs-lookup"><span data-stu-id="1259e-119">String</span></span>|<span data-ttu-id="1259e-120">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="1259e-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="1259e-121">аваилаблелиценсекаунт</span><span class="sxs-lookup"><span data-stu-id="1259e-121">availableLicenseCount</span></span>|<span data-ttu-id="1259e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="1259e-122">Int32</span></span>|<span data-ttu-id="1259e-123">Число доступных лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="1259e-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="1259e-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1259e-124">usedLicenseCount</span></span>|<span data-ttu-id="1259e-125">Int32</span><span class="sxs-lookup"><span data-stu-id="1259e-125">Int32</span></span>|<span data-ttu-id="1259e-126">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="1259e-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1259e-127">Связи</span><span class="sxs-lookup"><span data-stu-id="1259e-127">Relationships</span></span>
<span data-ttu-id="1259e-128">Нет</span><span class="sxs-lookup"><span data-stu-id="1259e-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1259e-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1259e-129">JSON Representation</span></span>
<span data-ttu-id="1259e-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1259e-130">Here is a JSON representation of the resource.</span></span>
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



