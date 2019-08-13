---
title: Тип ресурса Adminconsent.
description: Сведения о согласия администратора.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8d78333cd683501a8bf4fea0aa3a2e55944d9b5a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319311"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="d9ade-103">Тип ресурса Adminconsent.</span><span class="sxs-lookup"><span data-stu-id="d9ade-103">adminConsent resource type</span></span>

> <span data-ttu-id="d9ade-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9ade-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9ade-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9ade-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9ade-106">Сведения о согласия администратора.</span><span class="sxs-lookup"><span data-stu-id="d9ade-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="d9ade-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9ade-107">Properties</span></span>
|<span data-ttu-id="d9ade-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9ade-108">Property</span></span>|<span data-ttu-id="d9ade-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d9ade-109">Type</span></span>|<span data-ttu-id="d9ade-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d9ade-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9ade-111">шареапнсдата</span><span class="sxs-lookup"><span data-stu-id="d9ade-111">shareAPNSData</span></span>|[<span data-ttu-id="d9ade-112">админконсентстате</span><span class="sxs-lookup"><span data-stu-id="d9ade-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="d9ade-113">Разрешение администратора о предоставлении общего доступа к данным о пользователях и устройствах в Apple.</span><span class="sxs-lookup"><span data-stu-id="d9ade-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="d9ade-114">Возможные значения: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="d9ade-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|
|<span data-ttu-id="d9ade-115">шареусерекспериенцеаналитиксдата</span><span class="sxs-lookup"><span data-stu-id="d9ade-115">shareUserExperienceAnalyticsData</span></span>|[<span data-ttu-id="d9ade-116">админконсентстате</span><span class="sxs-lookup"><span data-stu-id="d9ade-116">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="d9ade-117">Получает или задает согласие администратора для совместного использования данных аналитики взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="d9ade-117">Gets or sets the admin consent for sharing User experience analytics data.</span></span> <span data-ttu-id="d9ade-118">Возможные значения: `notConfigured`, `granted`, `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="d9ade-118">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9ade-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="d9ade-119">Relationships</span></span>
<span data-ttu-id="d9ade-120">Нет</span><span class="sxs-lookup"><span data-stu-id="d9ade-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9ade-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9ade-121">JSON Representation</span></span>
<span data-ttu-id="d9ade-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9ade-122">Here is a JSON representation of the resource.</span></span>
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



