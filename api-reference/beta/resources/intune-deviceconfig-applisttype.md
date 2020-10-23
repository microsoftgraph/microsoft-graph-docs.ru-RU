---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 79bf27c55b1bb237cac8c537473e8ffd98edca7a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708825"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="f9a01-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="f9a01-103">appListType enum type</span></span>

<span data-ttu-id="f9a01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9a01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9a01-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9a01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9a01-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9a01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9a01-107">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="f9a01-107">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="f9a01-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f9a01-108">Members</span></span>
|<span data-ttu-id="f9a01-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f9a01-109">Member</span></span>|<span data-ttu-id="f9a01-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f9a01-110">Value</span></span>|<span data-ttu-id="f9a01-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f9a01-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9a01-112">none</span><span class="sxs-lookup"><span data-stu-id="f9a01-112">none</span></span>|<span data-ttu-id="f9a01-113">нуль</span><span class="sxs-lookup"><span data-stu-id="f9a01-113">0</span></span>|<span data-ttu-id="f9a01-114">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="f9a01-114">Default value, no intent.</span></span>|
|<span data-ttu-id="f9a01-115">аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="f9a01-115">appsInListCompliant</span></span>|<span data-ttu-id="f9a01-116">1,1</span><span class="sxs-lookup"><span data-stu-id="f9a01-116">1</span></span>|<span data-ttu-id="f9a01-117">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="f9a01-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="f9a01-118">аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="f9a01-118">appsNotInListCompliant</span></span>|<span data-ttu-id="f9a01-119">2</span><span class="sxs-lookup"><span data-stu-id="f9a01-119">2</span></span>|<span data-ttu-id="f9a01-120">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="f9a01-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





