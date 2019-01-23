---
title: Тип ресурса vppTokenLicenseSummary
description: Сводка данного приложения в маркер лицензии.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8fb84a549d95459db1e4b39c11b526f73db08752
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395183"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="e5ece-103">Тип ресурса vppTokenLicenseSummary</span><span class="sxs-lookup"><span data-stu-id="e5ece-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="e5ece-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e5ece-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e5ece-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5ece-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5ece-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5ece-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5ece-107">Сводка данного приложения в маркер лицензии.</span><span class="sxs-lookup"><span data-stu-id="e5ece-107">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="e5ece-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5ece-108">Properties</span></span>
|<span data-ttu-id="e5ece-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5ece-109">Property</span></span>|<span data-ttu-id="e5ece-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e5ece-110">Type</span></span>|<span data-ttu-id="e5ece-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e5ece-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5ece-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="e5ece-112">vppTokenId</span></span>|<span data-ttu-id="e5ece-113">String</span><span class="sxs-lookup"><span data-stu-id="e5ece-113">String</span></span>|<span data-ttu-id="e5ece-114">Идентификатор маркера VPP.</span><span class="sxs-lookup"><span data-stu-id="e5ece-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="e5ece-115">appleId</span><span class="sxs-lookup"><span data-stu-id="e5ece-115">appleId</span></span>|<span data-ttu-id="e5ece-116">String</span><span class="sxs-lookup"><span data-stu-id="e5ece-116">String</span></span>|<span data-ttu-id="e5ece-117">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="e5ece-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="e5ece-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="e5ece-118">organizationName</span></span>|<span data-ttu-id="e5ece-119">Строка</span><span class="sxs-lookup"><span data-stu-id="e5ece-119">String</span></span>|<span data-ttu-id="e5ece-120">Организации, связанной с Apple тома покупки программа маркеров.</span><span class="sxs-lookup"><span data-stu-id="e5ece-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="e5ece-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e5ece-121">availableLicenseCount</span></span>|<span data-ttu-id="e5ece-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e5ece-122">Int32</span></span>|<span data-ttu-id="e5ece-123">Число доступных лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="e5ece-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="e5ece-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e5ece-124">usedLicenseCount</span></span>|<span data-ttu-id="e5ece-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e5ece-125">Int32</span></span>|<span data-ttu-id="e5ece-126">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="e5ece-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5ece-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="e5ece-127">Relationships</span></span>
<span data-ttu-id="e5ece-128">Нет</span><span class="sxs-lookup"><span data-stu-id="e5ece-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5ece-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5ece-129">JSON Representation</span></span>
<span data-ttu-id="e5ece-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5ece-130">Here is a JSON representation of the resource.</span></span>
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




