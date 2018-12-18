---
title: Тип перечисления appListType
description: Возможные значения список соответствия требованиям приложения.
author: tfitzmac
ms.openlocfilehash: ab5d8f45343b017693906b13be25c88d5b06e8f7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354721"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="dd0ec-103">Тип перечисления appListType</span><span class="sxs-lookup"><span data-stu-id="dd0ec-103">appListType enum type</span></span>

> <span data-ttu-id="dd0ec-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dd0ec-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd0ec-105">Возможные значения список соответствия требованиям приложения.</span><span class="sxs-lookup"><span data-stu-id="dd0ec-105">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="dd0ec-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="dd0ec-106">Members</span></span>
|<span data-ttu-id="dd0ec-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="dd0ec-107">Member</span></span>|<span data-ttu-id="dd0ec-108">Значение</span><span class="sxs-lookup"><span data-stu-id="dd0ec-108">Value</span></span>|<span data-ttu-id="dd0ec-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dd0ec-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd0ec-110">none</span><span class="sxs-lookup"><span data-stu-id="dd0ec-110">none</span></span>|<span data-ttu-id="dd0ec-111">0</span><span class="sxs-lookup"><span data-stu-id="dd0ec-111">0</span></span>|<span data-ttu-id="dd0ec-112">Значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="dd0ec-112">Default value, no intent.</span></span>|
|<span data-ttu-id="dd0ec-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="dd0ec-113">appsInListCompliant</span></span>|<span data-ttu-id="dd0ec-114">1</span><span class="sxs-lookup"><span data-stu-id="dd0ec-114">1</span></span>|<span data-ttu-id="dd0ec-115">Список представляет приложений, которые будут считаться спецификации (только для приложений в списке совместимых).</span><span class="sxs-lookup"><span data-stu-id="dd0ec-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="dd0ec-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="dd0ec-116">appsNotInListCompliant</span></span>|<span data-ttu-id="dd0ec-117">2</span><span class="sxs-lookup"><span data-stu-id="dd0ec-117">2</span></span>|<span data-ttu-id="dd0ec-118">Представляет список приложений, которые будут считаться несовместимой (все приложения совместимых за исключением приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="dd0ec-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



