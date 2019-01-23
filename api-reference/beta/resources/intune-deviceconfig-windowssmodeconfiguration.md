---
title: Тип перечисления windowsSModeConfiguration
description: Возможные варианты для настройки режима S разблокировки
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 858be5b3a55fbbf4454aa576785ba793f501079c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415469"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="b3bb5-103">Тип перечисления windowsSModeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3bb5-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="b3bb5-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b3bb5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b3bb5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3bb5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3bb5-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3bb5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3bb5-107">Возможные варианты для настройки режима S разблокировки</span><span class="sxs-lookup"><span data-stu-id="b3bb5-107">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="b3bb5-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b3bb5-108">Members</span></span>
|<span data-ttu-id="b3bb5-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b3bb5-109">Member</span></span>|<span data-ttu-id="b3bb5-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b3bb5-110">Value</span></span>|<span data-ttu-id="b3bb5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b3bb5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3bb5-112">noRestriction</span><span class="sxs-lookup"><span data-stu-id="b3bb5-112">noRestriction</span></span>|<span data-ttu-id="b3bb5-113">0</span><span class="sxs-lookup"><span data-stu-id="b3bb5-113">0</span></span>|<span data-ttu-id="b3bb5-114">Этот параметр удаляет все ограничения для разблокировки режим S - по умолчанию</span><span class="sxs-lookup"><span data-stu-id="b3bb5-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="b3bb5-115">блок</span><span class="sxs-lookup"><span data-stu-id="b3bb5-115">block</span></span>|<span data-ttu-id="b3bb5-116">1</span><span class="sxs-lookup"><span data-stu-id="b3bb5-116">1</span></span>|<span data-ttu-id="b3bb5-117">Этот параметр, будет блокировать пользователя для разблокировки устройства из режима S</span><span class="sxs-lookup"><span data-stu-id="b3bb5-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="b3bb5-118">Снятие блокировки</span><span class="sxs-lookup"><span data-stu-id="b3bb5-118">unlock</span></span>|<span data-ttu-id="b3bb5-119">2</span><span class="sxs-lookup"><span data-stu-id="b3bb5-119">2</span></span>|<span data-ttu-id="b3bb5-120">Этот параметр используется для открытия устройства из режима S</span><span class="sxs-lookup"><span data-stu-id="b3bb5-120">This option will unlock the device from S mode</span></span>|




