---
title: тип перечисления Ремедиатионстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dc2be0c860ba142f59bba05a2a0c5ae0105c0ab1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528517"
---
# <a name="remediationstate-enum-type"></a><span data-ttu-id="dd2c6-103">тип перечисления Ремедиатионстате</span><span class="sxs-lookup"><span data-stu-id="dd2c6-103">remediationState enum type</span></span>

<span data-ttu-id="dd2c6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dd2c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd2c6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd2c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd2c6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd2c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd2c6-107">Указывает тип состояния выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="dd2c6-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="dd2c6-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="dd2c6-108">Members</span></span>
|<span data-ttu-id="dd2c6-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="dd2c6-109">Member</span></span>|<span data-ttu-id="dd2c6-110">Значение</span><span class="sxs-lookup"><span data-stu-id="dd2c6-110">Value</span></span>|<span data-ttu-id="dd2c6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dd2c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd2c6-112">unknown</span><span class="sxs-lookup"><span data-stu-id="dd2c6-112">unknown</span></span>|<span data-ttu-id="dd2c6-113">нуль</span><span class="sxs-lookup"><span data-stu-id="dd2c6-113">0</span></span>|<span data-ttu-id="dd2c6-114">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="dd2c6-114">Unknown result.</span></span>|
|<span data-ttu-id="dd2c6-115">пропущенных</span><span class="sxs-lookup"><span data-stu-id="dd2c6-115">skipped</span></span>|<span data-ttu-id="dd2c6-116">1 </span><span class="sxs-lookup"><span data-stu-id="dd2c6-116">1</span></span>|<span data-ttu-id="dd2c6-117">Выполнение скрипта исправления пропущено</span><span class="sxs-lookup"><span data-stu-id="dd2c6-117">Remediation script execution was skipped</span></span>|
|<span data-ttu-id="dd2c6-118">success</span><span class="sxs-lookup"><span data-stu-id="dd2c6-118">success</span></span>|<span data-ttu-id="dd2c6-119">2 </span><span class="sxs-lookup"><span data-stu-id="dd2c6-119">2</span></span>|<span data-ttu-id="dd2c6-120">Сценарий исправления успешно выполнен и исправлено состояние устройства</span><span class="sxs-lookup"><span data-stu-id="dd2c6-120">Remediation script executed successfully and remediated the device state</span></span>|
|<span data-ttu-id="dd2c6-121">ремедиатионфаилед</span><span class="sxs-lookup"><span data-stu-id="dd2c6-121">remediationFailed</span></span>|<span data-ttu-id="dd2c6-122">3 </span><span class="sxs-lookup"><span data-stu-id="dd2c6-122">3</span></span>|<span data-ttu-id="dd2c6-123">Сценарий исправления успешно выполнен, но ему не удалось исправить состояние устройства</span><span class="sxs-lookup"><span data-stu-id="dd2c6-123">Remediation script executed successfully but failed to remediated the device state</span></span>|
|<span data-ttu-id="dd2c6-124">скриптеррор</span><span class="sxs-lookup"><span data-stu-id="dd2c6-124">scriptError</span></span>|<span data-ttu-id="dd2c6-125">4 </span><span class="sxs-lookup"><span data-stu-id="dd2c6-125">4</span></span>|<span data-ttu-id="dd2c6-126">Произошла ошибка или истекло время ожидания выполнения скрипта исправления</span><span class="sxs-lookup"><span data-stu-id="dd2c6-126">Remediation script execution encountered and error or timed out</span></span>|



