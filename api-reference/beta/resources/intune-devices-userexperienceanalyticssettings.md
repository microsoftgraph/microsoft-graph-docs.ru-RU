---
title: Тип ресурса Усерекспериенцеаналитикссеттингс
description: Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 07b1249da8d05931f4176c1bdb82f99daa1e3f00
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727388"
---
# <a name="userexperienceanalyticssettings-resource-type"></a><span data-ttu-id="0bfb6-103">Тип ресурса Усерекспериенцеаналитикссеттингс</span><span class="sxs-lookup"><span data-stu-id="0bfb6-103">userExperienceAnalyticsSettings resource type</span></span>

<span data-ttu-id="0bfb6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bfb6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bfb6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bfb6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bfb6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0bfb6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bfb6-107">Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="0bfb6-107">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="0bfb6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0bfb6-108">Properties</span></span>
|<span data-ttu-id="0bfb6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0bfb6-109">Property</span></span>|<span data-ttu-id="0bfb6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0bfb6-110">Type</span></span>|<span data-ttu-id="0bfb6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0bfb6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bfb6-112">конфигуратионманажердатаконнекторконфигуред</span><span class="sxs-lookup"><span data-stu-id="0bfb6-112">configurationManagerDataConnectorConfigured</span></span>|<span data-ttu-id="0bfb6-113">Логический</span><span class="sxs-lookup"><span data-stu-id="0bfb6-113">Boolean</span></span>|<span data-ttu-id="0bfb6-114">Значение true, если присоединение клиента настроено.</span><span class="sxs-lookup"><span data-stu-id="0bfb6-114">True if Tenant attach is configured.</span></span> <span data-ttu-id="0bfb6-115">Если этот флажок установлен, подключенные к клиенту SCCM устройства будут отображаться в отчетах УКСА.</span><span class="sxs-lookup"><span data-stu-id="0bfb6-115">If configured then SCCM tenant attached devices will show up in UXA reporting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bfb6-116">Связи</span><span class="sxs-lookup"><span data-stu-id="0bfb6-116">Relationships</span></span>
<span data-ttu-id="0bfb6-117">Нет</span><span class="sxs-lookup"><span data-stu-id="0bfb6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0bfb6-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0bfb6-118">JSON Representation</span></span>
<span data-ttu-id="0bfb6-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0bfb6-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsSettings",
  "configurationManagerDataConnectorConfigured": true
}
```





