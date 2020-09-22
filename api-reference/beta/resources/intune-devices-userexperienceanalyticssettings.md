---
title: Тип ресурса Усерекспериенцеаналитикссеттингс
description: Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2783d882c3ba5e5d8154be35db6a4a8411227955
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080763"
---
# <a name="userexperienceanalyticssettings-resource-type"></a><span data-ttu-id="8bcdb-103">Тип ресурса Усерекспериенцеаналитикссеттингс</span><span class="sxs-lookup"><span data-stu-id="8bcdb-103">userExperienceAnalyticsSettings resource type</span></span>

<span data-ttu-id="8bcdb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bcdb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8bcdb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bcdb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bcdb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bcdb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bcdb-107">Аналитика пользовательского интерфейса является рекомендацией для усовершенствования оценки анализа взаимодействия с пользователем.</span><span class="sxs-lookup"><span data-stu-id="8bcdb-107">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="8bcdb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bcdb-108">Properties</span></span>
|<span data-ttu-id="8bcdb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bcdb-109">Property</span></span>|<span data-ttu-id="8bcdb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8bcdb-110">Type</span></span>|<span data-ttu-id="8bcdb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8bcdb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bcdb-112">конфигуратионманажердатаконнекторконфигуред</span><span class="sxs-lookup"><span data-stu-id="8bcdb-112">configurationManagerDataConnectorConfigured</span></span>|<span data-ttu-id="8bcdb-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bcdb-113">Boolean</span></span>|<span data-ttu-id="8bcdb-114">Значение true, если присоединение клиента настроено.</span><span class="sxs-lookup"><span data-stu-id="8bcdb-114">True if Tenant attach is configured.</span></span> <span data-ttu-id="8bcdb-115">Если этот флажок установлен, подключенные к клиенту SCCM устройства будут отображаться в отчетах УКСА.</span><span class="sxs-lookup"><span data-stu-id="8bcdb-115">If configured then SCCM tenant attached devices will show up in UXA reporting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bcdb-116">Связи</span><span class="sxs-lookup"><span data-stu-id="8bcdb-116">Relationships</span></span>
<span data-ttu-id="8bcdb-117">Нет</span><span class="sxs-lookup"><span data-stu-id="8bcdb-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bcdb-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8bcdb-118">JSON Representation</span></span>
<span data-ttu-id="8bcdb-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bcdb-119">Here is a JSON representation of the resource.</span></span>
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






