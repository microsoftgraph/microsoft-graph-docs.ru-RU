---
title: тип перечисления Диагностикдатасубмиссионмоде
description: Разрешить устройству отправку данных о диагностике и использовании, например Watson.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e85544eef7556fd70c880f9c402966d251da6fc7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056823"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="d90d0-103">тип перечисления Диагностикдатасубмиссионмоде</span><span class="sxs-lookup"><span data-stu-id="d90d0-103">diagnosticDataSubmissionMode enum type</span></span>

<span data-ttu-id="d90d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d90d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d90d0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d90d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d90d0-106">Разрешить устройству отправку данных о диагностике и использовании, например Watson.</span><span class="sxs-lookup"><span data-stu-id="d90d0-106">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="d90d0-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="d90d0-107">Members</span></span>
|<span data-ttu-id="d90d0-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="d90d0-108">Member</span></span>|<span data-ttu-id="d90d0-109">Значение</span><span class="sxs-lookup"><span data-stu-id="d90d0-109">Value</span></span>|<span data-ttu-id="d90d0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d90d0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d90d0-111">UserDefined типа</span><span class="sxs-lookup"><span data-stu-id="d90d0-111">userDefined</span></span>|<span data-ttu-id="d90d0-112">нуль</span><span class="sxs-lookup"><span data-stu-id="d90d0-112">0</span></span>|<span data-ttu-id="d90d0-113">Разрешить пользователю устанавливать.</span><span class="sxs-lookup"><span data-stu-id="d90d0-113">Allow the user to set.</span></span>|
|<span data-ttu-id="d90d0-114">Нет</span><span class="sxs-lookup"><span data-stu-id="d90d0-114">none</span></span>|<span data-ttu-id="d90d0-115">1 </span><span class="sxs-lookup"><span data-stu-id="d90d0-115">1</span></span>|<span data-ttu-id="d90d0-116">Данные телеметрии не отправляются из компонентов ОС.</span><span class="sxs-lookup"><span data-stu-id="d90d0-116">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="d90d0-117">Примечание: это значение относится только к корпоративным и серверным устройствам.</span><span class="sxs-lookup"><span data-stu-id="d90d0-117">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="d90d0-118">Использование этого параметра на других устройствах эквивалентно установке значения 1.</span><span class="sxs-lookup"><span data-stu-id="d90d0-118">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="d90d0-119">Основное</span><span class="sxs-lookup"><span data-stu-id="d90d0-119">basic</span></span>|<span data-ttu-id="d90d0-120">2 </span><span class="sxs-lookup"><span data-stu-id="d90d0-120">2</span></span>|<span data-ttu-id="d90d0-121">Отправляет основные данные телеметрии.</span><span class="sxs-lookup"><span data-stu-id="d90d0-121">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="d90d0-122">усовершенствован</span><span class="sxs-lookup"><span data-stu-id="d90d0-122">enhanced</span></span>|<span data-ttu-id="d90d0-123">4</span><span class="sxs-lookup"><span data-stu-id="d90d0-123">3</span></span>|<span data-ttu-id="d90d0-124">Отправляет расширенные данные телеметрии, в том числе сведения об использовании и Insights.</span><span class="sxs-lookup"><span data-stu-id="d90d0-124">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="d90d0-125">полный</span><span class="sxs-lookup"><span data-stu-id="d90d0-125">full</span></span>|<span data-ttu-id="d90d0-126">4 </span><span class="sxs-lookup"><span data-stu-id="d90d0-126">4</span></span>|<span data-ttu-id="d90d0-127">Отправляет полные данные телеметрии, в том числе диагностические данные, например состояние системы.</span><span class="sxs-lookup"><span data-stu-id="d90d0-127">Sends full telemetry data including diagnostic data, such as system state.</span></span>|









