---
title: Тип перечисления windowsSModeConfiguration
description: Возможные варианты для настройки режима S разблокировки
author: tfitzmac
ms.openlocfilehash: 592eb58a13d1f78caadb5b46acac5b43e6c97384
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344704"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="2f520-103">Тип перечисления windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f520-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="2f520-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2f520-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f520-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f520-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f520-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2f520-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f520-107">Возможные варианты для настройки режима S разблокировки</span><span class="sxs-lookup"><span data-stu-id="2f520-107">The possible options to configure S mode unlock</span></span>
## <a name="members"></a><span data-ttu-id="2f520-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="2f520-108">Members</span></span>
|<span data-ttu-id="2f520-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="2f520-109">Member</span></span>|<span data-ttu-id="2f520-110">Значение</span><span class="sxs-lookup"><span data-stu-id="2f520-110">Value</span></span>|<span data-ttu-id="2f520-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2f520-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f520-112">noRestriction</span><span class="sxs-lookup"><span data-stu-id="2f520-112">noRestriction</span></span>|<span data-ttu-id="2f520-113">0</span><span class="sxs-lookup"><span data-stu-id="2f520-113">0</span></span>|<span data-ttu-id="2f520-114">Этот параметр удаляет все ограничения для разблокировки режим S - по умолчанию</span><span class="sxs-lookup"><span data-stu-id="2f520-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="2f520-115">блок</span><span class="sxs-lookup"><span data-stu-id="2f520-115">block</span></span>|<span data-ttu-id="2f520-116">1</span><span class="sxs-lookup"><span data-stu-id="2f520-116">1</span></span>|<span data-ttu-id="2f520-117">Этот параметр, будет блокировать пользователя для разблокировки устройства из режима S</span><span class="sxs-lookup"><span data-stu-id="2f520-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="2f520-118">Снятие блокировки</span><span class="sxs-lookup"><span data-stu-id="2f520-118">unlock</span></span>|<span data-ttu-id="2f520-119">2</span><span class="sxs-lookup"><span data-stu-id="2f520-119">2</span></span>|<span data-ttu-id="2f520-120">Этот параметр используется для открытия устройства из режима S</span><span class="sxs-lookup"><span data-stu-id="2f520-120">This option will unlock the device from S mode</span></span>|





