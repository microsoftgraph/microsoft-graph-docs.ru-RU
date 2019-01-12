---
title: Включение тип перечисления
description: 'Значения, используемые для указания состояния устройства. '
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 539d57111003f348147a6be3952d969ab4206b5d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911961"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="49fc0-103">Включение тип перечисления</span><span class="sxs-lookup"><span data-stu-id="49fc0-103">enablement enum type</span></span>

> <span data-ttu-id="49fc0-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="49fc0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49fc0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49fc0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49fc0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="49fc0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49fc0-107">Значения, используемые для указания состояния устройства.</span><span class="sxs-lookup"><span data-stu-id="49fc0-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="49fc0-108">Обратите внимание, что существует разница между отключена и не настроена.</span><span class="sxs-lookup"><span data-stu-id="49fc0-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="49fc0-109">Элементы</span><span class="sxs-lookup"><span data-stu-id="49fc0-109">Members</span></span>
|<span data-ttu-id="49fc0-110">Элемент</span><span class="sxs-lookup"><span data-stu-id="49fc0-110">Member</span></span>|<span data-ttu-id="49fc0-111">Значение</span><span class="sxs-lookup"><span data-stu-id="49fc0-111">Value</span></span>|<span data-ttu-id="49fc0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="49fc0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49fc0-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="49fc0-113">notConfigured</span></span>|<span data-ttu-id="49fc0-114">0</span><span class="sxs-lookup"><span data-stu-id="49fc0-114">0</span></span>|<span data-ttu-id="49fc0-115">Значение по умолчанию устройства, без цели.</span><span class="sxs-lookup"><span data-stu-id="49fc0-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="49fc0-116">enabled</span><span class="sxs-lookup"><span data-stu-id="49fc0-116">enabled</span></span>|<span data-ttu-id="49fc0-117">1</span><span class="sxs-lookup"><span data-stu-id="49fc0-117">1</span></span>|<span data-ttu-id="49fc0-118">Включение параметра на устройстве.</span><span class="sxs-lookup"><span data-stu-id="49fc0-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="49fc0-119">Этот параметр отключен</span><span class="sxs-lookup"><span data-stu-id="49fc0-119">disabled</span></span>|<span data-ttu-id="49fc0-120">2</span><span class="sxs-lookup"><span data-stu-id="49fc0-120">2</span></span>|<span data-ttu-id="49fc0-121">Отключает настройку на устройстве.</span><span class="sxs-lookup"><span data-stu-id="49fc0-121">Disables the setting on the device.</span></span>|
