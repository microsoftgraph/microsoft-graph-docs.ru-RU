---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8e76b06d474f642f26655fa7f1b8e07e540b7495
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051104"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="f75c6-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="f75c6-103">appListType enum type</span></span>

<span data-ttu-id="f75c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f75c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f75c6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f75c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f75c6-106">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="f75c6-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="f75c6-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f75c6-107">Members</span></span>
|<span data-ttu-id="f75c6-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f75c6-108">Member</span></span>|<span data-ttu-id="f75c6-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f75c6-109">Value</span></span>|<span data-ttu-id="f75c6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f75c6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f75c6-111">Нет</span><span class="sxs-lookup"><span data-stu-id="f75c6-111">none</span></span>|<span data-ttu-id="f75c6-112">нуль</span><span class="sxs-lookup"><span data-stu-id="f75c6-112">0</span></span>|<span data-ttu-id="f75c6-113">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="f75c6-113">Default value, no intent.</span></span>|
|<span data-ttu-id="f75c6-114">аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="f75c6-114">appsInListCompliant</span></span>|<span data-ttu-id="f75c6-115">1 </span><span class="sxs-lookup"><span data-stu-id="f75c6-115">1</span></span>|<span data-ttu-id="f75c6-116">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="f75c6-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="f75c6-117">аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="f75c6-117">appsNotInListCompliant</span></span>|<span data-ttu-id="f75c6-118">2 </span><span class="sxs-lookup"><span data-stu-id="f75c6-118">2</span></span>|<span data-ttu-id="f75c6-119">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="f75c6-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|









