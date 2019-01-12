---
title: Тип перечисления sharedPCAccountDeletionPolicyType
description: Возможные значения для при удалении учетных записей на общую ПК.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 081069f9462c426f24a1e3cf276730b1db40b191
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951952"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="0ee28-103">Тип перечисления sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="0ee28-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="0ee28-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0ee28-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ee28-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ee28-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ee28-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0ee28-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ee28-107">Возможные значения для при удалении учетных записей на общую ПК.</span><span class="sxs-lookup"><span data-stu-id="0ee28-107">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="0ee28-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0ee28-108">Members</span></span>
|<span data-ttu-id="0ee28-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0ee28-109">Member</span></span>|<span data-ttu-id="0ee28-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0ee28-110">Value</span></span>|<span data-ttu-id="0ee28-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0ee28-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ee28-112">Интерпретация</span><span class="sxs-lookup"><span data-stu-id="0ee28-112">immediate</span></span>|<span data-ttu-id="0ee28-113">0</span><span class="sxs-lookup"><span data-stu-id="0ee28-113">0</span></span>|<span data-ttu-id="0ee28-114">Удаление немедленно.</span><span class="sxs-lookup"><span data-stu-id="0ee28-114">Delete immediately.</span></span>|
|<span data-ttu-id="0ee28-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="0ee28-115">diskSpaceThreshold</span></span>|<span data-ttu-id="0ee28-116">1</span><span class="sxs-lookup"><span data-stu-id="0ee28-116">1</span></span>|<span data-ttu-id="0ee28-117">Удалите в порога места на диске.</span><span class="sxs-lookup"><span data-stu-id="0ee28-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="0ee28-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="0ee28-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="0ee28-119">2</span><span class="sxs-lookup"><span data-stu-id="0ee28-119">2</span></span>|<span data-ttu-id="0ee28-120">Удалите порога места на диске, так и неактивных пороговое значение.</span><span class="sxs-lookup"><span data-stu-id="0ee28-120">Delete at disk space threshold or inactive threshold.</span></span>|





