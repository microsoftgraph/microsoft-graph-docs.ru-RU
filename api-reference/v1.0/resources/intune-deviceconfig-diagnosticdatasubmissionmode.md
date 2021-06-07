---
title: тип enum diagnosticDataSubmissionMode
description: Разрешить устройству отправлять данные телеметрии диагностики и использования, такие как Watson.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 172ac80e4491d238414777c4d1d30d9f969f2a39
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755086"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="42399-103">тип enum diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="42399-103">diagnosticDataSubmissionMode enum type</span></span>

<span data-ttu-id="42399-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42399-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42399-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42399-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42399-106">Разрешить устройству отправлять данные телеметрии диагностики и использования, такие как Watson.</span><span class="sxs-lookup"><span data-stu-id="42399-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="42399-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="42399-107">Members</span></span>
|<span data-ttu-id="42399-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="42399-108">Member</span></span>|<span data-ttu-id="42399-109">Значение</span><span class="sxs-lookup"><span data-stu-id="42399-109">Value</span></span>|<span data-ttu-id="42399-110">Описание</span><span class="sxs-lookup"><span data-stu-id="42399-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42399-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="42399-111">userDefined</span></span>|<span data-ttu-id="42399-112">0</span><span class="sxs-lookup"><span data-stu-id="42399-112">0</span></span>|<span data-ttu-id="42399-113">Разрешить пользователю установить.</span><span class="sxs-lookup"><span data-stu-id="42399-113">Allow the user to set.</span></span>|
|<span data-ttu-id="42399-114">нет</span><span class="sxs-lookup"><span data-stu-id="42399-114">none</span></span>|<span data-ttu-id="42399-115">1</span><span class="sxs-lookup"><span data-stu-id="42399-115">1</span></span>|<span data-ttu-id="42399-116">Данные телеметрии не отправляются из компонентов ОС.</span><span class="sxs-lookup"><span data-stu-id="42399-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="42399-117">Примечание. Это значение применимо только к корпоративным и серверным устройствам.</span><span class="sxs-lookup"><span data-stu-id="42399-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="42399-118">Использование этого параметра на других устройствах равно значению 1.</span><span class="sxs-lookup"><span data-stu-id="42399-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="42399-119">основные</span><span class="sxs-lookup"><span data-stu-id="42399-119">basic</span></span>|<span data-ttu-id="42399-120">2</span><span class="sxs-lookup"><span data-stu-id="42399-120">2</span></span>|<span data-ttu-id="42399-121">Отправляет основные данные телеметрии.</span><span class="sxs-lookup"><span data-stu-id="42399-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="42399-122">расширенный</span><span class="sxs-lookup"><span data-stu-id="42399-122">enhanced</span></span>|<span data-ttu-id="42399-123">3</span><span class="sxs-lookup"><span data-stu-id="42399-123">3</span></span>|<span data-ttu-id="42399-124">Отправляет расширенные данные телеметрии, включая данные об использовании и анализах.</span><span class="sxs-lookup"><span data-stu-id="42399-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="42399-125">полный</span><span class="sxs-lookup"><span data-stu-id="42399-125">full</span></span>|<span data-ttu-id="42399-126">4 </span><span class="sxs-lookup"><span data-stu-id="42399-126">4</span></span>|<span data-ttu-id="42399-127">Отправляет полные данные телеметрии, включая диагностические данные, например состояние системы.</span><span class="sxs-lookup"><span data-stu-id="42399-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




