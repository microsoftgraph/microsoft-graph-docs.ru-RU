---
title: тип перечисления Диагностикдатасубмиссионмоде
description: Разрешить устройству отправку данных о диагностике и использовании, например Watson.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 80a936c103caa4655addd25f8a21d75d9bc67040
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465690"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="aa1b8-103">тип перечисления Диагностикдатасубмиссионмоде</span><span class="sxs-lookup"><span data-stu-id="aa1b8-103">diagnosticDataSubmissionMode enum type</span></span>

<span data-ttu-id="aa1b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa1b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa1b8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa1b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa1b8-106">Разрешить устройству отправку данных о диагностике и использовании, например Watson.</span><span class="sxs-lookup"><span data-stu-id="aa1b8-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="aa1b8-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="aa1b8-107">Members</span></span>
|<span data-ttu-id="aa1b8-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="aa1b8-108">Member</span></span>|<span data-ttu-id="aa1b8-109">Значение</span><span class="sxs-lookup"><span data-stu-id="aa1b8-109">Value</span></span>|<span data-ttu-id="aa1b8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aa1b8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa1b8-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="aa1b8-111">userDefined</span></span>|<span data-ttu-id="aa1b8-112">нуль</span><span class="sxs-lookup"><span data-stu-id="aa1b8-112">0</span></span>|<span data-ttu-id="aa1b8-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="aa1b8-113">Allow the user to set.</span></span>|
|<span data-ttu-id="aa1b8-114">Нет</span><span class="sxs-lookup"><span data-stu-id="aa1b8-114">none</span></span>|<span data-ttu-id="aa1b8-115">1,1</span><span class="sxs-lookup"><span data-stu-id="aa1b8-115">1</span></span>|<span data-ttu-id="aa1b8-116">Данные телеметрии не отправляются из компонентов ОС.</span><span class="sxs-lookup"><span data-stu-id="aa1b8-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="aa1b8-117">Примечание: это значение относится только к корпоративным и серверным устройствам.</span><span class="sxs-lookup"><span data-stu-id="aa1b8-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="aa1b8-118">Использование этого параметра на других устройствах эквивалентно установке значения 1.</span><span class="sxs-lookup"><span data-stu-id="aa1b8-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="aa1b8-119">Основное</span><span class="sxs-lookup"><span data-stu-id="aa1b8-119">basic</span></span>|<span data-ttu-id="aa1b8-120">2</span><span class="sxs-lookup"><span data-stu-id="aa1b8-120">2</span></span>|<span data-ttu-id="aa1b8-121">Отправляет основные данные телеметрии.</span><span class="sxs-lookup"><span data-stu-id="aa1b8-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="aa1b8-122">усовершенствован</span><span class="sxs-lookup"><span data-stu-id="aa1b8-122">enhanced</span></span>|<span data-ttu-id="aa1b8-123">4</span><span class="sxs-lookup"><span data-stu-id="aa1b8-123">3</span></span>|<span data-ttu-id="aa1b8-124">Отправляет расширенные данные телеметрии, в том числе сведения об использовании и Insights.</span><span class="sxs-lookup"><span data-stu-id="aa1b8-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="aa1b8-125">полный</span><span class="sxs-lookup"><span data-stu-id="aa1b8-125">full</span></span>|<span data-ttu-id="aa1b8-126">4 </span><span class="sxs-lookup"><span data-stu-id="aa1b8-126">4</span></span>|<span data-ttu-id="aa1b8-127">Отправляет полные данные телеметрии, в том числе диагностические данные, например состояние системы.</span><span class="sxs-lookup"><span data-stu-id="aa1b8-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|







