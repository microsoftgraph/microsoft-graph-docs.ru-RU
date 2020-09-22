---
title: Тип ресурса Adminconsent.
description: Сведения о согласия администратора.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b09db43661113de84712a8228af047ca1683c383
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060904"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="37936-103">Тип ресурса Adminconsent.</span><span class="sxs-lookup"><span data-stu-id="37936-103">adminConsent resource type</span></span>

<span data-ttu-id="37936-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37936-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37936-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37936-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37936-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37936-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37936-107">Сведения о согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="37936-107">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="37936-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="37936-108">Properties</span></span>
|<span data-ttu-id="37936-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="37936-109">Property</span></span>|<span data-ttu-id="37936-110">Тип</span><span class="sxs-lookup"><span data-stu-id="37936-110">Type</span></span>|<span data-ttu-id="37936-111">Описание</span><span class="sxs-lookup"><span data-stu-id="37936-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37936-112">шареапнсдата</span><span class="sxs-lookup"><span data-stu-id="37936-112">shareAPNSData</span></span>|[<span data-ttu-id="37936-113">админконсентстате</span><span class="sxs-lookup"><span data-stu-id="37936-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="37936-114">Разрешение администратора о предоставлении общего доступа к данным о пользователях и устройствах в Apple.</span><span class="sxs-lookup"><span data-stu-id="37936-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="37936-115">Возможные значения: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="37936-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|
|<span data-ttu-id="37936-116">шареусерекспериенцеаналитиксдата</span><span class="sxs-lookup"><span data-stu-id="37936-116">shareUserExperienceAnalyticsData</span></span>|[<span data-ttu-id="37936-117">админконсентстате</span><span class="sxs-lookup"><span data-stu-id="37936-117">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="37936-118">Получает или задает согласие администратора для совместного использования данных аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="37936-118">Gets or sets the admin consent for sharing User experience analytics data.</span></span> <span data-ttu-id="37936-119">Возможные значения: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="37936-119">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37936-120">Связи</span><span class="sxs-lookup"><span data-stu-id="37936-120">Relationships</span></span>
<span data-ttu-id="37936-121">Нет</span><span class="sxs-lookup"><span data-stu-id="37936-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37936-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37936-122">JSON Representation</span></span>
<span data-ttu-id="37936-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37936-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String",
  "shareUserExperienceAnalyticsData": "String"
}
```






