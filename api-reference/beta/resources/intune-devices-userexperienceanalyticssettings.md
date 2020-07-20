---
title: Тип ресурса Усерекспериенцеаналитикссеттингс
description: Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 950bd227d36cc691072fb11b17d2a0972d00de07
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793649"
---
# <a name="userexperienceanalyticssettings-resource-type"></a><span data-ttu-id="421ae-103">Тип ресурса Усерекспериенцеаналитикссеттингс</span><span class="sxs-lookup"><span data-stu-id="421ae-103">userExperienceAnalyticsSettings resource type</span></span>

<span data-ttu-id="421ae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="421ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="421ae-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="421ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="421ae-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="421ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="421ae-107">Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="421ae-107">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="421ae-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="421ae-108">Properties</span></span>
|<span data-ttu-id="421ae-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="421ae-109">Property</span></span>|<span data-ttu-id="421ae-110">Тип</span><span class="sxs-lookup"><span data-stu-id="421ae-110">Type</span></span>|<span data-ttu-id="421ae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="421ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="421ae-112">конфигуратионманажердатаконнекторконфигуред</span><span class="sxs-lookup"><span data-stu-id="421ae-112">configurationManagerDataConnectorConfigured</span></span>|<span data-ttu-id="421ae-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="421ae-113">Boolean</span></span>|<span data-ttu-id="421ae-114">Значение true, если присоединение клиента настроено.</span><span class="sxs-lookup"><span data-stu-id="421ae-114">True if Tenant attach is configured.</span></span> <span data-ttu-id="421ae-115">Если этот флажок установлен, подключенные к клиенту SCCM устройства будут отображаться в отчетах УКСА.</span><span class="sxs-lookup"><span data-stu-id="421ae-115">If configured then SCCM tenant attached devices will show up in UXA reporting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="421ae-116">Связи</span><span class="sxs-lookup"><span data-stu-id="421ae-116">Relationships</span></span>
<span data-ttu-id="421ae-117">Нет</span><span class="sxs-lookup"><span data-stu-id="421ae-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="421ae-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="421ae-118">JSON Representation</span></span>
<span data-ttu-id="421ae-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="421ae-119">Here is a JSON representation of the resource.</span></span>
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



