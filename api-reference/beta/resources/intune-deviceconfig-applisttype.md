---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 61999950fbf9a54a2d93576fe77d950e30b8b561
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469954"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="26334-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="26334-103">appListType enum type</span></span>

<span data-ttu-id="26334-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26334-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26334-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26334-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26334-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="26334-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26334-107">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="26334-107">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="26334-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="26334-108">Members</span></span>
|<span data-ttu-id="26334-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="26334-109">Member</span></span>|<span data-ttu-id="26334-110">Значение</span><span class="sxs-lookup"><span data-stu-id="26334-110">Value</span></span>|<span data-ttu-id="26334-111">Описание</span><span class="sxs-lookup"><span data-stu-id="26334-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26334-112">Нет</span><span class="sxs-lookup"><span data-stu-id="26334-112">none</span></span>|<span data-ttu-id="26334-113">нуль</span><span class="sxs-lookup"><span data-stu-id="26334-113">0</span></span>|<span data-ttu-id="26334-114">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="26334-114">Default value, no intent.</span></span>|
|<span data-ttu-id="26334-115">аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="26334-115">appsInListCompliant</span></span>|<span data-ttu-id="26334-116">1,1</span><span class="sxs-lookup"><span data-stu-id="26334-116">1</span></span>|<span data-ttu-id="26334-117">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="26334-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="26334-118">аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="26334-118">appsNotInListCompliant</span></span>|<span data-ttu-id="26334-119">2</span><span class="sxs-lookup"><span data-stu-id="26334-119">2</span></span>|<span data-ttu-id="26334-120">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="26334-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



