---
title: тип перечисления Апплисттипе
description: Возможные значения списка приложений для обеспечения соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7cd3e1f8cffa747ca23e00ba0d9264cb1089dee2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260819"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="f4f15-103">тип перечисления Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="f4f15-103">appListType enum type</span></span>

<span data-ttu-id="f4f15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4f15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4f15-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4f15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4f15-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4f15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4f15-107">Возможные значения списка приложений для обеспечения соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="f4f15-107">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="f4f15-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="f4f15-108">Members</span></span>
|<span data-ttu-id="f4f15-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="f4f15-109">Member</span></span>|<span data-ttu-id="f4f15-110">Значение</span><span class="sxs-lookup"><span data-stu-id="f4f15-110">Value</span></span>|<span data-ttu-id="f4f15-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f4f15-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4f15-112">Нет</span><span class="sxs-lookup"><span data-stu-id="f4f15-112">none</span></span>|<span data-ttu-id="f4f15-113">нуль</span><span class="sxs-lookup"><span data-stu-id="f4f15-113">0</span></span>|<span data-ttu-id="f4f15-114">Значение по умолчанию без намерения.</span><span class="sxs-lookup"><span data-stu-id="f4f15-114">Default value, no intent.</span></span>|
|<span data-ttu-id="f4f15-115">аппсинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="f4f15-115">appsInListCompliant</span></span>|<span data-ttu-id="f4f15-116">1,1</span><span class="sxs-lookup"><span data-stu-id="f4f15-116">1</span></span>|<span data-ttu-id="f4f15-117">Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).</span><span class="sxs-lookup"><span data-stu-id="f4f15-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="f4f15-118">аппснотинлисткомплиант</span><span class="sxs-lookup"><span data-stu-id="f4f15-118">appsNotInListCompliant</span></span>|<span data-ttu-id="f4f15-119">2</span><span class="sxs-lookup"><span data-stu-id="f4f15-119">2</span></span>|<span data-ttu-id="f4f15-120">Список представляет приложения, которые будут считаться несовместимыми (все приложения являются совместимыми, кроме приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="f4f15-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|




