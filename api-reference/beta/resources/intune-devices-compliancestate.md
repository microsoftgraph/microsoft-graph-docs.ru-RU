---
title: Тип перечисления complianceState
description: Состояние соответствия требованиям.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 04f77da451970a302dbf249e8820aa5a2a8f0ebc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392740"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="54021-103">Тип перечисления complianceState</span><span class="sxs-lookup"><span data-stu-id="54021-103">complianceState enum type</span></span>

> <span data-ttu-id="54021-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="54021-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="54021-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54021-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54021-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54021-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54021-107">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="54021-107">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="54021-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="54021-108">Members</span></span>
|<span data-ttu-id="54021-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="54021-109">Member</span></span>|<span data-ttu-id="54021-110">Значение</span><span class="sxs-lookup"><span data-stu-id="54021-110">Value</span></span>|<span data-ttu-id="54021-111">Описание</span><span class="sxs-lookup"><span data-stu-id="54021-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54021-112">unknown</span><span class="sxs-lookup"><span data-stu-id="54021-112">unknown</span></span>|<span data-ttu-id="54021-113">0</span><span class="sxs-lookup"><span data-stu-id="54021-113">0</span></span>|<span data-ttu-id="54021-114">Неизвестно.</span><span class="sxs-lookup"><span data-stu-id="54021-114">Unknown.</span></span>|
|<span data-ttu-id="54021-115">спецификации</span><span class="sxs-lookup"><span data-stu-id="54021-115">compliant</span></span>|<span data-ttu-id="54021-116">1</span><span class="sxs-lookup"><span data-stu-id="54021-116">1</span></span>|<span data-ttu-id="54021-117">Спецификации.</span><span class="sxs-lookup"><span data-stu-id="54021-117">Compliant.</span></span>|
|<span data-ttu-id="54021-118">несовместимый</span><span class="sxs-lookup"><span data-stu-id="54021-118">noncompliant</span></span>|<span data-ttu-id="54021-119">2</span><span class="sxs-lookup"><span data-stu-id="54021-119">2</span></span>|<span data-ttu-id="54021-120">Устройство не соответствует спецификации и запретом корпоративным ресурсам.</span><span class="sxs-lookup"><span data-stu-id="54021-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="54021-121">конфликта</span><span class="sxs-lookup"><span data-stu-id="54021-121">conflict</span></span>|<span data-ttu-id="54021-122">3</span><span class="sxs-lookup"><span data-stu-id="54021-122">3</span></span>|<span data-ttu-id="54021-123">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="54021-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="54021-124">error</span><span class="sxs-lookup"><span data-stu-id="54021-124">error</span></span>|<span data-ttu-id="54021-125">4</span><span class="sxs-lookup"><span data-stu-id="54021-125">4</span></span>|<span data-ttu-id="54021-126">Ошибка</span><span class="sxs-lookup"><span data-stu-id="54021-126">Error.</span></span>|
|<span data-ttu-id="54021-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="54021-127">inGracePeriod</span></span>|<span data-ttu-id="54021-128">254</span><span class="sxs-lookup"><span data-stu-id="54021-128">254</span></span>|<span data-ttu-id="54021-129">Устройство, не соответствует спецификации, но по-прежнему имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="54021-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="54021-130">configManager</span><span class="sxs-lookup"><span data-stu-id="54021-130">configManager</span></span>|<span data-ttu-id="54021-131">255</span><span class="sxs-lookup"><span data-stu-id="54021-131">255</span></span>|<span data-ttu-id="54021-132">Управляет диспетчер конфигурации</span><span class="sxs-lookup"><span data-stu-id="54021-132">Managed by Config Manager</span></span>|




