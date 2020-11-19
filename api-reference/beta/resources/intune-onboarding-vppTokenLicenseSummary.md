---
title: Тип ресурса Впптокенлиценсесуммари
description: Сводка по лицензии для определенного приложения в маркере.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5182e9aebbefa1a1ce818e52cb442a8950b0b737
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301202"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="f4c9b-103">Тип ресурса Впптокенлиценсесуммари</span><span class="sxs-lookup"><span data-stu-id="f4c9b-103">vppTokenLicenseSummary resource type</span></span>

<span data-ttu-id="f4c9b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4c9b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4c9b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4c9b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4c9b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4c9b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4c9b-107">Сводка по лицензии для определенного приложения в маркере.</span><span class="sxs-lookup"><span data-stu-id="f4c9b-107">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="f4c9b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4c9b-108">Properties</span></span>
|<span data-ttu-id="f4c9b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4c9b-109">Property</span></span>|<span data-ttu-id="f4c9b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f4c9b-110">Type</span></span>|<span data-ttu-id="f4c9b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f4c9b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4c9b-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="f4c9b-112">vppTokenId</span></span>|<span data-ttu-id="f4c9b-113">String</span><span class="sxs-lookup"><span data-stu-id="f4c9b-113">String</span></span>|<span data-ttu-id="f4c9b-114">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="f4c9b-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="f4c9b-115">appleId</span><span class="sxs-lookup"><span data-stu-id="f4c9b-115">appleId</span></span>|<span data-ttu-id="f4c9b-116">String</span><span class="sxs-lookup"><span data-stu-id="f4c9b-116">String</span></span>|<span data-ttu-id="f4c9b-117">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="f4c9b-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f4c9b-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="f4c9b-118">organizationName</span></span>|<span data-ttu-id="f4c9b-119">Строка</span><span class="sxs-lookup"><span data-stu-id="f4c9b-119">String</span></span>|<span data-ttu-id="f4c9b-120">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="f4c9b-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f4c9b-121">аваилаблелиценсекаунт</span><span class="sxs-lookup"><span data-stu-id="f4c9b-121">availableLicenseCount</span></span>|<span data-ttu-id="f4c9b-122">Int32</span><span class="sxs-lookup"><span data-stu-id="f4c9b-122">Int32</span></span>|<span data-ttu-id="f4c9b-123">Число доступных лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="f4c9b-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="f4c9b-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f4c9b-124">usedLicenseCount</span></span>|<span data-ttu-id="f4c9b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f4c9b-125">Int32</span></span>|<span data-ttu-id="f4c9b-126">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="f4c9b-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4c9b-127">Связи</span><span class="sxs-lookup"><span data-stu-id="f4c9b-127">Relationships</span></span>
<span data-ttu-id="f4c9b-128">Нет</span><span class="sxs-lookup"><span data-stu-id="f4c9b-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4c9b-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4c9b-129">JSON Representation</span></span>
<span data-ttu-id="f4c9b-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4c9b-130">Here is a JSON representation of the resource.</span></span>
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




