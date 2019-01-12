---
title: Тип перечисления appListType
description: Возможные значения список соответствия требованиям приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1439ab860ab6a1fbf9ff4deb30320bb57fba338
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967240"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="d8e28-103">Тип перечисления appListType</span><span class="sxs-lookup"><span data-stu-id="d8e28-103">appListType enum type</span></span>

> <span data-ttu-id="d8e28-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d8e28-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8e28-105">Возможные значения список соответствия требованиям приложения.</span><span class="sxs-lookup"><span data-stu-id="d8e28-105">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="d8e28-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="d8e28-106">Members</span></span>
|<span data-ttu-id="d8e28-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="d8e28-107">Member</span></span>|<span data-ttu-id="d8e28-108">Значение</span><span class="sxs-lookup"><span data-stu-id="d8e28-108">Value</span></span>|<span data-ttu-id="d8e28-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d8e28-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8e28-110">Нет</span><span class="sxs-lookup"><span data-stu-id="d8e28-110">none</span></span>|<span data-ttu-id="d8e28-111">0</span><span class="sxs-lookup"><span data-stu-id="d8e28-111">0</span></span>|<span data-ttu-id="d8e28-112">Значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="d8e28-112">Default value, no intent.</span></span>|
|<span data-ttu-id="d8e28-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="d8e28-113">appsInListCompliant</span></span>|<span data-ttu-id="d8e28-114">1</span><span class="sxs-lookup"><span data-stu-id="d8e28-114">1</span></span>|<span data-ttu-id="d8e28-115">Список представляет приложений, которые будут считаться спецификации (только для приложений в списке совместимых).</span><span class="sxs-lookup"><span data-stu-id="d8e28-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="d8e28-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="d8e28-116">appsNotInListCompliant</span></span>|<span data-ttu-id="d8e28-117">2</span><span class="sxs-lookup"><span data-stu-id="d8e28-117">2</span></span>|<span data-ttu-id="d8e28-118">Представляет список приложений, которые будут считаться несовместимой (все приложения совместимых за исключением приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="d8e28-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



