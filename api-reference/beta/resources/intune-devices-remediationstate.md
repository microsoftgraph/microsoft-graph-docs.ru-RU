---
title: тип перечисления Ремедиатионстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 49161209ad1a38123067ed3c434cbe31a3a2af70
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725430"
---
# <a name="remediationstate-enum-type"></a><span data-ttu-id="02ccd-103">тип перечисления Ремедиатионстате</span><span class="sxs-lookup"><span data-stu-id="02ccd-103">remediationState enum type</span></span>

<span data-ttu-id="02ccd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02ccd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02ccd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02ccd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02ccd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02ccd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02ccd-107">Указывает тип состояния выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="02ccd-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="02ccd-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="02ccd-108">Members</span></span>
|<span data-ttu-id="02ccd-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="02ccd-109">Member</span></span>|<span data-ttu-id="02ccd-110">Значение</span><span class="sxs-lookup"><span data-stu-id="02ccd-110">Value</span></span>|<span data-ttu-id="02ccd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="02ccd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02ccd-112">unknown</span><span class="sxs-lookup"><span data-stu-id="02ccd-112">unknown</span></span>|<span data-ttu-id="02ccd-113">нуль</span><span class="sxs-lookup"><span data-stu-id="02ccd-113">0</span></span>|<span data-ttu-id="02ccd-114">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="02ccd-114">Unknown result.</span></span>|
|<span data-ttu-id="02ccd-115">пропущенных</span><span class="sxs-lookup"><span data-stu-id="02ccd-115">skipped</span></span>|<span data-ttu-id="02ccd-116">1,1</span><span class="sxs-lookup"><span data-stu-id="02ccd-116">1</span></span>|<span data-ttu-id="02ccd-117">Выполнение скрипта исправления пропущено</span><span class="sxs-lookup"><span data-stu-id="02ccd-117">Remediation script execution was skipped</span></span>|
|<span data-ttu-id="02ccd-118">success</span><span class="sxs-lookup"><span data-stu-id="02ccd-118">success</span></span>|<span data-ttu-id="02ccd-119">2</span><span class="sxs-lookup"><span data-stu-id="02ccd-119">2</span></span>|<span data-ttu-id="02ccd-120">Сценарий исправления успешно выполнен и исправлено состояние устройства</span><span class="sxs-lookup"><span data-stu-id="02ccd-120">Remediation script executed successfully and remediated the device state</span></span>|
|<span data-ttu-id="02ccd-121">ремедиатионфаилед</span><span class="sxs-lookup"><span data-stu-id="02ccd-121">remediationFailed</span></span>|<span data-ttu-id="02ccd-122">4</span><span class="sxs-lookup"><span data-stu-id="02ccd-122">3</span></span>|<span data-ttu-id="02ccd-123">Сценарий исправления успешно выполнен, но ему не удалось исправить состояние устройства</span><span class="sxs-lookup"><span data-stu-id="02ccd-123">Remediation script executed successfully but failed to remediated the device state</span></span>|
|<span data-ttu-id="02ccd-124">скриптеррор</span><span class="sxs-lookup"><span data-stu-id="02ccd-124">scriptError</span></span>|<span data-ttu-id="02ccd-125">4 </span><span class="sxs-lookup"><span data-stu-id="02ccd-125">4</span></span>|<span data-ttu-id="02ccd-126">Произошла ошибка или истекло время ожидания выполнения скрипта исправления</span><span class="sxs-lookup"><span data-stu-id="02ccd-126">Remediation script execution encountered and error or timed out</span></span>|





