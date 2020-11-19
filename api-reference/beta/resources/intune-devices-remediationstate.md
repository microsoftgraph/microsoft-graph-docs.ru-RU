---
title: тип перечисления Ремедиатионстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 90e930d6b8955671abb494839bafe6cac16438f0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49230879"
---
# <a name="remediationstate-enum-type"></a><span data-ttu-id="d8b5c-103">тип перечисления Ремедиатионстате</span><span class="sxs-lookup"><span data-stu-id="d8b5c-103">remediationState enum type</span></span>

<span data-ttu-id="d8b5c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8b5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8b5c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8b5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8b5c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8b5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8b5c-107">Указывает тип состояния выполнения скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="d8b5c-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="d8b5c-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="d8b5c-108">Members</span></span>
|<span data-ttu-id="d8b5c-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="d8b5c-109">Member</span></span>|<span data-ttu-id="d8b5c-110">Значение</span><span class="sxs-lookup"><span data-stu-id="d8b5c-110">Value</span></span>|<span data-ttu-id="d8b5c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d8b5c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8b5c-112">unknown</span><span class="sxs-lookup"><span data-stu-id="d8b5c-112">unknown</span></span>|<span data-ttu-id="d8b5c-113">нуль</span><span class="sxs-lookup"><span data-stu-id="d8b5c-113">0</span></span>|<span data-ttu-id="d8b5c-114">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="d8b5c-114">Unknown result.</span></span>|
|<span data-ttu-id="d8b5c-115">пропущенных</span><span class="sxs-lookup"><span data-stu-id="d8b5c-115">skipped</span></span>|<span data-ttu-id="d8b5c-116">1,1</span><span class="sxs-lookup"><span data-stu-id="d8b5c-116">1</span></span>|<span data-ttu-id="d8b5c-117">Выполнение скрипта исправления пропущено</span><span class="sxs-lookup"><span data-stu-id="d8b5c-117">Remediation script execution was skipped</span></span>|
|<span data-ttu-id="d8b5c-118">success</span><span class="sxs-lookup"><span data-stu-id="d8b5c-118">success</span></span>|<span data-ttu-id="d8b5c-119">2</span><span class="sxs-lookup"><span data-stu-id="d8b5c-119">2</span></span>|<span data-ttu-id="d8b5c-120">Сценарий исправления успешно выполнен и исправлено состояние устройства</span><span class="sxs-lookup"><span data-stu-id="d8b5c-120">Remediation script executed successfully and remediated the device state</span></span>|
|<span data-ttu-id="d8b5c-121">ремедиатионфаилед</span><span class="sxs-lookup"><span data-stu-id="d8b5c-121">remediationFailed</span></span>|<span data-ttu-id="d8b5c-122">4</span><span class="sxs-lookup"><span data-stu-id="d8b5c-122">3</span></span>|<span data-ttu-id="d8b5c-123">Сценарий исправления успешно выполнен, но ему не удалось исправить состояние устройства</span><span class="sxs-lookup"><span data-stu-id="d8b5c-123">Remediation script executed successfully but failed to remediated the device state</span></span>|
|<span data-ttu-id="d8b5c-124">скриптеррор</span><span class="sxs-lookup"><span data-stu-id="d8b5c-124">scriptError</span></span>|<span data-ttu-id="d8b5c-125">4 </span><span class="sxs-lookup"><span data-stu-id="d8b5c-125">4</span></span>|<span data-ttu-id="d8b5c-126">Произошла ошибка или истекло время ожидания выполнения скрипта исправления</span><span class="sxs-lookup"><span data-stu-id="d8b5c-126">Remediation script execution encountered and error or timed out</span></span>|




