---
title: Тип перечисления windowsUserAccountControlSettings
description: Возможные значения для параметров контроля учетных записей пользователей Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cd16db4236096687ddcc9f169dd657c938fd6815
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911814"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="37c23-103">Тип перечисления windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="37c23-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="37c23-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="37c23-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37c23-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37c23-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37c23-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="37c23-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37c23-107">Возможные значения для параметров контроля учетных записей пользователей Windows.</span><span class="sxs-lookup"><span data-stu-id="37c23-107">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="37c23-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="37c23-108">Members</span></span>
|<span data-ttu-id="37c23-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="37c23-109">Member</span></span>|<span data-ttu-id="37c23-110">Значение</span><span class="sxs-lookup"><span data-stu-id="37c23-110">Value</span></span>|<span data-ttu-id="37c23-111">Описание</span><span class="sxs-lookup"><span data-stu-id="37c23-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37c23-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="37c23-112">userDefined</span></span>|<span data-ttu-id="37c23-113">0</span><span class="sxs-lookup"><span data-stu-id="37c23-113">0</span></span>|<span data-ttu-id="37c23-114">User Defined, значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="37c23-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="37c23-115">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="37c23-115">alwaysNotify</span></span>|<span data-ttu-id="37c23-116">1</span><span class="sxs-lookup"><span data-stu-id="37c23-116">1</span></span>|<span data-ttu-id="37c23-117">Всегда уведомите.</span><span class="sxs-lookup"><span data-stu-id="37c23-117">Always notify.</span></span>|
|<span data-ttu-id="37c23-118">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="37c23-118">notifyOnAppChanges</span></span>|<span data-ttu-id="37c23-119">2</span><span class="sxs-lookup"><span data-stu-id="37c23-119">2</span></span>|<span data-ttu-id="37c23-120">Уведомление об изменениях приложения.</span><span class="sxs-lookup"><span data-stu-id="37c23-120">Notify on app changes.</span></span>|
|<span data-ttu-id="37c23-121">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="37c23-121">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="37c23-122">3</span><span class="sxs-lookup"><span data-stu-id="37c23-122">3</span></span>|<span data-ttu-id="37c23-123">Уведомления на изменения в приложении без затемнение рабочего стола.</span><span class="sxs-lookup"><span data-stu-id="37c23-123">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="37c23-124">neverNotify</span><span class="sxs-lookup"><span data-stu-id="37c23-124">neverNotify</span></span>|<span data-ttu-id="37c23-125">4</span><span class="sxs-lookup"><span data-stu-id="37c23-125">4</span></span>|<span data-ttu-id="37c23-126">Никогда не уведомлять.</span><span class="sxs-lookup"><span data-stu-id="37c23-126">Never notify.</span></span>|





