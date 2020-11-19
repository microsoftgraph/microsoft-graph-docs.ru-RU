---
title: Тип ресурса Adminconsent.
description: Сведения о согласия администратора.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 11a8cd99c544dcd11b713d4c3c98eede77c48eb1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49209222"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="81a9d-103">Тип ресурса Adminconsent.</span><span class="sxs-lookup"><span data-stu-id="81a9d-103">adminConsent resource type</span></span>

<span data-ttu-id="81a9d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81a9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81a9d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81a9d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81a9d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="81a9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81a9d-107">Сведения о согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="81a9d-107">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="81a9d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="81a9d-108">Properties</span></span>
|<span data-ttu-id="81a9d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="81a9d-109">Property</span></span>|<span data-ttu-id="81a9d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="81a9d-110">Type</span></span>|<span data-ttu-id="81a9d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="81a9d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81a9d-112">шареапнсдата</span><span class="sxs-lookup"><span data-stu-id="81a9d-112">shareAPNSData</span></span>|[<span data-ttu-id="81a9d-113">админконсентстате</span><span class="sxs-lookup"><span data-stu-id="81a9d-113">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="81a9d-114">Разрешение администратора о предоставлении общего доступа к данным о пользователях и устройствах в Apple.</span><span class="sxs-lookup"><span data-stu-id="81a9d-114">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="81a9d-115">Возможные значения: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="81a9d-115">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|
|<span data-ttu-id="81a9d-116">шареусерекспериенцеаналитиксдата</span><span class="sxs-lookup"><span data-stu-id="81a9d-116">shareUserExperienceAnalyticsData</span></span>|[<span data-ttu-id="81a9d-117">админконсентстате</span><span class="sxs-lookup"><span data-stu-id="81a9d-117">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="81a9d-118">Получает или задает согласие администратора для совместного использования данных аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="81a9d-118">Gets or sets the admin consent for sharing User experience analytics data.</span></span> <span data-ttu-id="81a9d-119">Возможные значения: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="81a9d-119">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81a9d-120">Связи</span><span class="sxs-lookup"><span data-stu-id="81a9d-120">Relationships</span></span>
<span data-ttu-id="81a9d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="81a9d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81a9d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81a9d-122">JSON Representation</span></span>
<span data-ttu-id="81a9d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81a9d-123">Here is a JSON representation of the resource.</span></span>
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




