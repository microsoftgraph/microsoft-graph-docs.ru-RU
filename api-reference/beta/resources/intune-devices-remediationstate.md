---
title: тип перечисления Ремедиатионстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: cd940bbe2256baa7954e67ba9469ac00740f4ad1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783916"
---
# <a name="remediationstate-enum-type"></a><span data-ttu-id="6543c-103">тип перечисления Ремедиатионстате</span><span class="sxs-lookup"><span data-stu-id="6543c-103">remediationState enum type</span></span>

> <span data-ttu-id="6543c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6543c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6543c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6543c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6543c-106">Указывает тип состояния выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="6543c-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="6543c-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="6543c-107">Members</span></span>
|<span data-ttu-id="6543c-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="6543c-108">Member</span></span>|<span data-ttu-id="6543c-109">Значение</span><span class="sxs-lookup"><span data-stu-id="6543c-109">Value</span></span>|<span data-ttu-id="6543c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6543c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6543c-111">unknown</span><span class="sxs-lookup"><span data-stu-id="6543c-111">unknown</span></span>|<span data-ttu-id="6543c-112">нуль</span><span class="sxs-lookup"><span data-stu-id="6543c-112">0</span></span>|<span data-ttu-id="6543c-113">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="6543c-113">Unknown result.</span></span>|
|<span data-ttu-id="6543c-114">пропущенных</span><span class="sxs-lookup"><span data-stu-id="6543c-114">skipped</span></span>|<span data-ttu-id="6543c-115">1,1</span><span class="sxs-lookup"><span data-stu-id="6543c-115">1</span></span>|<span data-ttu-id="6543c-116">Выполнение скрипта исправления пропущено</span><span class="sxs-lookup"><span data-stu-id="6543c-116">Remediation script execution was skipped</span></span>|
|<span data-ttu-id="6543c-117">success</span><span class="sxs-lookup"><span data-stu-id="6543c-117">success</span></span>|<span data-ttu-id="6543c-118">2</span><span class="sxs-lookup"><span data-stu-id="6543c-118">2</span></span>|<span data-ttu-id="6543c-119">Сценарий исправления успешно выполнен и исправлено состояние устройства</span><span class="sxs-lookup"><span data-stu-id="6543c-119">Remediation script executed successfully and remediated the device state</span></span>|
|<span data-ttu-id="6543c-120">ремедиатионфаилед</span><span class="sxs-lookup"><span data-stu-id="6543c-120">remediationFailed</span></span>|<span data-ttu-id="6543c-121">4</span><span class="sxs-lookup"><span data-stu-id="6543c-121">3</span></span>|<span data-ttu-id="6543c-122">Сценарий исправления успешно выполнен, но ему не удалось исправить состояние устройства</span><span class="sxs-lookup"><span data-stu-id="6543c-122">Remediation script executed successfully but failed to remediated the device state</span></span>|
|<span data-ttu-id="6543c-123">скриптеррор</span><span class="sxs-lookup"><span data-stu-id="6543c-123">scriptError</span></span>|<span data-ttu-id="6543c-124">4 </span><span class="sxs-lookup"><span data-stu-id="6543c-124">4</span></span>|<span data-ttu-id="6543c-125">Произошла ошибка или истекло время ожидания выполнения скрипта исправления</span><span class="sxs-lookup"><span data-stu-id="6543c-125">Remediation script execution encountered and error or timed out</span></span>|



