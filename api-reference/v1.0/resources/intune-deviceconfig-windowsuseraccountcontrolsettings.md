---
title: Тип перечисления windowsUserAccountControlSettings
description: Возможные значения для параметров контроля учетных записей пользователей Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0475d8fb013cbb07f8d69a659f8ecde2eb580e43
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972476"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="3c014-103">Тип перечисления windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="3c014-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="3c014-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3c014-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c014-105">Возможные значения для параметров контроля учетных записей пользователей Windows.</span><span class="sxs-lookup"><span data-stu-id="3c014-105">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="3c014-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="3c014-106">Members</span></span>
|<span data-ttu-id="3c014-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="3c014-107">Member</span></span>|<span data-ttu-id="3c014-108">Значение</span><span class="sxs-lookup"><span data-stu-id="3c014-108">Value</span></span>|<span data-ttu-id="3c014-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3c014-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c014-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="3c014-110">userDefined</span></span>|<span data-ttu-id="3c014-111">0</span><span class="sxs-lookup"><span data-stu-id="3c014-111">0</span></span>|<span data-ttu-id="3c014-112">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="3c014-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="3c014-113">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="3c014-113">alwaysNotify</span></span>|<span data-ttu-id="3c014-114">1</span><span class="sxs-lookup"><span data-stu-id="3c014-114">1</span></span>|<span data-ttu-id="3c014-115">Всегда уведомите.</span><span class="sxs-lookup"><span data-stu-id="3c014-115">Always notify.</span></span>|
|<span data-ttu-id="3c014-116">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="3c014-116">notifyOnAppChanges</span></span>|<span data-ttu-id="3c014-117">2</span><span class="sxs-lookup"><span data-stu-id="3c014-117">2</span></span>|<span data-ttu-id="3c014-118">Уведомление об изменениях приложения.</span><span class="sxs-lookup"><span data-stu-id="3c014-118">Notify on app changes.</span></span>|
|<span data-ttu-id="3c014-119">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="3c014-119">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="3c014-120">3</span><span class="sxs-lookup"><span data-stu-id="3c014-120">3</span></span>|<span data-ttu-id="3c014-121">Уведомления на изменения в приложении без затемнение рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="3c014-121">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="3c014-122">neverNotify</span><span class="sxs-lookup"><span data-stu-id="3c014-122">neverNotify</span></span>|<span data-ttu-id="3c014-123">4</span><span class="sxs-lookup"><span data-stu-id="3c014-123">4</span></span>|<span data-ttu-id="3c014-124">Никогда не уведомлять.</span><span class="sxs-lookup"><span data-stu-id="3c014-124">Never notify.</span></span>|



