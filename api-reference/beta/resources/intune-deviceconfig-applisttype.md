---
title: Тип перечисления appListType
description: Возможные значения список соответствия требованиям приложения.
author: tfitzmac
ms.openlocfilehash: 3f0fa162131fc1f59beba1f057fa888e0f2260c5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331194"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="f8154-103">Тип перечисления appListType</span><span class="sxs-lookup"><span data-stu-id="f8154-103">appListType enum type</span></span>

> <span data-ttu-id="f8154-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f8154-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8154-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8154-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8154-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f8154-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8154-107">Возможные значения список соответствия требованиям приложения.</span><span class="sxs-lookup"><span data-stu-id="f8154-107">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="f8154-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f8154-108">Members</span></span>
|<span data-ttu-id="f8154-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f8154-109">Member</span></span>|<span data-ttu-id="f8154-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f8154-110">Value</span></span>|<span data-ttu-id="f8154-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f8154-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8154-112">none</span><span class="sxs-lookup"><span data-stu-id="f8154-112">none</span></span>|<span data-ttu-id="f8154-113">0</span><span class="sxs-lookup"><span data-stu-id="f8154-113">0</span></span>|<span data-ttu-id="f8154-114">Значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="f8154-114">Default value, no intent.</span></span>|
|<span data-ttu-id="f8154-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="f8154-115">appsInListCompliant</span></span>|<span data-ttu-id="f8154-116">1</span><span class="sxs-lookup"><span data-stu-id="f8154-116">1</span></span>|<span data-ttu-id="f8154-117">Список представляет приложений, которые будут считаться спецификации (только для приложений в списке совместимых).</span><span class="sxs-lookup"><span data-stu-id="f8154-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="f8154-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="f8154-118">appsNotInListCompliant</span></span>|<span data-ttu-id="f8154-119">2</span><span class="sxs-lookup"><span data-stu-id="f8154-119">2</span></span>|<span data-ttu-id="f8154-120">Представляет список приложений, которые будут считаться несовместимой (все приложения совместимых за исключением приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="f8154-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





