---
title: Тип перечисления runState
description: Указывает тип состояния выполнения скрипта управления устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c2178d492b7c341ffc8f5b7af85c78f46bd3f733
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956033"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="03a8f-103">Тип перечисления runState</span><span class="sxs-lookup"><span data-stu-id="03a8f-103">runState enum type</span></span>

> <span data-ttu-id="03a8f-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="03a8f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03a8f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03a8f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03a8f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="03a8f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03a8f-107">Указывает тип состояния выполнения скрипта управления устройства.</span><span class="sxs-lookup"><span data-stu-id="03a8f-107">Indicates the type of execution status of the device management script.</span></span>
## <a name="members"></a><span data-ttu-id="03a8f-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="03a8f-108">Members</span></span>
|<span data-ttu-id="03a8f-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="03a8f-109">Member</span></span>|<span data-ttu-id="03a8f-110">Значение</span><span class="sxs-lookup"><span data-stu-id="03a8f-110">Value</span></span>|<span data-ttu-id="03a8f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="03a8f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03a8f-112">unknown</span><span class="sxs-lookup"><span data-stu-id="03a8f-112">unknown</span></span>|<span data-ttu-id="03a8f-113">0</span><span class="sxs-lookup"><span data-stu-id="03a8f-113">0</span></span>|<span data-ttu-id="03a8f-114">Неизвестный результат.</span><span class="sxs-lookup"><span data-stu-id="03a8f-114">Unknown result.</span></span>|
|<span data-ttu-id="03a8f-115">success</span><span class="sxs-lookup"><span data-stu-id="03a8f-115">success</span></span>|<span data-ttu-id="03a8f-116">1</span><span class="sxs-lookup"><span data-stu-id="03a8f-116">1</span></span>|<span data-ttu-id="03a8f-117">Сценарий выполняется успешно.</span><span class="sxs-lookup"><span data-stu-id="03a8f-117">Script is run successfully.</span></span>|
|<span data-ttu-id="03a8f-118">с ошибкой</span><span class="sxs-lookup"><span data-stu-id="03a8f-118">fail</span></span>|<span data-ttu-id="03a8f-119">2</span><span class="sxs-lookup"><span data-stu-id="03a8f-119">2</span></span>|<span data-ttu-id="03a8f-120">Не удалось выполнить скрипт.</span><span class="sxs-lookup"><span data-stu-id="03a8f-120">Script failed to run.</span></span>|





