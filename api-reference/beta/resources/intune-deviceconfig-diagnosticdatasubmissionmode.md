---
title: тип перечисления Диагностикдатасубмиссионмоде
description: Разрешить устройству отправку данных о диагностике и использовании, например Watson.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fce6bbe40d985c15c5455c3b83de88ced4cce768
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332689"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="8fec5-103">тип перечисления Диагностикдатасубмиссионмоде</span><span class="sxs-lookup"><span data-stu-id="8fec5-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="8fec5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fec5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fec5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8fec5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fec5-106">Разрешить устройству отправку данных о диагностике и использовании, например Watson.</span><span class="sxs-lookup"><span data-stu-id="8fec5-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="8fec5-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="8fec5-107">Members</span></span>
|<span data-ttu-id="8fec5-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="8fec5-108">Member</span></span>|<span data-ttu-id="8fec5-109">Значение</span><span class="sxs-lookup"><span data-stu-id="8fec5-109">Value</span></span>|<span data-ttu-id="8fec5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8fec5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fec5-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="8fec5-111">userDefined</span></span>|<span data-ttu-id="8fec5-112">нуль</span><span class="sxs-lookup"><span data-stu-id="8fec5-112">0</span></span>|<span data-ttu-id="8fec5-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="8fec5-113">Allow the user to set.</span></span>|
|<span data-ttu-id="8fec5-114">none</span><span class="sxs-lookup"><span data-stu-id="8fec5-114">none</span></span>|<span data-ttu-id="8fec5-115">1,1</span><span class="sxs-lookup"><span data-stu-id="8fec5-115">1</span></span>|<span data-ttu-id="8fec5-116">Данные телеметрии не отправляются из компонентов ОС.</span><span class="sxs-lookup"><span data-stu-id="8fec5-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="8fec5-117">Примечание: это значение относится только к корпоративным и серверным устройствам.</span><span class="sxs-lookup"><span data-stu-id="8fec5-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="8fec5-118">Использование этого параметра на других устройствах эквивалентно установке значения 1.</span><span class="sxs-lookup"><span data-stu-id="8fec5-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="8fec5-119">Основное</span><span class="sxs-lookup"><span data-stu-id="8fec5-119">basic</span></span>|<span data-ttu-id="8fec5-120">2</span><span class="sxs-lookup"><span data-stu-id="8fec5-120">2</span></span>|<span data-ttu-id="8fec5-121">Отправляет основные данные телеметрии.</span><span class="sxs-lookup"><span data-stu-id="8fec5-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="8fec5-122">усовершенствован</span><span class="sxs-lookup"><span data-stu-id="8fec5-122">enhanced</span></span>|<span data-ttu-id="8fec5-123">4</span><span class="sxs-lookup"><span data-stu-id="8fec5-123">3</span></span>|<span data-ttu-id="8fec5-124">Отправляет расширенные данные телеметрии, в том числе сведения об использовании и Insights.</span><span class="sxs-lookup"><span data-stu-id="8fec5-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="8fec5-125">полный</span><span class="sxs-lookup"><span data-stu-id="8fec5-125">full</span></span>|<span data-ttu-id="8fec5-126">SP4</span><span class="sxs-lookup"><span data-stu-id="8fec5-126">4</span></span>|<span data-ttu-id="8fec5-127">Отправляет полные данные телеметрии, в том числе диагностические данные, например состояние системы.</span><span class="sxs-lookup"><span data-stu-id="8fec5-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



