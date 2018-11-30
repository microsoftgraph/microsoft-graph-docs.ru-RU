---
title: Тип перечисления appListType
description: Возможные значения список соответствия требованиям приложения.
ms.openlocfilehash: 2733723252f3b8f03cf08fda6d0b09f207ae5550
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028151"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="c64d3-103">Тип перечисления appListType</span><span class="sxs-lookup"><span data-stu-id="c64d3-103">appListType enum type</span></span>

> <span data-ttu-id="c64d3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c64d3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c64d3-105">Возможные значения список соответствия требованиям приложения.</span><span class="sxs-lookup"><span data-stu-id="c64d3-105">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="c64d3-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="c64d3-106">Members</span></span>
|<span data-ttu-id="c64d3-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="c64d3-107">Member</span></span>|<span data-ttu-id="c64d3-108">Значение</span><span class="sxs-lookup"><span data-stu-id="c64d3-108">Value</span></span>|<span data-ttu-id="c64d3-109">Description</span><span class="sxs-lookup"><span data-stu-id="c64d3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c64d3-110">Нет</span><span class="sxs-lookup"><span data-stu-id="c64d3-110">none</span></span>|<span data-ttu-id="c64d3-111">0</span><span class="sxs-lookup"><span data-stu-id="c64d3-111">0</span></span>|<span data-ttu-id="c64d3-112">Значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="c64d3-112">Default value, no intent.</span></span>|
|<span data-ttu-id="c64d3-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="c64d3-113">appsInListCompliant</span></span>|<span data-ttu-id="c64d3-114">1</span><span class="sxs-lookup"><span data-stu-id="c64d3-114">1</span></span>|<span data-ttu-id="c64d3-115">Список представляет приложений, которые будут считаться спецификации (только для приложений в списке совместимых).</span><span class="sxs-lookup"><span data-stu-id="c64d3-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="c64d3-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="c64d3-116">appsNotInListCompliant</span></span>|<span data-ttu-id="c64d3-117">2</span><span class="sxs-lookup"><span data-stu-id="c64d3-117">2</span></span>|<span data-ttu-id="c64d3-118">Представляет список приложений, которые будут считаться несовместимой (все приложения совместимых за исключением приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="c64d3-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



