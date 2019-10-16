---
title: тип перечисления Ремедиатионстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b359842d7fb266803fdb758d32ca51e6a4b78b97
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37529090"
---
# <a name="remediationstate-enum-type"></a><span data-ttu-id="90e40-103">тип перечисления Ремедиатионстате</span><span class="sxs-lookup"><span data-stu-id="90e40-103">remediationState enum type</span></span>

> <span data-ttu-id="90e40-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90e40-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90e40-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90e40-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90e40-106">Указывает тип состояния выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="90e40-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="90e40-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="90e40-107">Members</span></span>
|<span data-ttu-id="90e40-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="90e40-108">Member</span></span>|<span data-ttu-id="90e40-109">Значение</span><span class="sxs-lookup"><span data-stu-id="90e40-109">Value</span></span>|<span data-ttu-id="90e40-110">Описание</span><span class="sxs-lookup"><span data-stu-id="90e40-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90e40-111">unknown</span><span class="sxs-lookup"><span data-stu-id="90e40-111">unknown</span></span>|<span data-ttu-id="90e40-112">нуль</span><span class="sxs-lookup"><span data-stu-id="90e40-112">0</span></span>|<span data-ttu-id="90e40-113">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="90e40-113">Unknown result.</span></span>|
|<span data-ttu-id="90e40-114">пропущенных</span><span class="sxs-lookup"><span data-stu-id="90e40-114">skipped</span></span>|<span data-ttu-id="90e40-115">1,1</span><span class="sxs-lookup"><span data-stu-id="90e40-115">1</span></span>|<span data-ttu-id="90e40-116">Выполнение скрипта исправления пропущено</span><span class="sxs-lookup"><span data-stu-id="90e40-116">Remediation script execution was skipped</span></span>|
|<span data-ttu-id="90e40-117">success</span><span class="sxs-lookup"><span data-stu-id="90e40-117">success</span></span>|<span data-ttu-id="90e40-118">2</span><span class="sxs-lookup"><span data-stu-id="90e40-118">2</span></span>|<span data-ttu-id="90e40-119">Сценарий исправления успешно выполнен и исправлено состояние устройства</span><span class="sxs-lookup"><span data-stu-id="90e40-119">Remediation script executed successfully and remediated the device state</span></span>|
|<span data-ttu-id="90e40-120">ремедиатионфаилед</span><span class="sxs-lookup"><span data-stu-id="90e40-120">remediationFailed</span></span>|<span data-ttu-id="90e40-121">4</span><span class="sxs-lookup"><span data-stu-id="90e40-121">3</span></span>|<span data-ttu-id="90e40-122">Сценарий исправления успешно выполнен, но ему не удалось исправить состояние устройства</span><span class="sxs-lookup"><span data-stu-id="90e40-122">Remediation script executed successfully but failed to remediated the device state</span></span>|
|<span data-ttu-id="90e40-123">скриптеррор</span><span class="sxs-lookup"><span data-stu-id="90e40-123">scriptError</span></span>|<span data-ttu-id="90e40-124">4 </span><span class="sxs-lookup"><span data-stu-id="90e40-124">4</span></span>|<span data-ttu-id="90e40-125">Произошла ошибка или истекло время ожидания выполнения скрипта исправления</span><span class="sxs-lookup"><span data-stu-id="90e40-125">Remediation script execution encountered and error or timed out</span></span>|



