---
title: Тип перечисления androidDeviceOwnerSystemUpdateInstallType
description: Системные типы обновлений для Android устройства владельцем.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d7caaa3c79062bba6b8aa06ea11389e1370fba5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419179"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a><span data-ttu-id="c1c70-103">Тип перечисления androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="c1c70-103">androidDeviceOwnerSystemUpdateInstallType enum type</span></span>

> <span data-ttu-id="c1c70-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c1c70-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c1c70-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1c70-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1c70-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1c70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1c70-107">Системные типы обновлений для Android устройства владельцем.</span><span class="sxs-lookup"><span data-stu-id="c1c70-107">System Update Types for Android Device Owner.</span></span>

## <a name="members"></a><span data-ttu-id="c1c70-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="c1c70-108">Members</span></span>
|<span data-ttu-id="c1c70-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="c1c70-109">Member</span></span>|<span data-ttu-id="c1c70-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c1c70-110">Value</span></span>|<span data-ttu-id="c1c70-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c1c70-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1c70-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c1c70-112">deviceDefault</span></span>|<span data-ttu-id="c1c70-113">0</span><span class="sxs-lookup"><span data-stu-id="c1c70-113">0</span></span>|<span data-ttu-id="c1c70-114">Поведение по умолчанию устройство, которое обычно выдает запрос пользователю принимать обновления системы.</span><span class="sxs-lookup"><span data-stu-id="c1c70-114">Device default behavior, which typically prompts the user to accept system updates.</span></span>|
|<span data-ttu-id="c1c70-115">отложить</span><span class="sxs-lookup"><span data-stu-id="c1c70-115">postpone</span></span>|<span data-ttu-id="c1c70-116">1</span><span class="sxs-lookup"><span data-stu-id="c1c70-116">1</span></span>|<span data-ttu-id="c1c70-117">Отложить автоматическую установку обновлений вверх до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="c1c70-117">Postpone automatic install of updates up to 30 days.</span></span>|
|<span data-ttu-id="c1c70-118">оконного</span><span class="sxs-lookup"><span data-stu-id="c1c70-118">windowed</span></span>|<span data-ttu-id="c1c70-119">2</span><span class="sxs-lookup"><span data-stu-id="c1c70-119">2</span></span>|<span data-ttu-id="c1c70-120">Внутри ежедневного периода обслуживания автоматической установки.</span><span class="sxs-lookup"><span data-stu-id="c1c70-120">Install automatically inside a daily maintenance window.</span></span>|
|<span data-ttu-id="c1c70-121">Автоматически</span><span class="sxs-lookup"><span data-stu-id="c1c70-121">automatic</span></span>|<span data-ttu-id="c1c70-122">3</span><span class="sxs-lookup"><span data-stu-id="c1c70-122">3</span></span>|<span data-ttu-id="c1c70-123">Как можно скорее автоматическую установку обновлений.</span><span class="sxs-lookup"><span data-stu-id="c1c70-123">Automatically install updates as soon as possible.</span></span>|




