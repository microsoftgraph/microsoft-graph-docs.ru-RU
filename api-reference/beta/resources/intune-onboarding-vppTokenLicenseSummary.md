---
title: Тип ресурса vppTokenLicenseSummary
description: Сводка данного приложения в маркер лицензии.
ms.openlocfilehash: fba888c706b21a796615bf9bc2ea79968d5ad6d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076466"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="06ffb-103">Тип ресурса vppTokenLicenseSummary</span><span class="sxs-lookup"><span data-stu-id="06ffb-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="06ffb-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="06ffb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06ffb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06ffb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06ffb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="06ffb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06ffb-107">Сводка данного приложения в маркер лицензии.</span><span class="sxs-lookup"><span data-stu-id="06ffb-107">License summary of a given app in a token.</span></span>
## <a name="properties"></a><span data-ttu-id="06ffb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="06ffb-108">Properties</span></span>
|<span data-ttu-id="06ffb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="06ffb-109">Property</span></span>|<span data-ttu-id="06ffb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="06ffb-110">Type</span></span>|<span data-ttu-id="06ffb-111">Description</span><span class="sxs-lookup"><span data-stu-id="06ffb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06ffb-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="06ffb-112">vppTokenId</span></span>|<span data-ttu-id="06ffb-113">String</span><span class="sxs-lookup"><span data-stu-id="06ffb-113">String</span></span>|<span data-ttu-id="06ffb-114">Идентификатор маркера VPP.</span><span class="sxs-lookup"><span data-stu-id="06ffb-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="06ffb-115">appleId</span><span class="sxs-lookup"><span data-stu-id="06ffb-115">appleId</span></span>|<span data-ttu-id="06ffb-116">String</span><span class="sxs-lookup"><span data-stu-id="06ffb-116">String</span></span>|<span data-ttu-id="06ffb-117">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="06ffb-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="06ffb-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="06ffb-118">organizationName</span></span>|<span data-ttu-id="06ffb-119">Строка</span><span class="sxs-lookup"><span data-stu-id="06ffb-119">String</span></span>|<span data-ttu-id="06ffb-120">Организации, связанной с Apple тома покупки программа маркеров.</span><span class="sxs-lookup"><span data-stu-id="06ffb-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="06ffb-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="06ffb-121">availableLicenseCount</span></span>|<span data-ttu-id="06ffb-122">Int32</span><span class="sxs-lookup"><span data-stu-id="06ffb-122">Int32</span></span>|<span data-ttu-id="06ffb-123">Число доступных лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="06ffb-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="06ffb-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="06ffb-124">usedLicenseCount</span></span>|<span data-ttu-id="06ffb-125">Int32</span><span class="sxs-lookup"><span data-stu-id="06ffb-125">Int32</span></span>|<span data-ttu-id="06ffb-126">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="06ffb-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06ffb-127">Связи</span><span class="sxs-lookup"><span data-stu-id="06ffb-127">Relationships</span></span>
<span data-ttu-id="06ffb-128">Нет</span><span class="sxs-lookup"><span data-stu-id="06ffb-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="06ffb-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06ffb-129">JSON Representation</span></span>
<span data-ttu-id="06ffb-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06ffb-130">Here is a JSON representation of the resource.</span></span>
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





