---
title: Тип перечисления appListType
description: Возможные значения список соответствия требованиям приложения.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 76c13c26812fd8ab7c8e1224b55e616502b514ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839272"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="3cd22-103">Тип перечисления appListType</span><span class="sxs-lookup"><span data-stu-id="3cd22-103">appListType enum type</span></span>

> <span data-ttu-id="3cd22-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3cd22-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cd22-105">Возможные значения список соответствия требованиям приложения.</span><span class="sxs-lookup"><span data-stu-id="3cd22-105">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="3cd22-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="3cd22-106">Members</span></span>
|<span data-ttu-id="3cd22-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="3cd22-107">Member</span></span>|<span data-ttu-id="3cd22-108">Значение</span><span class="sxs-lookup"><span data-stu-id="3cd22-108">Value</span></span>|<span data-ttu-id="3cd22-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3cd22-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cd22-110">Нет</span><span class="sxs-lookup"><span data-stu-id="3cd22-110">none</span></span>|<span data-ttu-id="3cd22-111">0</span><span class="sxs-lookup"><span data-stu-id="3cd22-111">0</span></span>|<span data-ttu-id="3cd22-112">Значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="3cd22-112">Default value, no intent.</span></span>|
|<span data-ttu-id="3cd22-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="3cd22-113">appsInListCompliant</span></span>|<span data-ttu-id="3cd22-114">1</span><span class="sxs-lookup"><span data-stu-id="3cd22-114">1</span></span>|<span data-ttu-id="3cd22-115">Список представляет приложений, которые будут считаться спецификации (только для приложений в списке совместимых).</span><span class="sxs-lookup"><span data-stu-id="3cd22-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="3cd22-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="3cd22-116">appsNotInListCompliant</span></span>|<span data-ttu-id="3cd22-117">2</span><span class="sxs-lookup"><span data-stu-id="3cd22-117">2</span></span>|<span data-ttu-id="3cd22-118">Представляет список приложений, которые будут считаться несовместимой (все приложения совместимых за исключением приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="3cd22-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



