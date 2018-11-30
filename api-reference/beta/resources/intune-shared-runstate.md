---
title: Тип перечисления runState
description: Указывает тип состояния выполнения скрипта управления устройства.
ms.openlocfilehash: 74802b347d83db0785c5c132315071024d944ddc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074592"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="3ed10-103">Тип перечисления runState</span><span class="sxs-lookup"><span data-stu-id="3ed10-103">runState enum type</span></span>

> <span data-ttu-id="3ed10-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3ed10-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ed10-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ed10-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ed10-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3ed10-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ed10-107">Указывает тип состояния выполнения скрипта управления устройства.</span><span class="sxs-lookup"><span data-stu-id="3ed10-107">Indicates the type of execution status of the device management script.</span></span>
## <a name="members"></a><span data-ttu-id="3ed10-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="3ed10-108">Members</span></span>
|<span data-ttu-id="3ed10-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="3ed10-109">Member</span></span>|<span data-ttu-id="3ed10-110">Значение</span><span class="sxs-lookup"><span data-stu-id="3ed10-110">Value</span></span>|<span data-ttu-id="3ed10-111">Description</span><span class="sxs-lookup"><span data-stu-id="3ed10-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ed10-112">unknown</span><span class="sxs-lookup"><span data-stu-id="3ed10-112">unknown</span></span>|<span data-ttu-id="3ed10-113">0</span><span class="sxs-lookup"><span data-stu-id="3ed10-113">0</span></span>|<span data-ttu-id="3ed10-114">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="3ed10-114">Unknown result.</span></span>|
|<span data-ttu-id="3ed10-115">success</span><span class="sxs-lookup"><span data-stu-id="3ed10-115">success</span></span>|<span data-ttu-id="3ed10-116">1</span><span class="sxs-lookup"><span data-stu-id="3ed10-116">1</span></span>|<span data-ttu-id="3ed10-117">Сценарий выполняется успешно.</span><span class="sxs-lookup"><span data-stu-id="3ed10-117">Script is run successfully.</span></span>|
|<span data-ttu-id="3ed10-118">с ошибкой</span><span class="sxs-lookup"><span data-stu-id="3ed10-118">fail</span></span>|<span data-ttu-id="3ed10-119">2</span><span class="sxs-lookup"><span data-stu-id="3ed10-119">2</span></span>|<span data-ttu-id="3ed10-120">Не удалось выполнить скрипт.</span><span class="sxs-lookup"><span data-stu-id="3ed10-120">Script failed to run.</span></span>|





