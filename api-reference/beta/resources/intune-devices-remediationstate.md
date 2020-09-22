---
title: тип перечисления Ремедиатионстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fb46c05ddbd1055f44794f0300077d47122aea25
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081120"
---
# <a name="remediationstate-enum-type"></a><span data-ttu-id="da493-103">тип перечисления Ремедиатионстате</span><span class="sxs-lookup"><span data-stu-id="da493-103">remediationState enum type</span></span>

<span data-ttu-id="da493-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da493-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da493-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da493-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da493-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="da493-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da493-107">Указывает тип состояния выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="da493-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="da493-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="da493-108">Members</span></span>
|<span data-ttu-id="da493-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="da493-109">Member</span></span>|<span data-ttu-id="da493-110">Значение</span><span class="sxs-lookup"><span data-stu-id="da493-110">Value</span></span>|<span data-ttu-id="da493-111">Описание</span><span class="sxs-lookup"><span data-stu-id="da493-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da493-112">unknown</span><span class="sxs-lookup"><span data-stu-id="da493-112">unknown</span></span>|<span data-ttu-id="da493-113">нуль</span><span class="sxs-lookup"><span data-stu-id="da493-113">0</span></span>|<span data-ttu-id="da493-114">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="da493-114">Unknown result.</span></span>|
|<span data-ttu-id="da493-115">пропущенных</span><span class="sxs-lookup"><span data-stu-id="da493-115">skipped</span></span>|<span data-ttu-id="da493-116">1 </span><span class="sxs-lookup"><span data-stu-id="da493-116">1</span></span>|<span data-ttu-id="da493-117">Выполнение скрипта исправления пропущено</span><span class="sxs-lookup"><span data-stu-id="da493-117">Remediation script execution was skipped</span></span>|
|<span data-ttu-id="da493-118">success</span><span class="sxs-lookup"><span data-stu-id="da493-118">success</span></span>|<span data-ttu-id="da493-119">2 </span><span class="sxs-lookup"><span data-stu-id="da493-119">2</span></span>|<span data-ttu-id="da493-120">Сценарий исправления успешно выполнен и исправлено состояние устройства</span><span class="sxs-lookup"><span data-stu-id="da493-120">Remediation script executed successfully and remediated the device state</span></span>|
|<span data-ttu-id="da493-121">ремедиатионфаилед</span><span class="sxs-lookup"><span data-stu-id="da493-121">remediationFailed</span></span>|<span data-ttu-id="da493-122">4</span><span class="sxs-lookup"><span data-stu-id="da493-122">3</span></span>|<span data-ttu-id="da493-123">Сценарий исправления успешно выполнен, но ему не удалось исправить состояние устройства</span><span class="sxs-lookup"><span data-stu-id="da493-123">Remediation script executed successfully but failed to remediated the device state</span></span>|
|<span data-ttu-id="da493-124">скриптеррор</span><span class="sxs-lookup"><span data-stu-id="da493-124">scriptError</span></span>|<span data-ttu-id="da493-125">4 </span><span class="sxs-lookup"><span data-stu-id="da493-125">4</span></span>|<span data-ttu-id="da493-126">Произошла ошибка или истекло время ожидания выполнения скрипта исправления</span><span class="sxs-lookup"><span data-stu-id="da493-126">Remediation script execution encountered and error or timed out</span></span>|






