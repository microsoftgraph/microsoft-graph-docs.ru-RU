---
title: Включение тип перечисления
description: 'Значения, используемые для указания состояния устройства. '
ms.openlocfilehash: 5e72df98d33a7d3502dae4bc369781b69bc6aeb0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078437"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="17cad-103">Включение тип перечисления</span><span class="sxs-lookup"><span data-stu-id="17cad-103">enablement enum type</span></span>

> <span data-ttu-id="17cad-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="17cad-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17cad-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17cad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17cad-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="17cad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17cad-107">Значения, используемые для указания состояния устройства.</span><span class="sxs-lookup"><span data-stu-id="17cad-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="17cad-108">Обратите внимание, что существует разница между отключена и не настроена.</span><span class="sxs-lookup"><span data-stu-id="17cad-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="17cad-109">Элементы</span><span class="sxs-lookup"><span data-stu-id="17cad-109">Members</span></span>
|<span data-ttu-id="17cad-110">Элемент</span><span class="sxs-lookup"><span data-stu-id="17cad-110">Member</span></span>|<span data-ttu-id="17cad-111">Значение</span><span class="sxs-lookup"><span data-stu-id="17cad-111">Value</span></span>|<span data-ttu-id="17cad-112">Description</span><span class="sxs-lookup"><span data-stu-id="17cad-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17cad-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="17cad-113">notConfigured</span></span>|<span data-ttu-id="17cad-114">0</span><span class="sxs-lookup"><span data-stu-id="17cad-114">0</span></span>|<span data-ttu-id="17cad-115">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="17cad-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="17cad-116">enabled</span><span class="sxs-lookup"><span data-stu-id="17cad-116">enabled</span></span>|<span data-ttu-id="17cad-117">1</span><span class="sxs-lookup"><span data-stu-id="17cad-117">1</span></span>|<span data-ttu-id="17cad-118">Включение параметра на устройстве.</span><span class="sxs-lookup"><span data-stu-id="17cad-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="17cad-119">Этот параметр отключен</span><span class="sxs-lookup"><span data-stu-id="17cad-119">disabled</span></span>|<span data-ttu-id="17cad-120">2</span><span class="sxs-lookup"><span data-stu-id="17cad-120">2</span></span>|<span data-ttu-id="17cad-121">Отключает настройку на устройстве.</span><span class="sxs-lookup"><span data-stu-id="17cad-121">Disables the setting on the device.</span></span>|
