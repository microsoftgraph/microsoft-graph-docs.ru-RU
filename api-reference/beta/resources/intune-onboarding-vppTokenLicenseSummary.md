---
title: Тип ресурса vppTokenLicenseSummary
description: Сводка данного приложения в маркер лицензии.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0766fd4da996b57032154be98bbc22fd8c8a4a5b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939961"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="5afed-103">Тип ресурса vppTokenLicenseSummary</span><span class="sxs-lookup"><span data-stu-id="5afed-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="5afed-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5afed-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5afed-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5afed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5afed-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5afed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5afed-107">Сводка данного приложения в маркер лицензии.</span><span class="sxs-lookup"><span data-stu-id="5afed-107">License summary of a given app in a token.</span></span>
## <a name="properties"></a><span data-ttu-id="5afed-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5afed-108">Properties</span></span>
|<span data-ttu-id="5afed-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5afed-109">Property</span></span>|<span data-ttu-id="5afed-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5afed-110">Type</span></span>|<span data-ttu-id="5afed-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5afed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5afed-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="5afed-112">vppTokenId</span></span>|<span data-ttu-id="5afed-113">String</span><span class="sxs-lookup"><span data-stu-id="5afed-113">String</span></span>|<span data-ttu-id="5afed-114">Идентификатор маркера VPP.</span><span class="sxs-lookup"><span data-stu-id="5afed-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="5afed-115">appleId</span><span class="sxs-lookup"><span data-stu-id="5afed-115">appleId</span></span>|<span data-ttu-id="5afed-116">String</span><span class="sxs-lookup"><span data-stu-id="5afed-116">String</span></span>|<span data-ttu-id="5afed-117">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="5afed-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="5afed-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="5afed-118">organizationName</span></span>|<span data-ttu-id="5afed-119">Строка</span><span class="sxs-lookup"><span data-stu-id="5afed-119">String</span></span>|<span data-ttu-id="5afed-120">Организации, связанной с Apple тома покупки программа маркеров.</span><span class="sxs-lookup"><span data-stu-id="5afed-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="5afed-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="5afed-121">availableLicenseCount</span></span>|<span data-ttu-id="5afed-122">Int32</span><span class="sxs-lookup"><span data-stu-id="5afed-122">Int32</span></span>|<span data-ttu-id="5afed-123">Число доступных лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="5afed-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="5afed-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="5afed-124">usedLicenseCount</span></span>|<span data-ttu-id="5afed-125">Int32</span><span class="sxs-lookup"><span data-stu-id="5afed-125">Int32</span></span>|<span data-ttu-id="5afed-126">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="5afed-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5afed-127">Связи</span><span class="sxs-lookup"><span data-stu-id="5afed-127">Relationships</span></span>
<span data-ttu-id="5afed-128">Нет</span><span class="sxs-lookup"><span data-stu-id="5afed-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5afed-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5afed-129">JSON Representation</span></span>
<span data-ttu-id="5afed-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5afed-130">Here is a JSON representation of the resource.</span></span>
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





