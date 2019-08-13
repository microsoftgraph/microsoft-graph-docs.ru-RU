---
title: Тип ресурса Впптокенлиценсесуммари
description: Сводка по лицензии для определенного приложения в маркере.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f421da54543d74009cb921ec429e3795e31d8572
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375396"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="1e6bc-103">Тип ресурса Впптокенлиценсесуммари</span><span class="sxs-lookup"><span data-stu-id="1e6bc-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="1e6bc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e6bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e6bc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e6bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e6bc-106">Сводка по лицензии для определенного приложения в маркере.</span><span class="sxs-lookup"><span data-stu-id="1e6bc-106">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="1e6bc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e6bc-107">Properties</span></span>
|<span data-ttu-id="1e6bc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e6bc-108">Property</span></span>|<span data-ttu-id="1e6bc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1e6bc-109">Type</span></span>|<span data-ttu-id="1e6bc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1e6bc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e6bc-111">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="1e6bc-111">vppTokenId</span></span>|<span data-ttu-id="1e6bc-112">String</span><span class="sxs-lookup"><span data-stu-id="1e6bc-112">String</span></span>|<span data-ttu-id="1e6bc-113">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="1e6bc-113">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="1e6bc-114">appleId</span><span class="sxs-lookup"><span data-stu-id="1e6bc-114">appleId</span></span>|<span data-ttu-id="1e6bc-115">String</span><span class="sxs-lookup"><span data-stu-id="1e6bc-115">String</span></span>|<span data-ttu-id="1e6bc-116">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="1e6bc-116">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="1e6bc-117">organizationName</span><span class="sxs-lookup"><span data-stu-id="1e6bc-117">organizationName</span></span>|<span data-ttu-id="1e6bc-118">String</span><span class="sxs-lookup"><span data-stu-id="1e6bc-118">String</span></span>|<span data-ttu-id="1e6bc-119">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="1e6bc-119">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="1e6bc-120">аваилаблелиценсекаунт</span><span class="sxs-lookup"><span data-stu-id="1e6bc-120">availableLicenseCount</span></span>|<span data-ttu-id="1e6bc-121">Int32</span><span class="sxs-lookup"><span data-stu-id="1e6bc-121">Int32</span></span>|<span data-ttu-id="1e6bc-122">Число доступных лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="1e6bc-122">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="1e6bc-123">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1e6bc-123">usedLicenseCount</span></span>|<span data-ttu-id="1e6bc-124">Int32</span><span class="sxs-lookup"><span data-stu-id="1e6bc-124">Int32</span></span>|<span data-ttu-id="1e6bc-125">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="1e6bc-125">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e6bc-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="1e6bc-126">Relationships</span></span>
<span data-ttu-id="1e6bc-127">Нет</span><span class="sxs-lookup"><span data-stu-id="1e6bc-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e6bc-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e6bc-128">JSON Representation</span></span>
<span data-ttu-id="1e6bc-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e6bc-129">Here is a JSON representation of the resource.</span></span>
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



