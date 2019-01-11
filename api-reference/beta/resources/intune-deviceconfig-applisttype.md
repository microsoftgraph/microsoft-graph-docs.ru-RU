---
title: Тип перечисления appListType
description: Возможные значения список соответствия требованиям приложения.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 17452d09976d84f19ed56bbaeb4e558a727b1c7c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841022"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="ee996-103">Тип перечисления appListType</span><span class="sxs-lookup"><span data-stu-id="ee996-103">appListType enum type</span></span>

> <span data-ttu-id="ee996-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ee996-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee996-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee996-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee996-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ee996-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee996-107">Возможные значения список соответствия требованиям приложения.</span><span class="sxs-lookup"><span data-stu-id="ee996-107">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="ee996-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ee996-108">Members</span></span>
|<span data-ttu-id="ee996-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ee996-109">Member</span></span>|<span data-ttu-id="ee996-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ee996-110">Value</span></span>|<span data-ttu-id="ee996-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ee996-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee996-112">Нет</span><span class="sxs-lookup"><span data-stu-id="ee996-112">none</span></span>|<span data-ttu-id="ee996-113">0</span><span class="sxs-lookup"><span data-stu-id="ee996-113">0</span></span>|<span data-ttu-id="ee996-114">Значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="ee996-114">Default value, no intent.</span></span>|
|<span data-ttu-id="ee996-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="ee996-115">appsInListCompliant</span></span>|<span data-ttu-id="ee996-116">1</span><span class="sxs-lookup"><span data-stu-id="ee996-116">1</span></span>|<span data-ttu-id="ee996-117">Список представляет приложений, которые будут считаться спецификации (только для приложений в списке совместимых).</span><span class="sxs-lookup"><span data-stu-id="ee996-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="ee996-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="ee996-118">appsNotInListCompliant</span></span>|<span data-ttu-id="ee996-119">2</span><span class="sxs-lookup"><span data-stu-id="ee996-119">2</span></span>|<span data-ttu-id="ee996-120">Представляет список приложений, которые будут считаться несовместимой (все приложения совместимых за исключением приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="ee996-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





