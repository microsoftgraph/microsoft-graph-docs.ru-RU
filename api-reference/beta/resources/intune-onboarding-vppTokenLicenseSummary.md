---
title: Тип ресурса Впптокенлиценсесуммари
description: Сводка по лицензии для определенного приложения в маркере.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1292caa41a2e56c42adde8be7f9bb8988b369cd7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566411"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="00ac5-103">Тип ресурса Впптокенлиценсесуммари</span><span class="sxs-lookup"><span data-stu-id="00ac5-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="00ac5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00ac5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00ac5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00ac5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00ac5-106">Сводка по лицензии для определенного приложения в маркере.</span><span class="sxs-lookup"><span data-stu-id="00ac5-106">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="00ac5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="00ac5-107">Properties</span></span>
|<span data-ttu-id="00ac5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="00ac5-108">Property</span></span>|<span data-ttu-id="00ac5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="00ac5-109">Type</span></span>|<span data-ttu-id="00ac5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="00ac5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00ac5-111">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="00ac5-111">vppTokenId</span></span>|<span data-ttu-id="00ac5-112">String</span><span class="sxs-lookup"><span data-stu-id="00ac5-112">String</span></span>|<span data-ttu-id="00ac5-113">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="00ac5-113">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="00ac5-114">appleId</span><span class="sxs-lookup"><span data-stu-id="00ac5-114">appleId</span></span>|<span data-ttu-id="00ac5-115">String</span><span class="sxs-lookup"><span data-stu-id="00ac5-115">String</span></span>|<span data-ttu-id="00ac5-116">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="00ac5-116">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="00ac5-117">organizationName</span><span class="sxs-lookup"><span data-stu-id="00ac5-117">organizationName</span></span>|<span data-ttu-id="00ac5-118">String</span><span class="sxs-lookup"><span data-stu-id="00ac5-118">String</span></span>|<span data-ttu-id="00ac5-119">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="00ac5-119">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="00ac5-120">Аваилаблелиценсекаунт</span><span class="sxs-lookup"><span data-stu-id="00ac5-120">availableLicenseCount</span></span>|<span data-ttu-id="00ac5-121">Int32</span><span class="sxs-lookup"><span data-stu-id="00ac5-121">Int32</span></span>|<span data-ttu-id="00ac5-122">Число доступных лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="00ac5-122">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="00ac5-123">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="00ac5-123">usedLicenseCount</span></span>|<span data-ttu-id="00ac5-124">Int32</span><span class="sxs-lookup"><span data-stu-id="00ac5-124">Int32</span></span>|<span data-ttu-id="00ac5-125">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="00ac5-125">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00ac5-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="00ac5-126">Relationships</span></span>
<span data-ttu-id="00ac5-127">Нет</span><span class="sxs-lookup"><span data-stu-id="00ac5-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00ac5-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00ac5-128">JSON Representation</span></span>
<span data-ttu-id="00ac5-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00ac5-129">Here is a JSON representation of the resource.</span></span>
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





