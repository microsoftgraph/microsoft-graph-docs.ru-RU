---
title: Тип ресурса Впптокенлиценсесуммари
description: Сводка по лицензии для определенного приложения в маркере.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20d7c24c887ca97f3a5a9890f5089b745130055e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777877"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="f1648-103">Тип ресурса Впптокенлиценсесуммари</span><span class="sxs-lookup"><span data-stu-id="f1648-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="f1648-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1648-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1648-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1648-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1648-106">Сводка по лицензии для определенного приложения в маркере.</span><span class="sxs-lookup"><span data-stu-id="f1648-106">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="f1648-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1648-107">Properties</span></span>
|<span data-ttu-id="f1648-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1648-108">Property</span></span>|<span data-ttu-id="f1648-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f1648-109">Type</span></span>|<span data-ttu-id="f1648-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f1648-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1648-111">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="f1648-111">vppTokenId</span></span>|<span data-ttu-id="f1648-112">String</span><span class="sxs-lookup"><span data-stu-id="f1648-112">String</span></span>|<span data-ttu-id="f1648-113">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="f1648-113">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="f1648-114">appleId</span><span class="sxs-lookup"><span data-stu-id="f1648-114">appleId</span></span>|<span data-ttu-id="f1648-115">String</span><span class="sxs-lookup"><span data-stu-id="f1648-115">String</span></span>|<span data-ttu-id="f1648-116">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="f1648-116">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f1648-117">organizationName</span><span class="sxs-lookup"><span data-stu-id="f1648-117">organizationName</span></span>|<span data-ttu-id="f1648-118">String</span><span class="sxs-lookup"><span data-stu-id="f1648-118">String</span></span>|<span data-ttu-id="f1648-119">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="f1648-119">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f1648-120">аваилаблелиценсекаунт</span><span class="sxs-lookup"><span data-stu-id="f1648-120">availableLicenseCount</span></span>|<span data-ttu-id="f1648-121">Int32</span><span class="sxs-lookup"><span data-stu-id="f1648-121">Int32</span></span>|<span data-ttu-id="f1648-122">Число доступных лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="f1648-122">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="f1648-123">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f1648-123">usedLicenseCount</span></span>|<span data-ttu-id="f1648-124">Int32</span><span class="sxs-lookup"><span data-stu-id="f1648-124">Int32</span></span>|<span data-ttu-id="f1648-125">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="f1648-125">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1648-126">Связи</span><span class="sxs-lookup"><span data-stu-id="f1648-126">Relationships</span></span>
<span data-ttu-id="f1648-127">Нет</span><span class="sxs-lookup"><span data-stu-id="f1648-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1648-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1648-128">JSON Representation</span></span>
<span data-ttu-id="f1648-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1648-129">Here is a JSON representation of the resource.</span></span>
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



