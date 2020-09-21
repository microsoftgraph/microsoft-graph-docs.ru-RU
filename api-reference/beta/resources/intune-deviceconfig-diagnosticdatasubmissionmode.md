---
title: тип перечисления Диагностикдатасубмиссионмоде
description: Разрешить устройству отправку данных о диагностике и использовании, например Watson.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7ef0a61e8d95793e6e4717a3a5ed66d518e80590
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968446"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="224e4-103">тип перечисления Диагностикдатасубмиссионмоде</span><span class="sxs-lookup"><span data-stu-id="224e4-103">diagnosticDataSubmissionMode enum type</span></span>

<span data-ttu-id="224e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="224e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="224e4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="224e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="224e4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="224e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="224e4-107">Разрешить устройству отправку данных о диагностике и использовании, например Watson.</span><span class="sxs-lookup"><span data-stu-id="224e4-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="224e4-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="224e4-108">Members</span></span>
|<span data-ttu-id="224e4-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="224e4-109">Member</span></span>|<span data-ttu-id="224e4-110">Значение</span><span class="sxs-lookup"><span data-stu-id="224e4-110">Value</span></span>|<span data-ttu-id="224e4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="224e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="224e4-112">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="224e4-112">userDefined</span></span>|<span data-ttu-id="224e4-113">нуль</span><span class="sxs-lookup"><span data-stu-id="224e4-113">0</span></span>|<span data-ttu-id="224e4-114">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="224e4-114">Allow the user to set.</span></span>|
|<span data-ttu-id="224e4-115">Нет</span><span class="sxs-lookup"><span data-stu-id="224e4-115">none</span></span>|<span data-ttu-id="224e4-116">1 </span><span class="sxs-lookup"><span data-stu-id="224e4-116">1</span></span>|<span data-ttu-id="224e4-117">Данные телеметрии не отправляются из компонентов ОС.</span><span class="sxs-lookup"><span data-stu-id="224e4-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="224e4-118">Примечание: это значение относится только к корпоративным и серверным устройствам.</span><span class="sxs-lookup"><span data-stu-id="224e4-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="224e4-119">Использование этого параметра на других устройствах эквивалентно установке значения 1.</span><span class="sxs-lookup"><span data-stu-id="224e4-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="224e4-120">Основное</span><span class="sxs-lookup"><span data-stu-id="224e4-120">basic</span></span>|<span data-ttu-id="224e4-121">2 </span><span class="sxs-lookup"><span data-stu-id="224e4-121">2</span></span>|<span data-ttu-id="224e4-122">Отправляет основные данные телеметрии.</span><span class="sxs-lookup"><span data-stu-id="224e4-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="224e4-123">усовершенствован</span><span class="sxs-lookup"><span data-stu-id="224e4-123">enhanced</span></span>|<span data-ttu-id="224e4-124">4</span><span class="sxs-lookup"><span data-stu-id="224e4-124">3</span></span>|<span data-ttu-id="224e4-125">Отправляет расширенные данные телеметрии, в том числе сведения об использовании и Insights.</span><span class="sxs-lookup"><span data-stu-id="224e4-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="224e4-126">полный</span><span class="sxs-lookup"><span data-stu-id="224e4-126">full</span></span>|<span data-ttu-id="224e4-127">4 </span><span class="sxs-lookup"><span data-stu-id="224e4-127">4</span></span>|<span data-ttu-id="224e4-128">Отправляет полные данные телеметрии, в том числе диагностические данные, например состояние системы.</span><span class="sxs-lookup"><span data-stu-id="224e4-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|






